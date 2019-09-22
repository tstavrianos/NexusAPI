###NexusAPI

Handler for the NexusMods api, implemented using [RestEase](https://github.com/canton7/RestEase) and [Newtonsoft.Json](https://www.newtonsoft.com/json).
The response classes were copied from the models classes in [FluentNexus](https://github.com/Pathoschild/FluentNexus).

The design of the project is still in flux and will probably change in the future.

####Features
* Throttles all requests, so as to abide by the rules of use stated on the NexusMods website.
* Checks allowed daily and hourly limits and postpones requests if these have been exceeded (implementation for this is working but will probably change).
* Caches all requests (currently Mods, ModFiles and DownloadLinks only).

####Todo
* Actually write a proper readme.
* Document the api calls.
* Add wrappers for the rest of the api calls that use throttling and caching.
