##### Order Status
ENTER SQL SERVER MANAGEMENT, RIGHT CLICK ON THE SERVER AND CREATE A NEW DATABASE FOR EXAMPLE "ConnectionDb" THEN PASTE THE QUERY I GIVEN FOR ORDER STATUS AS A NEW QUERY AND EXECUTE IT
WHILE DOING THESE, CHECK THE DATASE CONNECTION IN THE APPSETTINGS.JSON FILE


TO LOG IN TO THE ADMIN PANEL

admin@gmail.com
Admin@123


[ORDER STATU QUERY]
```sql
   USE [BookShoppingCartMvc]
   GO
   SET IDENTITY_INSERT [dbo].[OrderStatus] ON 
   GO
   INSERT [dbo].[OrderStatus] ([Id], [StatusId], [StatusName]) VALUES (1, 1, N'Pending')
   GO
   INSERT [dbo].[OrderStatus] ([Id], [StatusId], [StatusName]) VALUES (2, 2, N'Shipped')
   GO
   INSERT [dbo].[OrderStatus] ([Id], [StatusId], [StatusName]) VALUES (3, 3, N'Delivered')
   GO
   INSERT [dbo].[OrderStatus] ([Id], [StatusId], [StatusName]) VALUES (4, 4, N'Cancelled')
   GO
   INSERT [dbo].[OrderStatus] ([Id], [StatusId], [StatusName]) VALUES (5, 5, N'Returned')
   GO
   INSERT [dbo].[OrderStatus] ([Id], [StatusId], [StatusName]) VALUES (6, 6, N'Refund')
   GO
   SET IDENTITY_INSERT [dbo].[OrderStatus] OFF
   GO
