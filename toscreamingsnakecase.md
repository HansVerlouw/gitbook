# ToScreamingSnakeCase

sed script to replace old ICMS variables with new variables in SCREAMING\_SNAKE\_CASE

Usage:

* open bash
* run the sed command like: `sed -f ToScreamingSnakeCase.sed <input-file>`
* or: `sed -f ToScreamingSnakeCase.sed <input-file> > <output-file>`

Git: https://git.geodan.io/icms/icms-system-engineering/-/blob/develop/ToScreamingSnakeCase.sed

Example:

sed -f /d/Projecten/Incident\ Management/ToScreamingSnakeCase.sed docker-compose-icm2.yml > docker-compose-icm2\_new.yml
