# Search_Aggregator
This is a simple search aggregator that aggregates search results from Google and Bing.

-Built in .NET MVC
-For Google, I used NuGet for the visual studio API tool and created a simple search engine to allow *.com, *.net, *.org and *.ca searches.
-For Bing, I parsed the json received after sending a GET request to their API.
-I put the API services into different service classes that implement ISearchService interface. 
 Then, I used Visual Studio Unity tool to create a container that registers the different searches. 
 After, I inject the service into the controller which calls each of the services and appends the results.
 By doing this, modularity is increased and it becomes easy to add or remove more search services.