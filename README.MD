Take a list of domain names from "list.txt" and add those containing ".co.uk" and write them as rules to a file "output.json"

For the required format, see "outputExample.json" as a reference. Each domain added should be an item in the "rules" list as follows;

For a domain name "approvedpattesting.co.uk"
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

Every email that contains .co.uk in the list should be displayed like the above in the final output.json.

Modify the content of "process.js" to achieve the above.
