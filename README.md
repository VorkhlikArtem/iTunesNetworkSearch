# iTunes App
The app allows searching different media types in ITunes: movies, books, music, apps. It provides 2 viewing modes of items: single row mode(TableView) and 3 items in a row(CollectionView).    

## About Techniques
- ITunes API for fetching tracks
* Concurrency:
  * async/await 
  * Task (for creating concurrent environment) with capability of cancellation if a result won't be useful
  * ThrowingTaskGroup for running multiple child tasks 
  * actors (@MainActor)

- KeyedDecodingContainer for decoding fetched data from the network
- UICollectionView Compositional Layout & UICollectionView Diffable Datasource
- Container View for displaying 2 child VCs: Collection and Table VCs
- perform(_:with:afterDelay:inModes:) for delaying requests from search bar input


## Screenshots 
<p align="center">
  <img src= "https://github.com/VorkhlikArtem/iTunesNetworkSearch/assets/115653999/45b9be87-e7f5-4637-85b5-bc4d02bfd538" width="170">
  <img src= "https://github.com/VorkhlikArtem/iTunesNetworkSearch/assets/115653999/d1e7e7b5-9655-4480-a22c-923027eb98df" width="170">
  <img src= "https://github.com/VorkhlikArtem/iTunesNetworkSearch/assets/115653999/4d678fb2-c896-48a7-8cf9-510e4bda39c6" width="170">  
</p>

<p align="center">
  <img src= "https://github.com/VorkhlikArtem/iTunesNetworkSearch/assets/115653999/01249798-0282-4f22-b35c-ffa97098aae1" width="200">
  <img src= "https://github.com/VorkhlikArtem/iTunesNetworkSearch/assets/115653999/f78247ed-5499-490a-8d08-ae670ebb3c36" width="200">
  <img src= "https://github.com/VorkhlikArtem/iTunesNetworkSearch/assets/115653999/7d06d32b-ce63-4c7b-a747-39b5762581eb" width="200">  
</p>


## Requirements
- IOS 13.0+
- IPhone 7+
- XCode 13.0+
