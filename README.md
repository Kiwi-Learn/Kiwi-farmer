# kiwi-farmer

## Package your code

```
zip -r kiwi_farmer.zip .
```

## Upload your code

```
iron worker upload --zip kiwi_farmer.zip --name kiwi_farmer iron/images:ruby-2.1 ruby kiwi_farmer.rb
```

## Queue / Schedule jobs for your worker

With `--payload-file` option can set up your credential file path, so you don't need upload your credential to IronWorker.

```
iron worker queue --payload-file ../config/config.json --wait kiwi_farmer
```
