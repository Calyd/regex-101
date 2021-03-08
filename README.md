# Regex 101

## The Raw Data
```text
Giusto Metzing (gmetzing0@dyndns.org); Nerti Braban (nbraban1@hibu.com); Nissa Vigurs (nvigurs2@washington.edu); Bridgette Bewly (bbewly3@goo.gl); Storm Beneteau (sbeneteau4@ustream.tv); Nollie Dresse (ndresse5@google.cn); Fallon Mintram (fmintram6@purevolume.com); Ros Baylis (rbaylis7@vimeo.com); Lorri Burchess (lburchess8@springer.com); Rosella Ponte (rponte9@zimbio.com);
```
## Split to New Lines on Semicolon

Search expression: `; {0,1}`

Replace expression: `\n`

```text
Giusto Metzing (gmetzing0@dyndns.org)
Nerti Braban (nbraban1@hibu.com)
Nissa Vigurs (nvigurs2@washington.edu)
Bridgette Bewly (bbewly3@goo.gl)
Storm Beneteau (sbeneteau4@ustream.tv)
Nollie Dresse (ndresse5@google.cn)
Fallon Mintram (fmintram6@purevolume.com)
Ros Baylis (rbaylis7@vimeo.com)
Lorri Burchess (lburchess8@springer.com)
Rosella Ponte (rponte9@zimbio.com)
```

## Convert to `FirstName LastName (e-mail address)` format

Search expression: `(.*),(.*),(.*)`

Replace expression: `$1 $2 ($3)`

```text
Giusto Metzing (gmetzing0@dyndns.org)
Nerti Braban (nbraban1@hibu.com)
Nissa Vigurs (nvigurs2@washington.edu)
Bridgette Bewly (bbewly3@goo.gl)
Storm Beneteau (sbeneteau4@ustream.tv)
Nollie Dresse (ndresse5@google.cn)
Fallon Mintram (fmintram6@purevolume.com)
Ros Baylis (rbaylis7@vimeo.com)
Lorri Burchess (lburchess8@springer.com)
Rosella Ponte (rponte9@zimbio.com)
```

## Remove E-mail Address

Search expression: `(.*) (.*) .*`

Replace expression: `$1 $2`

```text
Giusto Metzing
Nerti Braban
Nissa Vigurs
Bridgette Bewly
Storm Beneteau
Nollie Dresse
Fallon Mintram
Ros Baylis
Lorri Burchess
Rosella Ponte
```
