---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<SearchRequest> requestsList = new LinkedList<SearchRequest>();
SearchRequest requests = new SearchRequest();
LinkedList<EntityType> entityTypesList = new LinkedList<EntityType>();
entityTypesList.add(EntityType.EVENT);
requests.entityTypes = entityTypesList;
SearchQuery query = new SearchQuery();
query.queryString = "test";
requests.query = query;
requests.from = 0;
requests.size = 15;
requests.enableTopResults = true;

requestsList.add(requests);

graphClient.search()
	.query(SearchEntityQueryParameterSet
		.newBuilder()
		.withRequests(requestsList)
		.build())
	.buildRequest()
	.post();

```