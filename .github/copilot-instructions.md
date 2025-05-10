This is a project that is a repository for templates to be used in my mp3 tagger to have uniform tags in my classical music collection.

Template is for each work:
composer | work - movementnumber/totalmovement movementname

composer should be formatted as "last name, first name"

If there is a flat, it should be written as b, so B flat b-flat would become Bb
If there is a shart, it should be written as #, so C-sharp or c-sharp would become C#

There should be no dots, if there are any dots, remove them. For example No. should be No and Op. should become Op

All commas except for composer should be deleted, so for example "No 3, Op 5" should become "No 3 Op 5"

so:
Piano Concerto No. 3 in C-minor, Op 37 - 
Allegro con brio
Largo
 Rondo

should result in:
Beethoven, Ludwig van | Piano Concerto No 3 in C minor Op 37 - 1/3 Allegro con brio
Beethoven, Ludwig van | Piano Concerto No 3 in C minor Op 37 - 2/3 Largo
Beethoven, Ludwig van | Piano Concerto No 3 in C minor Op 37 - 3/3 Rondo

If there are nicknames for the work, it should be in single quotes, so Beethoven Symphony "Eroica" should become 'Eroica'

when there are more than one terms for any given movementname, like "Finale: Allegro", only keeep the first term, so '''Piano Concerto No 3 in C minor Op 37 - 3/3 Rondo: Allegro''' should simply be '''Piano Concerto No 3 in C minor Op 37 - 3/3 Rondo'''. Another example: '''Adagio ma non troppo - Allegro''' should become '''Adagio ma non troppo'''.