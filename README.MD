# Tech Test
We have a list of domain names in the file "list.txt". The domain names end in various ways e.g. .com, .eu, .co.uk etc.
We also have our "input.js" file that contains a JSON.
## Your Task
Collect only those domains from the "list.txt" file that ends with .co.uk and reorganize each domain into the following object where "value" is the domain you have collected.
```
{
 "id": "emailAddress",
 "field": "emailAddress",
 "type": "string",
 "operator": "contains",
 "value": "approvedpattesting.co.uk"
 }
```

For the finished example, see "outputExample.json" as a reference for what the final outcome should be. For example for the domain name "approvedpattesting.co.uk";

```
{
 "condition": "OR",
 "not": false,
 "version": 2,
 "rules": [
 ...,
 {
 "id": "emailAddress",
 "field": "emailAddress",
 "type": "string",
 "operator": "contains",
 "value": "approvedpattesting.co.uk"
 },
 ....
 ],
 "valid": true
}
```
Every email that contains ".co.uk" in the list should be displayed like the above in the final "output.json" file.
Modify the content of "process.js" to achieve this.
