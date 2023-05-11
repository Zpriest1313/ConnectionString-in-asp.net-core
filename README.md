# ConnectionString-in-asp.net-core
  // connection string in app.setting.json
  "ConnectionStrings": {
    "DefaultConnection": "Server=./;Database=RepositoryDesignPatternMVC;Trusted_Connection=true;TrustServerCertificate=true "
  }
  // add service of Dbcontext in program.cs at startup
  builder.Services.AddDbContext<EmployeeContext>(options => options.UseSqlServer(builder.Configuration.GetConnectionString("DefaultConnection")));
// install at tools NuGet manager
  EntityFramework.Core
  EntityFrameWork.Core.SqlServer
  EnttiyFramework.Core.tools
  // package manager console
  add-migration nameofmigration
  update-database
