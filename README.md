# EF6DBFirstDemo
F6DBFirstDemo Original 
== Install-Package Microsoft.SqlServer.Types		
	Following a comment in an answer for current post, adding these two lines (preferebly to the main function) solved my problem for
	 Console App:
			SqlProviderServices.SqlServerTypesAssemblyName = typeof(SqlGeography).Assembly.FullName;
        		SqlServerTypes.Utilities.LoadNativeAssemblies(AppDomain.CurrentDomain.BaseDirectory);
							
              using System.Data.Entity.Spatial;
              using System.Data.Entity.SqlServer;
