[article]:
  type
    http://schema.org/ScholarlyArticle
  title
    My First Article About _Escherichia coli_
  sameAs
    http://dx.doi.org/10.1234/example.1
  datePublished
    2015-03-15T12:00:00
  author
    [alice-jones]
    [bob-smith]
  contributor
    [role-investigation]
    [role-software]
  funder
    [mrc123]
    [mrc456]
    [nih123]
    
[alice-jones]:
  type
    http://schema.org/Person
  name
    Alice Jones
  email
    alice.jones@example.com
  sameAs
    http://orcid.org/00000000-0000-0000-000002
  affiliation
    [harvard]

[bob-smith]:
  type
    http://schema.org/Person
  name
    Bob Smith
  email
    bob.smith@example.com
  sameAs
    http://orcid.org/00000000-0000-0000-000001
  url
    http://example.org/authors/1
  affiliation
    [stanford]


[harvard]:
  type
    http://schema.org/Organization
  address
    Department, Institution, City, State, Country

[stanford]:
  type
    http://schema.org/Organization
  address
    Department, Institution, City, State, Country
  url
    http://mathematics.stanford.edu/    

[role-investigation]:
  type
    http://schema.org/Role
  url
    http://dictionary.casrai.org/Contributor_Roles/Investigation
  description
    carried out the investigation
  startDate
    2015-01-01
  endDate
    2015-01-31
  contributor
    [bob-smith]
    [alice-jones]

[role-software]:
  type
    http://schema.org/Role
  url
    http://dictionary.casrai.org/Contributor_Roles/Software
  description
    wrote the software
  contributor
    [alice-jones]

[role-draft]:
  type
    http://schema.org/Role
  url
    http://dictionary.casrai.org/Contributor_Roles/Writing_%E2%80%93_original_draft
  description
    wrote the manuscript
  contributor
    [alice-jones]

[role-review]:
  type
    http://schema.org/Role
  url
    http://dictionary.casrai.org/Contributor_Roles/Writing_%E2%80%93_review_%26_editing
  description
    reviewed and edited the manuscript
  contributor
    [bob-smith]

[mrc123]:
  type
    http://schema.org/PayAction
  name
    MRC123
  agent
    [mrc]
  recipient
    [bob-smith]
    [alice-jones]

[mrc456]:
  type
    http://schema.org/PayAction
  name
    MRC456
  agent
    [mrc]
  recipient
    [bob-smith]
    [alice-jones]

[nih123]:
  type
    http://schema.org/PayAction
  name
    NIH123
  agent
    [nih]
  recipient
    [alice-jones]

[mrc]:
  type
    http://schema.org/Organization
  name
    Medical Research Council
  sameAs
    http://dx.doi.org/10.13039/501100000265

[nih]:
  type
    http://schema.org/Organization
  name
    National Institutes of Health
  url
    http://www.nih.gov/
  sameAs
    http://dx.doi.org/10.13039/100000002
