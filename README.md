<h1>Bookmap + Order book</h1>
The bookmap serves to see the depth of market (DOM or Level 2) using a heat map, which is useful to detect capital injections, aggressive and passive orders, aggressive levels of volume and also comes with an Order Book that shows the distribution of the price along with the total amount of volume in the market (both Total and Bid/Ask).

It is a very complete tool because it allows us to apply filters of orders and data to numerical and percentage level, plus a wide range of styles that lets us vary from colors to size of the letters and limits, but that's not all ... There is an option called "Realtime save session" within "Book Map Database" with which we can record in real time all the data extracted by the Bookmap and then save it in a .db file, this is very useful because we can reload the session whenever we want and not lose any progress. Another great feature is to be able to use this file (if you know how to read it) for data analysis, applying Machine Learning or any statistical method to look for patterns, in fact this is the purpose of such functionality.

If you see my examples all of it is "1 second" of time-frame, this is because with this setup we can able to see the market in a very precision way. Experts algorithms can use this for detect market manipulation and High frequency trading(HFT).

Features:
* Ladder range: x(levels of the ladder of contracts)
* Market orders calculation: Delta, Total.
Book map database:
* Session save file path: filename.db(the ".db" is obligatory)
* Session load file path: filename.db(the name of the file saved previously)
* Realtime save session: True/Falta(do you want to save?, enable this option!)
Book map Filters:
* Agressive market orders: X(detect agressive volume from X, this is show in the price)
* Big pending orders: Y(detect orders from Y, it is useful for detect HFT)

<h1>Order Flow</h1>
The order flow is a tool that allows us to see the flow of orders in the market, with this we can see the difference between
the level of supply and demand. A good trader(or an AI algorithm in my case) can provide us information about a possible future price imbalance, and using this knowledge exploit a resistance point at which to place an order.
In other words, the order flow shows us the number of contracts at each price level, which is why it is sometimes also called "Cluster Chart" or "Footprint".

This tools offers a lot of styles and formulas to deal with it:
* Formulas: Bid/Ask, Total Delta, Total, Delta
* Representation: Volume(raw numbers), Percent
* Position(Profile): Left, Right
* Style: Profile, Heatmap
* Cluster POC, POC Lines, Cluster POI, POI Lines
* Extra info: POC = Point of control(Maximum volume cluster), POI = Point of imbalance(Minimum volume cluster)

<h1>Volume Profile</h1>

The volume profile shows a horizontal distribution of the number of contracts traded at each price level over a period of time. It also provides additional information such as POC, POI, Delta volume, Total Volume over a certain period of time.
One of its features is that it gives us the possibility to drag and drop, so we can select price zones and make a volume profile (we can also delete them when we don't need them).

Features:
* Formulas: Total, Delta, BidAsk, TotalAndBidAsk, TotalAndDelta, TotalAndDeltaAndBidAskm
* Ladder information: BidAsk, TotalAndDelta, Total, Delta.
* Time: Days, Minutes, Hours
* POC and POI.
* Hold CTRL and select a zone in the chart(the selected area will be marked in blue), then left click to show a new Volume Profile.
* Hold SHIFT and select an added Volume Profile(if the selected area is correct will be marked in red), then left click to delete a Volume Profile.

<h1>Volume Filter</h1>

The volume filter is an indispensable weapon when we need to detect areas of important volume, probably the market is in a battle between buyers and sellers. Sometimes we will only filter out a specific amount of volume while at other times we will need a "map" of all incoming volume (from the smallest to the most aggressive). This tool is very useful if is combined, for example with the Book Map.

Features:
* Formula: Delta, Total.
* Min volume filter: X(a volume less than this amount will be discarted)
Geometry:
* Drawn: Circle, Rectangle.
* Fill: True, False.
* Agressive level: X(this impact on the size of the volume zone).
* Among others...

<h1>Market Volume</h1>

This is the simplest volume analysis tool, and one of the most used... with it we can see the total amount of Delta volume, accumulated volume among other characteristics. One of the most innovative things is that we can choose cumulative time-frames (most tools of this type only allow a fixed time) as a default period. So we can set volume time-frames.

Features:
* Formula: BidAsk, Delta, Total, TotalBidAsk, TotalDelta.
* Period: 1(by default, if we increase this amount we can accumulate the volume period)
* Market calculation style: Zero Line Color
