
## Step 1

Create a new "random_form" module.  Starting at the root of the Drupal directory:
```
cd sites/all/modules/
mkdir random_form
cd random_form
```

Create two files: random_form.info and random_form.module with contents of tag [form-step01](https://github.com/ultrasaurus/drupal_module_example/tree/form-step01)

Go to: http://localhost/~sarah/drupal_dev/?q=examples/random
![Alt text](https://monosnap.com/image/uJ7eez7bw55B5CydVxzGkLd3n.png)

## Step 2
Display Results

Create a function that returns a "render array" to display the results.  Use hook_menu to call that from a specific URL.  Specify the page to render as as redirect to the URL in hook_form_submit.

More details at tag [form-step02](https://github.com/ultrasaurus/drupal_module_example/tree/form-step02)


![Alt text](https://monosnap.com/image/HoPk9kMzTRPWB1yA6Q20GByxW.png)
