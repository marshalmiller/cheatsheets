### [SQL](../README.md)
# Triggers

Database Triggers

A database trigger is associated with a specific table, view, or foreign table.
Database Trigger Query Types

In a database, triggers execute a specified function when certain operations are performed on the table (INSERT, UPDATE, DELETE, TRUNCATE). SELECT statements do not modify rows so no trigger can be set on a SELECT statement.
Database Triggers Timing

In a database, triggers can run before, after, or instead of the operation that fired them attempts to alter the row(s).
Triggers: FOR EACH ROW and FOR EACH STATEMENT

In PostgreSQL, a trigger set FOR EACH ROW is called once for every row modified. FOR EACH STATEMENT executes once for the entire operation (0 modified rows would still trigger this).
Database Triggers When Clause

A database trigger can specify a boolean WHEN condition to set when it should be fired.
Database Trigger Cascading

Multiple database triggers of the same kind can exist on the same table. If so, they are triggered in alphabetical order.
Database Trigger Dropping

To remove a trigger from a table/view you can use the DROP TRIGGER command.
Database Triggers Cascading

One SQL command can trigger more than one kind of trigger. For example, an insert can fire a trigger that updates a record creating a conflict that triggers an update on conflict trigger.
