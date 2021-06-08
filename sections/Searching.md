
# Searching entities to donate to

```Cirru
GET https://api.betterplace.org/de/api_v4/search.json?bounds=52.6754542%2C13.7611175%2C52.338234%2C13.08834&q=Katze
```

TODO


## URL Parameters

<table>
  <tr>
    <th>Parameter</th>
    <th>Example</th>
    <th>Required</th>
    <th>Description</th>
  </tr>
  <tr>
    <th align="left">q</th>
    <td><code>Katze</code></td>
    <td>no</td>
<td>

Fulltext search query.

</td>
  </tr>
  <tr>
    <th align="left">bounds</th>
    <td><code>52.6754542,13.7611175,52.338234,13.08834</code></td>
    <td>no</td>
<td>

A string of four comma-seperated floating point geo coordinates in
range of -180…180 for <code>sw_lat,sw_lng,ne_lat,ne_lng</code>
describing a bounding box around the search results' geo coordinates.


</td>
  </tr>
</table>


## Response Attributes


### Root Attributes

  <table>
    <tr>
      <th>Attribute</th>
      <th>Types</th>
      <th>Example</th>
      <th>Description</th>
    </tr>
    <tr>
      <th align="left">id</th>
      <td><code>number</code></td>
      <td><code>1</code></td>
<td>

An integer number ≥ 1

</td>
    </tr>
    <tr>
      <th align="left">created_at</th>
      <td><code>string</code></td>
      <td><code>"1994-11-05T13:15:30Z"</code></td>
<td>

DateTime (ISO8601 with Timezone)

</td>
    </tr>
    <tr>
      <th align="left">updated_at</th>
      <td><code>string</code></td>
      <td><code>"1994-11-05T13:15:30Z"</code></td>
<td>

DateTime (ISO8601 with Timezone)

</td>
    </tr>
    <tr>
      <th align="left">latitude</th>
      <td><code>number</code></td>
      <td><code>52.499007</code></td>
<td>

Decimal degrees based on user input

</td>
    </tr>
    <tr>
      <th align="left">longitude</th>
      <td><code>number</code></td>
      <td><code>13.44947</code></td>
<td>

Decimal degrees based on user input

</td>
    </tr>
    <tr>
      <th align="left">title</th>
      <td><code>string</code></td>
      <td><code>Katzenspass</code></td>
<td>

Name of the entity

</td>
    </tr>
    <tr>
      <th align="left">type</th>
      <td><code>string</code></td>
      <td><code>Project</code></td>
<td>

Type of the entity, either Project or FundraisingEvent

</td>
    </tr>
    <tr>
        <th align="left" style="white-space: nowrap">
          <a id="contact-ref" href="#contact">
            ↓contact
          </a>
        </th>
      <td><code>object</code></td>
      <td><code>TODO</code></td>
<td>

The public face of this entity

</td>
    </tr>
    <tr>
      <th align="left">progress_percentage</th>
      <td><code>number</code></td>
      <td><code>82</code></td>
<td>

% financed.


</td>
    </tr>
    <tr>
        <th align="left" style="white-space: nowrap">
          <a id="profile_picture-ref" href="#profile_picture">
            ↓profile_picture
          </a>
        </th>
      <td><code>null &#124; object</code></td>
      <td><code></code></td>
<td>

TODO

</td>
    </tr>
    <tr>
      <th align="left">donated_amount_in_cents</th>
      <td><code>number</code></td>
      <td><code>232323</code></td>
<td>

How many cents were already raised with the fundraising event

</td>
    </tr>
    <tr>
      <th align="left">country</th>
      <td><code>null &#124; string</code></td>
      <td><code>Berlin</code></td>
<td>

Name where this entity is located

</td>
    </tr>
    <tr>
      <th align="left">city</th>
      <td><code>null &#124; string</code></td>
      <td><code>Berlin</code></td>
<td>

Name where this entity is located

</td>
    </tr>
    <tr>
        <th align="left" style="white-space: nowrap">
          <a id="carrier-ref" href="#carrier">
            ↓carrier
          </a>
        </th>
      <td><code>null &#124; object</code></td>
      <td><code>TODO</code></td>
<td>

The organisation that carries this project

</td>
    </tr>
    <tr>
      <th align="left">donations_count</th>
      <td><code>number</code></td>
      <td><code>42</code></td>
<td>

Count of confirmed donations for this entity

</td>
    </tr>
    <tr>
      <th align="left">open_amount_in_cents</th>
      <td><code>number</code></td>
      <td><code>12382</code></td>
<td>

How many cents are needed to complete the project

</td>
    </tr>
  </table>

### <a id="contact" href="#contact-ref">↑Nested Attributes: contact</a>

  <table>
    <tr>
      <th>Attribute</th>
      <th>Types</th>
      <th>Example</th>
      <th>Description</th>
    </tr>
    <tr>
      <th align="left">contact.id</th>
      <td><code>number</code></td>
      <td><code>1</code></td>
<td>

An integer number ≥ 1

</td>
    </tr>
    <tr>
      <th align="left">contact.name</th>
      <td><code>null &#124; string</code></td>
      <td><code>"Till B."</code></td>
<td>

Display name of a betterplace.org user.
Possible formats: "Till B.", "T. Behnke", "Till Behnke".

In the case of donation-opinions the name might also be
empty/null for anonymous donations for anonymous donations.


</td>
    </tr>
    <tr>
        <th align="left" style="white-space: nowrap">
          <a id="contact.picture-ref" href="#contact.picture">
            ↓contact.picture
          </a>
        </th>
      <td><code>object</code></td>
      <td><code>//betterplace-assets.betterplace.org ↪/uploads/user/profile_picture ↪/000/000/001 ↪/fill_100x100_original_tb.jpg</code></td>
<td>

User profile picture or a fallback image

</td>
    </tr>
  </table>

### <a id="contact.picture" href="#contact.picture-ref">↑Nested Attributes: contact.picture</a>

  <table>
    <tr>
      <th>Attribute</th>
      <th>Types</th>
      <th>Example</th>
      <th>Description</th>
    </tr>
    <tr>
      <th align="left">contact.picture.fallback</th>
      <td><code>boolean</code></td>
      <td><code>true</code></td>
<td>

Specifies whether a fallback image is given or not

</td>
    </tr>
  </table>

### <a id="profile_picture" href="#profile_picture-ref">↑Nested Attributes: profile_picture</a>

  <table>
    <tr>
      <th>Attribute</th>
      <th>Types</th>
      <th>Example</th>
      <th>Description</th>
    </tr>
    <tr>
      <th align="left">profile_picture.fallback</th>
      <td><code>boolean</code></td>
      <td><code>true</code></td>
<td>

Specifies whether a fallback image is given or not

</td>
    </tr>
  </table>

### <a id="carrier" href="#carrier-ref">↑Nested Attributes: carrier</a>

  <table>
    <tr>
      <th>Attribute</th>
      <th>Types</th>
      <th>Example</th>
      <th>Description</th>
    </tr>
    <tr>
      <th align="left">carrier.id</th>
      <td><code>number</code></td>
      <td><code>1</code></td>
<td>

An integer number ≥ 1

</td>
    </tr>
    <tr>
      <th align="left">carrier.name</th>
      <td><code>string</code></td>
      <td><code>"Till B."</code></td>
<td>

The carrier can be an organisation or user.

</td>
    </tr>
    <tr>
      <th align="left">carrier.city</th>
      <td><code>string</code></td>
      <td><code>"Berlin"</code></td>
<td>

The city in which the carrier resides

</td>
    </tr>
    <tr>
        <th align="left" style="white-space: nowrap">
          <a id="carrier.picture-ref" href="#carrier.picture">
            ↓carrier.picture
          </a>
        </th>
      <td><code>object</code></td>
      <td><code>https://betterplace-assets.betterplace.org/…</code></td>
<td>

The organisation logo, user profile picture or a fallback image

</td>
    </tr>
  </table>

### <a id="carrier.picture" href="#carrier.picture-ref">↑Nested Attributes: carrier.picture</a>

  <table>
    <tr>
      <th>Attribute</th>
      <th>Types</th>
      <th>Example</th>
      <th>Description</th>
    </tr>
    <tr>
      <th align="left">carrier.picture.fallback</th>
      <td><code>boolean</code></td>
      <td><code>true</code></td>
<td>

Specifies whether a fallback image is given or not

</td>
    </tr>
  </table>
</table>

## Response Links

<table>
  <tr>
    <th>Linkname</th>
    <th>Description</th>
  </tr>
    <tr>
<th align="left">

platform

</th>
<td>

Permalink to betterplace.org

</td>
    </tr>
    <tr>
<th align="left">

self

</th>
<td>

Link to this resource itself


</td>
    </tr>
    <tr>
<th align="left">

pictures

</th>
<td>

Link to <a href="project_pictures_list.md">project pictures list</a>


</td>
    </tr>
    <tr>
<th align="left">

contact.platform

</th>
<td>

The user's profile on betterplace.org.
To view a user profile you have to be logged in.
This array is empty if the user has no useraccount
with betterplace.org but donated via one of our partner.


</td>
    </tr>
    <tr>
<th align="left">

contact.contact_data

</th>
<td>

The user's contact data. Please note that you need to be
<a href="../README.md#client-api">authenticated as a client</a> with matching
access rights in order to see this information.


</td>
    </tr>
    <tr>
<th align="left">

contact.picture.fill_100x100

</th>
<td>

100×100 Pixel

</td>
    </tr>
    <tr>
<th align="left">

contact.picture.original

</th>
<td>

Maximum sized image. This is the original image with default-cropping or user-cropping applied.

</td>
    </tr>
    <tr>
<th align="left">

profile_picture.fill_960x500

</th>
<td>

950×500 Pixel

</td>
    </tr>
    <tr>
<th align="left">

profile_picture.fill_730x380

</th>
<td>

730×380 Pixel

</td>
    </tr>
    <tr>
<th align="left">

profile_picture.fill_618x322

</th>
<td>

618×322 Pixel / DEPRECATED, will be removed after 5/2015

</td>
    </tr>
    <tr>
<th align="left">

profile_picture.fill_410x214

</th>
<td>

410×214 Pixel

</td>
    </tr>
    <tr>
<th align="left">

profile_picture.fill_270x141

</th>
<td>

270×141 Pixel / DEPRECATED, will be removed after 5/2015

</td>
    </tr>
    <tr>
<th align="left">

profile_picture.original

</th>
<td>

Maximum sized image. This is the original image with default-cropping or user-cropping applied.

</td>
    </tr>
    <tr>
<th align="left">

carrier.self

</th>
<td>

Link to this resource itself
(<a href="organisation_details.md">organisation details</a>)
Note: Since the there is no api for users yet, this is only
set for organisations.


</td>
    </tr>
    <tr>
<th align="left">

carrier.picture.fill_100x100

</th>
<td>

100×100 Pixel

</td>
    </tr>
    <tr>
<th align="left">

carrier.picture.original

</th>
<td>

Maximum sized image. This is the original image with default-cropping or user-cropping applied.

</td>
    </tr>
</table>

## Response Example

```json
{
  "total_entries": 284,
  "offset": 0,
  "total_pages": 95,
  "current_page": 1,
  "per_page": 3,
  "data": [
    {
      "id": 72206,
      "created_at": "2019-08-17T09:01:36+02:00",
      "updated_at": "2021-05-05T21:01:08+02:00",
      "latitude": 51.1856375,
      "longitude": 10.42078160000006,
      "title": "Tiere auf Lebenshof Gut Weidensee benötigen dringend Hilfe!",
      "type": "Project",
      "contact": {
        "id": 576646,
        "name": "Emma Wunderlich (display)",
        "picture": {
          "links": [
            {
              "rel": "fill_100x100",
              "href": "https://betterplace-assets.betterplace.org/uploads/user/profile_picture/000/576/646/fill_100x100_bp1584600717_Videoprint_37.jpg"
            },
            {
              "rel": "original",
              "href": "https://betterplace-assets.betterplace.org/uploads/user/profile_picture/000/576/646/crop_original_bp1584600717_Videoprint_37.jpg"
            }
          ]
        },
        "links": [
          {
            "rel": "platform",
            "href": "https://www.betterplace.org/de/users/576646"
          },
          {
            "rel": "contact_data",
            "href": "https://api.betterplace.org/de/api_v4/users/576646/contact_data.json"
          }
        ]
      },
      "progress_percentage": 86,
      "profile_picture": {
        "links": [
          {
            "rel": "fill_960x500",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/072/206/fill_960x500_bp1614871942_7.jpg"
          },
          {
            "rel": "fill_730x380",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/072/206/fill_730x380_bp1614871942_7.jpg"
          },
          {
            "rel": "fill_618x322",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/072/206/fill_618x322_bp1614871942_7.jpg"
          },
          {
            "rel": "fill_410x214",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/072/206/fill_410x214_bp1614871942_7.jpg"
          },
          {
            "rel": "fill_270x141",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/072/206/fill_270x141_bp1614871942_7.jpg"
          },
          {
            "rel": "original",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/072/206/crop_original_bp1614871942_7.jpg"
          }
        ]
      },
      "donated_amount_in_cents": 25549100,
      "country": "Deutschland",
      "city": "Mühlhausen",
      "carrier": {
        "id": 38291,
        "name": "Lebenshof Gut Weidensee",
        "city": "Mühlhausen",
        "picture": {
          "links": [
            {
              "rel": "fill_100x100",
              "href": "https://betterplace-assets.betterplace.org/uploads/organisation/profile_picture/000/038/291/fill_100x100_bp1566147543_index.png"
            },
            {
              "rel": "original",
              "href": "https://betterplace-assets.betterplace.org/uploads/organisation/profile_picture/000/038/291/crop_original_bp1566147543_index.png"
            }
          ]
        },
        "links": [
          {
            "rel": "self",
            "href": "https://api.betterplace.org/de/api_v4/organisations/38291.json"
          }
        ]
      },
      "donations_count": 6853,
      "open_amount_in_cents": 4101300,
      "links": [
        {
          "rel": "platform",
          "href": "https://www.betterplace.org/de/projects/72206-tiere-auf-lebenshof-gut-weidensee-benoetigen-dringend-hilfe"
        },
        {
          "rel": "self",
          "href": "https://api.betterplace.org/de/api_v4/projects/72206.json"
        },
        {
          "rel": "pictures",
          "href": "https://api.betterplace.org/de/api_v4/projects/72206/pictures.json"
        }
      ]
    },
    {
      "id": 51106,
      "created_at": "2016-12-16T14:54:22+01:00",
      "updated_at": "2021-05-05T00:08:07+02:00",
      "latitude": 47.92151,
      "longitude": 7.72327999999993,
      "title": "Förderverein Animal Hope and Wellness e.V.",
      "type": "Project",
      "contact": {
        "id": 508439,
        "name": "Charleen Aydın (display)",
        "picture": {
          "links": [
            {
              "rel": "fill_100x100",
              "href": "https://betterplace-assets.betterplace.org/uploads/user/profile_picture/000/508/439/fill_100x100_bp1604688857_IMG_2320.JPG"
            },
            {
              "rel": "original",
              "href": "https://betterplace-assets.betterplace.org/uploads/user/profile_picture/000/508/439/crop_original_bp1604688857_IMG_2320.JPG"
            }
          ]
        },
        "links": [
          {
            "rel": "platform",
            "href": "https://www.betterplace.org/de/users/508439"
          },
          {
            "rel": "contact_data",
            "href": "https://api.betterplace.org/de/api_v4/users/508439/contact_data.json"
          }
        ]
      },
      "progress_percentage": 93,
      "profile_picture": {
        "links": [
          {
            "rel": "fill_960x500",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/051/106/fill_960x500_bp1584552985_IMG_0631.JPG"
          },
          {
            "rel": "fill_730x380",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/051/106/fill_730x380_bp1584552985_IMG_0631.JPG"
          },
          {
            "rel": "fill_618x322",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/051/106/fill_618x322_bp1584552985_IMG_0631.JPG"
          },
          {
            "rel": "fill_410x214",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/051/106/fill_410x214_bp1584552985_IMG_0631.JPG"
          },
          {
            "rel": "fill_270x141",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/051/106/fill_270x141_bp1584552985_IMG_0631.JPG"
          },
          {
            "rel": "original",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/051/106/crop_original_bp1584552985_IMG_0631.JPG"
          }
        ]
      },
      "donated_amount_in_cents": 22880025,
      "country": "Deutschland",
      "city": "Ehrenkirchen",
      "carrier": {
        "id": 30392,
        "name": "Förderverein Animal Hope and Wellness e.V.",
        "city": "Ehrenkirchen",
        "picture": {
          "links": [
            {
              "rel": "fill_100x100",
              "href": "https://betterplace-assets.betterplace.org/uploads/organisation/profile_picture/000/030/392/fill_100x100_bp1526465549_Logo_FV_AH_W_web.jpg"
            },
            {
              "rel": "original",
              "href": "https://betterplace-assets.betterplace.org/uploads/organisation/profile_picture/000/030/392/crop_original_bp1526465549_Logo_FV_AH_W_web.jpg"
            }
          ]
        },
        "links": [
          {
            "rel": "self",
            "href": "https://api.betterplace.org/de/api_v4/organisations/30392.json"
          }
        ]
      },
      "donations_count": 12831,
      "open_amount_in_cents": 1547875,
      "links": [
        {
          "rel": "platform",
          "href": "https://www.betterplace.org/de/projects/51106-foerderverein-animal-hope-and-wellness-e-v"
        },
        {
          "rel": "self",
          "href": "https://api.betterplace.org/de/api_v4/projects/51106.json"
        },
        {
          "rel": "pictures",
          "href": "https://api.betterplace.org/de/api_v4/projects/51106/pictures.json"
        }
      ]
    },
    {
      "id": 94118,
      "created_at": "2021-04-26T13:28:40+02:00",
      "updated_at": "2021-05-05T00:21:38+02:00",
      "latitude": 41.0863854,
      "longitude": 23.5483819,
      "title": "Eine Reise ins Glück - Hilfst Du mir?!",
      "type": "Project",
      "contact": {
        "id": 487590,
        "name": "Tizian Bergmann (display)",
        "picture": {
          "links": [
            {
              "rel": "fill_100x100",
              "href": "https://betterplace-assets.betterplace.org/uploads/user/profile_picture/000/487/590/fill_100x100_bp1584583828_received_243203176096404.jpeg"
            },
            {
              "rel": "original",
              "href": "https://betterplace-assets.betterplace.org/uploads/user/profile_picture/000/487/590/crop_original_bp1584583828_received_243203176096404.jpeg"
            }
          ]
        },
        "links": [
          {
            "rel": "platform",
            "href": "https://www.betterplace.org/de/users/487590"
          },
          {
            "rel": "contact_data",
            "href": "https://api.betterplace.org/de/api_v4/users/487590/contact_data.json"
          }
        ]
      },
      "progress_percentage": 101,
      "profile_picture": {
        "links": [
          {
            "rel": "fill_960x500",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/094/118/fill_960x500_bp1619436753_20170926_115948.jpg"
          },
          {
            "rel": "fill_730x380",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/094/118/fill_730x380_bp1619436753_20170926_115948.jpg"
          },
          {
            "rel": "fill_618x322",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/094/118/fill_618x322_bp1619436753_20170926_115948.jpg"
          },
          {
            "rel": "fill_410x214",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/094/118/fill_410x214_bp1619436753_20170926_115948.jpg"
          },
          {
            "rel": "fill_270x141",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/094/118/fill_270x141_bp1619436753_20170926_115948.jpg"
          },
          {
            "rel": "original",
            "href": "https://betterplace-assets.betterplace.org/uploads/project/profile_picture/000/094/118/crop_original_bp1619436753_20170926_115948.jpg"
          }
        ]
      },
      "donated_amount_in_cents": 183060,
      "country": "Griechenland",
      "city": "Serres",
      "carrier": {
        "id": 25023,
        "name": "Hundegarten Serres e.V.",
        "city": "Euskirchen",
        "picture": {
          "links": [
            {
              "rel": "fill_100x100",
              "href": "https://betterplace-assets.betterplace.org/uploads/organisation/profile_picture/000/025/023/fill_100x100_Logo_Original.png"
            },
            {
              "rel": "original",
              "href": "https://betterplace-assets.betterplace.org/uploads/organisation/profile_picture/000/025/023/crop_original_Logo_Original.png"
            }
          ]
        },
        "links": [
          {
            "rel": "self",
            "href": "https://api.betterplace.org/de/api_v4/organisations/25023.json"
          }
        ]
      },
      "donations_count": 103,
      "open_amount_in_cents": 0,
      "links": [
        {
          "rel": "platform",
          "href": "https://www.betterplace.org/de/projects/94118-eine-reise-ins-glueck-hilfst-du-mir"
        },
        {
          "rel": "self",
          "href": "https://api.betterplace.org/de/api_v4/projects/94118.json"
        },
        {
          "rel": "pictures",
          "href": "https://api.betterplace.org/de/api_v4/projects/94118/pictures.json"
        }
      ]
    }
  ]
}
```

