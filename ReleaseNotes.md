# SignalR Release Notes
# 1.0rc1 (Official Release)
* Drain pending writes before ending the request to avoid AVs. ([010c4f6750](https://github.com/SignalR/SignalR/commit/010c4f675039bcf06bde9b8e68f8178f86501de4))
* Bubble canceled tasks via hubs back to the client. ([c1e8e6834b](https://github.com/SignalR/SignalR/commit/c1e8e6834b9ddb182d751a04c5ea382d1e3c8668))
* Expose Request to the HubCallerContext. ([5ec61eb37c](https://github.com/SignalR/SignalR/commit/5ec61eb37c16369976ba66f4d5262a0bf345acfc))
* Removed Hosting.Common altogether. ([acebe530a4](https://github.com/SignalR/SignalR/commit/acebe530a4502303ffb6b669dce0a73bf2ef172d))
* Fixed deadlock in ForeverTransport. ([11da5b71a3](https://github.com/SignalR/SignalR/commit/11da5b71a3d89d5947d6797f7a0176d6d7e688e9))
* Drop silverlight4 package from build. ([33cc5e06d9](https://github.com/SignalR/SignalR/commit/33cc5e06d952d3d242de13f3728ea6843964dcd5))
* Change the default keep alive to 15 seconds. ([6741075e63](https://github.com/SignalR/SignalR/commit/6741075e630e96f8a4d96c336da19dd886b27f15))
* Server configured DisconnectTimeout is not honored by JavaScript client. ([#1086](https://github.com/SignalR/SignalR/issues/1086))
* RegisterHubs hangs for a while. ([#1063](https://github.com/SignalR/SignalR/issues/1063))
* Firefox 5 fails when stopping forever frame. ([#1060](https://github.com/SignalR/SignalR/issues/1060))
* Connection never disconnects if data is being sent to it. ([#1046](https://github.com/SignalR/SignalR/issues/1046))
* Unable to distribute to groups if transport is longpolling and HubName attribute is used. ([#1039](https://github.com/SignalR/SignalR/issues/1039))
* When an invalid transport is specified $.connection.hub.start() will auto negotiate. It should throw an error and stop the connection. ([#1037](https://github.com/SignalR/SignalR/issues/1037))
* When reconnecting, don't trigger on error for longpolling. ([#1036](https://github.com/SignalR/SignalR/issues/1036))
* Consider removing IRequestCookieCollection. ([#1034](https://github.com/SignalR/SignalR/issues/1034))
* Expose generic items bag on IRequest. ([#1033](https://github.com/SignalR/SignalR/issues/1033))
* The CancellationTokenSource has been disposed. ([#1020](https://github.com/SignalR/SignalR/issues/1020))
* MessageBusExtensions.cs disposer.Dispose() throws ObjectDisposedException. ([#1005](https://github.com/SignalR/SignalR/issues/1005))
* Remove dynamic support from .NET client. ([#996](https://github.com/SignalR/SignalR/issues/996))
* Add Version Property in JS Library. ([#994](https://github.com/SignalR/SignalR/issues/994))
* .Net Client Send() task hangs when server operation throws. ([#991](https://github.com/SignalR/SignalR/issues/991))
* Remove BOM encoding from output streams. ([#982](https://github.com/SignalR/SignalR/issues/982))
* Fix script escaping script files in forever frame. ([#950](https://github.com/SignalR/SignalR/issues/950))
* If no messages received after connection joins group and then disconnect, the connection won't be in the group. ([#938](https://github.com/SignalR/SignalR/issues/938))
* We do not escape the Message Id Parameter on the JS client. ([#937](https://github.com/SignalR/SignalR/issues/937))
* Joining group with hash in the name fails ([#935](https://github.com/SignalR/SignalR/issues/935))
* Optimized message format ([#887](https://github.com/SignalR/SignalR/issues/887))
* IE throws 'Access denied' on foreverFrame ([#873](https://github.com/SignalR/SignalR/issues/873))
* Native heap corruption while flushing from ForeverFrameTransport.KeepAlive ([#854](https://github.com/SignalR/SignalR/issues/854))
* First chance exception when webSockets connection closes. ([#821](https://github.com/SignalR/SignalR/issues/821))
* Use OWIN host exclusivly. ([9f9a18089f](https://github.com/SignalR/SignalR/commit/9f9a18089f8564926ace3a3a656efc4de51d0793))
* WebSocket closes ungracefully with no error when trying to call hub method with wrong name or parameters. ([#440](https://github.com/SignalR/SignalR/issues/440))

# 0.5.3 (Official Release)
* Improve logging for hubs in js client. ([#505](https://github.com/SignalR/SignalR/issues/505))
* Can't pass querystring when creating HubConnection. ([#581](https://github.com/SignalR/SignalR/issues/581))
* Improve errors for .NET client. ([#515](https://github.com/SignalR/SignalR/issues/515))
* Make http streaming work with Win8 client. ([a61ee958ed](https://github.com/SignalR/SignalR/commit/a61ee958edcc34a5b7c20ea0a1063f5170a14f03))
* Fix bugs related to forever loading indicators on various browsers ([#215](https://github.com/SignalR/SignalR/issues/215)), ([#383](https://github.com/SignalR/SignalR/issues/383)), ([#491](https://github.com/SignalR/SignalR/issues/491))
* Force shut down a client, server execution flow didn't go into IDisconnect.Disconnect () at all. ([#511](https://github.com/SignalR/SignalR/issues/511))
* Transport fallback should fail if onFailed called and there's no good fallback. ([#485](https://github.com/SignalR/SignalR/issues/485))
* Turn ReadStreamBuffering off for WP7 and Silverlight to enable SSE support. ([18cb087037](https://github.com/SignalR/SignalR/commit/18cb087037ca25def2e9c7afed1b510577e37beb))
* Connect/Disconnect events not firing in IE ([#501](https://github.com/SignalR/SignalR/issues/501))
* Make dictionaries in bus case in sensitive. ([5916a588f9](https://github.com/SignalR/SignalR/commit/5916a588f901160508f757dd386e57dea33410a3))
* Groups.Add within persistent connection fails under high crank load. ([#388](https://github.com/SignalR/SignalR/issues/388))
* Use the HttpClient stack in silverlight. ([b51a4144db](https://github.com/SignalR/SignalR/commit/b51a4144dba794e8f8ce3242d48799037055eb80))
* Made reconnect timeout configurable on SSE transport. ([6b869a4cd9](https://github.com/SignalR/SignalR/commit/6b869a4cd92ef5c93a1a16a087930026a6b3a6f4))
* Fix race condition when client sends immediately after connecting ([#552](https://github.com/SignalR/SignalR/issues/552))
* Make access to the state thread safe in the .NET client. ([8464514a8d](https://github.com/SignalR/SignalR/commit/8464514a8dab4a02d6134f4d94caf390d6fcb846))
* Abort the request before calling close on the request in the .NET client. ([50ee2b9b6c](https://github.com/SignalR/SignalR/commit/50ee2b9b6c05168473608742d42f2fc6ad03ac6b))
* Throw if CreateProxy called after the connection is started. ([89eb8e492c](https://github.com/SignalR/SignalR/commit/89eb8e492c6362f32b375845eb14fda229011a06))
* Fix caching negotiate response in Silverlight client ([#522](https://github.com/SignalR/SignalR/issues/522))
* Serve silverlight's cross domain policy file for self hosted server. ([eaec182fee](https://github.com/SignalR/SignalR/commit/eaec182fee09cbd038dd68081b0e1c500ac3106c))
* Expose underlying AuthenticationSchemes property ([52dbfbef12](https://github.com/SignalR/SignalR/commit/52dbfbef123c85d901cb955bf3f39b9467ab6657))
* Made exception handling fixes to SSE stream reader (C# client) ([7f0fd4ddc7](https://github.com/SignalR/SignalR/commit/7f0fd4ddc70e6fe2561a3eb6bfd0a9acf3ee4576))
* Make event names and proxy names case insensitive. ([#508](https://github.com/SignalR/SignalR/issues/508))
* Added hub events support to JavaScript client (using hubs without proxy) ([97c984754f](https://github.com/SignalR/SignalR/commit/97c984754f20bd6dda8c343983d679b8f65093c8))
* Made websocket implementation for self host on .NET 4.5. ([e94d091100](https://github.com/SignalR/SignalR/commit/e94d091100a86396d6efa81f72fca6198cbb57f1))
* LongPolling broken on ASP.NET 4.5 ([#496](https://github.com/SignalR/SignalR/issues/496)) 
* Prevented caching ajax requests on reconnect. ([fbfc65371d](https://github.com/SignalR/SignalR/commit/fbfc65371d0febbd822fcfff134edf5c083a78e1))
* Added consistent way to get a strongly typed representation of the connected clients ([fa6d0b533e](https://github.com/SignalR/SignalR/commit/fa6d0b533e7d0adb35374ce58d4cd74b7473537a))

# 0.5.2 (Official Release)
* ForeverFrame reconnect error: null frame reference ([#447](https://github.com/SignalR/SignalR/issues/447))
* Error when clicking link (IE only) ([#446](https://github.com/SignalR/SignalR/issues/446))
* Fixed zombie connections issue with forever transports ([7d5204e55d](https://github.com/SignalR/SignalR/commit/7d5204e55d6293881d6eabe85929d02808083027))
* ForeverFrame transport does not handle embedded ```</script>``` tags properly ([#413](https://github.com/SignalR/SignalR/issues/413))
* Made some modifications to js client for SSE and longpolling transports. ([5d782dc3b4](https://github.com/SignalR/SignalR/commit/5d782dc3b45b31183737ea054bb5b4897ed23b76))
* Duplicate connections on reconnect with SSE transport ([#452](https://github.com/SignalR/SignalR/issues/452))
* Added .NET 3.5 Client ([9e3a95c65f](https://github.com/SignalR/SignalR/commit/9e3a95c65fa64ee149e5929318dc6faacc37ef2e))
* Add server variables to the IRequest abstraction ([#438](https://github.com/SignalR/SignalR/issues/438))
* Forever frame slows down in IE after receiving many messages ([#458](https://github.com/SignalR/SignalR/issues/458))
* Reworked connection tracking logic ([8d27c97792](https://github.com/SignalR/SignalR/commit/8d27c977929ef6964a7926e97b3de6b463cd858f))
* Fix connect bug in IE6 with longpolling ([7ab434c02d](https://github.com/SignalR/SignalR/commit/7ab434c02d7d9015689f8988c9ed8456a91c741b))
* Optimized type conversation so we don't end up parsing JSON twice on hub calls  ([50cefbba42](https://github.com/SignalR/SignalR/commit/50cefbba422a46adb1345bd4f22e49be7ecc52d2))
* Clean up the way we use connection state in the .NET Client ([#474](https://github.com/SignalR/SignalR/issues/474))
* Added an overload to Send that allows passing an object (.NET Client) ([9c171bd8e7](https://github.com/SignalR/SignalR/commit/9c171bd8e77f79755aa43a14d0e5ab77e9e50e4a))
* Don't parse the message ID as a long (.NET client) ([#475](https://github.com/SignalR/SignalR/issues/475))
* Prevent hang on Connection.Start() ([5752d6007b](https://github.com/SignalR/SignalR/commit/5752d6007b8751a3bc723fea0405d7a0994ed82e))
* Stop EventSource before calling onFailed ([5c7536131b](https://github.com/SignalR/SignalR/commit/5c7536131bb2b501fff7d2f8a12194df5ac6705f))
* Fixed issues with cross domain websockets ([#461](https://github.com/SignalR/SignalR/issues/461))
* HeartBeat.MarkConnection(this) called twice per Send(..) in ForeverTransport ([#333](https://github.com/SignalR/SignalR/issues/333))

# 0.5.1 (Official Release)
* Windows RT client support ([#171](https://github.com/SignalR/SignalR/issues/171))
* Fixed Race condition in .NET SSE transport ([#341](https://github.com/SignalR/SignalR/issues/341))
* Added reconnect support for Websocket transport ([#395](https://github.com/SignalR/SignalR/issues/395))
* Implemented clean disconnect support on browser close ([#396](https://github.com/SignalR/SignalR/issues/396))
* Added async flush support for ASP.NET 4.5 ([#402](https://github.com/SignalR/SignalR/issues/402))
* Fixed websockets in WinJS client ([407](https://github.com/SignalR/SignalR/issues/407))
* Added connection state and new state changed event to js and .NET client ([431](https://github.com/SignalR/SignalR/issues/431))
* Check connection state before retrying in js client ([af2ae94133](https://github.com/SignalR/SignalR/commit/af2ae941339082ab21d8ea888e486a3c902e4b34))
* Turn keep alive on by default ([47e17b68ce](https://github.com/SignalR/SignalR/commit/47e17b68ce93d74a690dd9a7f918fddeb842fb02))
* Auto detect cross domain ([0a5c62438b](https://github.com/SignalR/SignalR/commit/0a5c62438bc928452bb61f75553635e5bf9e821e))
* Changed IResponse.Write and End to take ArraySegment<byte> instead of string ([f521fd2e6a](https://github.com/SignalR/SignalR/commit/f521fd2e6af967ce3603244bd7ed8606313f48a5))
* Added hubify.exe to generate the hubs file at build time ([e7672ebb60](https://github.com/SignalR/SignalR/commit/e7672ebb60e826d13528783967a88f9db7af56a2))
* Built WebSockets transport into the core.

## v0.5.0 (Official Release)
* Server Send Events connections not closing ([#369](https://github.com/SignalR/SignalR/issues/369))
* Allow HubConnection to specify hub url ([#368](https://github.com/SignalR/SignalR/issues/368))
* Added current IPrincipal to IRequest. ([e381ef1cb6](https://github.com/SignalR/SignalR/commit/e381ef1cb6c0c13087c221abdfa2833c0ae841a6))
* Remove implicit Send overload from PersistentConnection. ([44ff03aafa](https://github.com/SignalR/SignalR/commit/44ff03aafa5f5e2f3b73a5a19ac5a2437674891b))
* Regression: Method overloads no longer work in hubs because of caching. ([#362](https://github.com/SignalR/SignalR/issues/362))

## v0.5.0 RC (Stable Prerelease)
* Performance: Only register for disconnect for chunked requests on self host. (#352)
* Provide way to override default resolver in ASP.NET other than through routing. (#347)
* Performance: Only subscribe to hubs that have method subscriptions (#346)
* Don't create all hub instances on connect/reconnect/disconnect (#345)
* Hub names are case sensitive. (#344)
* Crappy error message when failing to create a hub (#343)
* Performance: InProcessMessageBus<T>.RemoveExpiredEntries takes N+1 locks to remove N entries (#335)
* Performance: Use DateTime.UtcNow instead of DateTime.Now. (7edef25411)
* Fixed incompatibility with jQuery.Validate (#328, #145).
* .NET Client Fixed race condition in Stop() after connection fails. (cd87d40583)
* ReflectedMethodDescriptor::TryGetMethod Executable Method Caching (#351)
* Disconnect is broken in webfarms (#69)

## v0.5.0 (Stable Prerelease)

### Bugs Fixed
* Missing messages in some cases (#307)
* Exception in .NET client when fiddler attached (#304)
* Calling Send multiple times fails (#260)
* Exception in .NET client SSE impl with large messages (#256)
* Invoking Hub methods with byte[] arguments fail (#245)
* Fixed encoding issues with self host (#244)
* Calling Stop then Start after Start fails doesn't restart .NET client (#226)
* Unobserved task exception on long polling transport when server is restarted during first request (#320)
* Hubs in inner classes don't work (#204)
* LongPolling raises IConnected.Reconnect too many times (#188)
* Issues with large message sizes (#163)
* Regression: Reconnect client after server restart (#24)
* Fixed Guids in Hub method parameters (#194)
* SelfHost Server not recognising remote disconnections (#214)
* Removed double deserialize from .NET client. (fbb3ea615d)

### Features
* Mono support (#58)
* Dynamic hubs implementation (#276)
* Improved serveral APIs to be more consistent (#20)
* Cross domain via jsonp (#6)
* Transports need to send "Keep Alives" (#168)
* Add Current User Identity to SignalR.Hosting.Request (#241)
* Added support fo Silverlight 5 Client (#264)

