[README.md](../README.md)

## Week 02

### 1. ASP.NET Core UI: Razor Pages (`RazorPagesMovie`)

Built from the *Get started with Razor Pages in ASP.NET Core* tutorial series.

**Project:** [w02/RazorPagesMovie/](RazorPagesMovie/)

**Key Features Implemented**:
- **CRUD Operations**: Scaffolded and customized Razor Pages (`Index`, `Create`, `Edit`, `Details`, `Delete`).
- **Database & EF Core**: Configured SQLite with EF Core migrations (`InitialCreate`).
- **Search & Filtering**: Added search bar by movie title and genre dropdown filter.
- **Validation**: Applied DataAnnotations (`[Required]`, `[StringLength]`, `[Range]`, `[RegularExpression]`).

---

### 2. ASP.NET Core UI: MVC (`MvcMovie`)

Built from the *Get started with ASP.NET Core MVC* tutorial series and completed all W02 Assignment requirements.

**Project:** [w02/MvcMovie/](MvcMovie/)

**Key Features Implemented**:
- **Custom Branding**: Configured application name to "Ederson Movies" across `_Layout.cshtml` navbar, page titles, and footer.
- **Controllers & Routing**: Implemented `HelloWorldController` and `MoviesController` with full CRUD action methods.
- **Seed Data**: Preloaded database with classic movies and personalized favorites (*Harry Potter*, *Avatar*, *The Lord of the Rings*).
- **Listing Title**: Customized the movie listing header to "Ederson's Movies".
- **Enhanced Search & Year Filter**: Implemented filtering by Title, Genre, and Year (displays movies released in the selected year or newer: `ReleaseDate.Year >= movieYear`).
- **Form UI Styling**: Improved CSS styling by adding padding to form inputs (`input`, `select`, `textarea`) in `site.css` to prevent text crowding against borders.
- **Validation**: Enforced model validation with client-side jQuery scripts and server-side checks.
