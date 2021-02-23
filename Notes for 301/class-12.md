## Reading Notes 12 | Code 301 | EJS Partials

A partial can be made with EJS in which HTML that appears across several pages can
be made into one small file for reuse.
to include a partial file in a page you must use
    <%- include( PARTIAL_FILE ) %>

The html is stuctured as normal for the index or about or search page, but the instert partial statements go in place of reused footers or nav bars or forms.

It's an easy way to get reusable content.

[Back to Table of Contents](../README.md)