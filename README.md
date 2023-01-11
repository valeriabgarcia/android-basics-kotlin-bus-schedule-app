# Bus Scheduler App

https://developer.android.com/courses/pathways/android-basics-kotlin-unit-5-pathway-1

The Bus Scheduler app displays a list of bus stops and arrival times. Tapping a bus stop on the first screen will display a list of all arrival times for that particular stop.

The bus stops are stored in a Room database. Schedule items are represented by the `Schedule` class and queries on the data table are made by the `ScheduleDao` class. The app includes a view model to access the `ScheduleDao` and format data to be display in a list, using `Flow` to send data to a recycler view adapter.

## Summary

- Tables in a SQL database are represented in Room by Kotlin classes called entities.
- The DAO provides methods corresponding to SQL commands that interact with the database.
- ViewModel is a lifecycle aware component used to separate your app's data from its view.
- The AppDatabase class tells Room which entities to use, provides access to the DAO, and performs any setup when creating the database.
- ListAdapter is an adapter used with RecyclerView that is ideal for handling dynamically updated lists.
- Flow is a Kotlin feature for returning a stream of data and can be used with Room to ensure the UI and database are in sync.
