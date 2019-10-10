---
# The Good News

## Directives are now supported by GQL Gen 

---

# The Bad News

## We can't introspect them

Well, we can and we can't. `Deprecated` directive is a first class citizen
Directives descriptions are exposed on introspection, custom directives on fields or types etc are not

---
# What next?

---
# Wait

We can wait for [issue 300](https://github.com/graphql/graphql-spec/issues/300) to be resolved

Who knows how long that will take as it's been open since 28 April 2017 but an active pull request was opened 3 days ago (promising)

---

# Improvise

We use the MD type on a field (like comments on GCS `###some text###`) to format a table/list of metadata about a field/type. It's semi structured but will ultimately come down to string interpolation (nasty) 

--- 

# Adapt

We create a custom schema that we stitch into the upstream schemas that includes this information using the `extend` functionality ofschema stitching. GQL Gen supports this. It could be tricky but it's a way of extending an upstreams schema in a non-invasive way. 

---

# Overcome

erm no overcome I just wanted to use Improvise Adapt Overcome in a git pitch.  

