

## Step 1
Create a new "random" module.  Starting at the root of the Drupal directory:
```
cd sites/all/modules/
mkdir random
cd random
```

Create two files: random.info and random.module with contents of tag [step01](https://github.com/ultrasaurus/drupal_module_example/tree/step01)

The module does nothing, but it does appear on the Modules page -- if you are logged in as an admin, click "Modules" in the top menu.

![Step 1](https://monosnap.com/image/Y1rVL8gwga9CLFoGYyftyl0Py.png)

Check the checkbox and save to load the module.

## Step 2
Create a "block" that displays some (hard-coded) random words.

Edit random.module with contents of tag [step02](https://github.com/ultrasaurus/drupal_module_example/tree/step02)

If you type something wrong, Drupal will display a 500 error since it is configured to load our module.

```
tail /var/log/apache2/error_log
```
you may see something like:
```
[Sat Jul 27 17:29:12 2013] [error] [client ::1] PHP Parse error:  parse error in /Users/sarah/Sites/drupal_dev/sites/all/modules/random/random.module on line 31
```

In Toolbar: Structure > Blocks 
Go to the disabled section, find Random Words, choose “Content” from the popup menu and it will appear in the main content section.

