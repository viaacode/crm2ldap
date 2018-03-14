# crm2ldap

Integration between LDAP and CRM

## Introduction

TODO: introduction

## Overview

TODO: high-level overview (flow-diagram)

## Company

### Create

Method	POST 		http://localhost:10002/ldap/company/create

Header	Content-Type	application/json

Body

```json
{  
	"event_type"	: "company_added",
	"object_type"	: "company",
	"object_id"	: "15669750"
}
```

### Update

Method	POST 		http://localhost:10002/ldap/company/create

Header	Content-Type	application/json

Body

```json
{
	"event_type"	: "company_added",
	"object_type"	: "company",
	"object_id"	: "15669750"
}
```

### Delete

Method	POST 		http://localhost:10002/ldap/company/delete

Header	Content-Type	application/json

Body

```json
{
	"event_type"	: "company_deleted",
	"object_type"	: "company",
	"object_id"	: "15669750"
}
```

Method	GET	http://localhost:10002/ldap/company/delete?id=15612031

Id is teamleader id of the company

## Contact

### Related Update

Method	POST 		    http://localhost:10002/ldap/related_contacts/update

Header	Content-Type	application/json

Body

```json
{
	"event_type"	: "related_contacts_updated",
	"object_type"	: "company",
	"object_id"	: "17521500"
}
```

### Update

Method	POST 			http://localhost:10002/ldap/contact/update

Header	Content-Type	application/json

Body

```json
{
	"event_type"	: "contact_edited",
	"object_type"	: "contact",
	"object_id"	: "17963208"
}
```

### Delete

Method	GET 		http://localhost:10002/ldap/contact/delete?id=93dd48b4-a046-1037-83c4-3b668c0d1e16

UUId is EntryUUID attribute in LDAP
