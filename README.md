# WordPress Code Challenge

This is a simple Docker-based WordPress programming challenge, designed to test
general knowledge in a WordPress environment.

# Getting Started

1. Fork the repository and clone locally
2. Create the Local Environment:

```
docker-compose -f wordpress.yml up -d
```

3. Navigate to [http://localhost:8080](http://localhost:8080) to view the site.
4. Follow the onscreen instructions to install WordPress
5. Complete the **Requirements**, being sure to follow the **Rules**.
6. Commit and Push the code to the forked repository.
7. Send a Pull Request for us to review your solution.
8. Destroy the Local Environment:

```
docker-compose -f wordpress.yml down --volumes
```

# Rules

- All code should follow the [PSR12](https://www.php-fig.org/psr/psr-12/) standards.
- Complete all development using the "code-challenge" theme.
- Free to use third party libraries, but please mention their use upon submitting.
- Do not use a pre-existing plugin to complete the **Requirements**.
- Use of Google is encouraged.

# Requirements

### Create a list page using a public API to display configurable data

- Add a page template that allows adding shortcodes using Gutenberg. The template should follow the HTML5/CSS3 standards and be created in such a way that future templates can be added without repeating sections like the header or footer. Do not worry about the design and focus more on adhering to modern practices for the markup.
- Create a shortcode that displays a list of data from any public REST API, like [Earthquakes](https://earthquake.usgs.gov/fdsnws/event/1/) or even [Generated Fake Data](https://fakerapi.it/en). More resources below for finding an easy-to-use API.
- Extend the created shortcode to allow limiting the dataset. For instance, limiting to magnitude 5 earthquakes:
[\[earthquakes minmagnitude 5\]](https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minmagnitude=5)
- Add a settings page that an admin can use to configure some aspect of the shortcode, like limiting the number of results or adding an API key if its required.

# Resources

- [Docker WordPress Environment Sample](https://docs.docker.com/compose/wordpress/)
- [Public APIs](https://public-apis.io/)
- [API List](https://apilist.fun/)
