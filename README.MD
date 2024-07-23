Take a list of domain names from "list.txt" and add those containing ".co.uk" and write them as rules to a file "output.json"

For the required format, see "outputExample.json" as a reference. Each domain added should be an item in the "rules" list as follows;

For a domain name "approvedpattesting.co.uk"

    {
        "id": "emailAddress",
        "field": "emailAddress",
        "type": "string",
        "operator": "contains",
        "value": "approvedpattesting.co.uk"
    }

