
# Volunteering Details ⇄ [List](volunteering_list.md)

```Cirru
GET https://api.betterplace.org/de/api_v4/volunteering/78483.json
```

The details of a betterplace.org volunteering offer (donate time).

**For [betterplace.org clients](../README.md#client-api):**
This resource is not available at the moment.


## URL Parameters

<table>
  <tr>
    <th>Parameter</th>
    <th>Example</th>
    <th>Required</th>
    <th>Description</th>
  </tr>
  <tr>
    <th align="left">id</th>
    <td><code>78483</code></td>
    <td>yes</td>
<td>

Volunteering-id as an integer number ≥ 1.

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
      <th align="left">street</th>
      <td><code>null &#124; string</code></td>
      <td><code>"Schlesische Straße 26"</code></td>
<td>

Street address

</td>
    </tr>
    <tr>
      <th align="left">zip</th>
      <td><code>null &#124; string</code></td>
      <td><code>"10997"</code></td>
<td>

ZIP code

</td>
    </tr>
    <tr>
      <th align="left">city</th>
      <td><code>null &#124; string</code></td>
      <td><code>"Berlin"</code></td>
<td>

Name of the city

</td>
    </tr>
    <tr>
      <th align="left">country</th>
      <td><code>null &#124; string</code></td>
      <td><code>"Deutschland"</code></td>
<td>

Name of the country

</td>
    </tr>
    <tr>
      <th align="left">content_updated_at</th>
      <td><code>string</code></td>
      <td><code>"1994-11-05T13:15:30Z"</code></td>
<td>

DateTime (ISO8601 with Timezone)

</td>
    </tr>
    <tr>
      <th align="left">title</th>
      <td><code>string</code></td>
      <td><code>TODO</code></td>
<td>

Max 100 character

</td>
    </tr>
    <tr>
      <th align="left">description</th>
      <td><code>string</code></td>
      <td><code></code></td>
<td>

A description of the offer. This may contain any of the following
HTML tags: ```a, b, br, div, em, i, iframe, img, li, ol, p, strong, ul```.


</td>
    </tr>
    <tr>
        <th align="left" style="white-space: nowrap">
          <a id="carrier-ref" href="#carrier">
            ↓carrier
          </a>
        </th>
      <td><code>object</code></td>
      <td><code>TODO</code></td>
<td>

The organisation that carrier this volunteering

</td>
    </tr>
    <tr>
      <th align="left">vacancies</th>
      <td><code>number</code></td>
      <td><code>1</code></td>
<td>

The number of volunteers that are needed, provided by the manager

</td>
    </tr>
    <tr>
        <th align="left" style="white-space: nowrap">
          <a id="image-ref" href="#image">
            ↓image
          </a>
        </th>
      <td><code>null &#124; object</code></td>
      <td><code>TODO</code></td>
<td>

Each volunteering has one optional image / DEPRECATED, will be removed after 5/2015

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

Contact person, contact data and contact address

</td>
    </tr>
    <tr>
      <th align="left">location_fixed</th>
      <td><code>boolean</code></td>
      <td><code>true</code></td>
<td>

Specifies whether the volunteering offer is limited to a certain location or if it may be
executed remotely.


</td>
    </tr>
    <tr>
      <th align="left">working_time_selection</th>
      <td><code>string</code></td>
      <td><code>regular commitment</code></td>
<td>

Working time selection, specifies if this is a one-time event or if
this volunteering can takes place regulary.


</td>
    </tr>
    <tr>
      <th align="left">working_time_weekends</th>
      <td><code>array</code></td>
      <td><code>["in the mornings"]</code></td>
<td>

Up to three working time preferences. They specify when this volunteering
should take place on weekends.


</td>
    </tr>
    <tr>
      <th align="left">working_time_weekdays</th>
      <td><code>array</code></td>
      <td><code>["in the mornings"]</code></td>
<td>

Up to three working time preferences. They specify when this volunteering
should take place on weekdays.


</td>
    </tr>
    <tr>
      <th align="left">begins_at</th>
      <td><code>string</code></td>
      <td><code>"1994-11-05T13:15:30Z"</code></td>
<td>

DateTime (ISO8601 with Timezone)

</td>
    </tr>
    <tr>
      <th align="left">ends_at</th>
      <td><code>string</code></td>
      <td><code>"1994-11-05T13:15:30Z"</code></td>
<td>

DateTime (ISO8601 with Timezone)

</td>
    </tr>
    <tr>
      <th align="left">topics</th>
      <td><code>array</code></td>
      <td><code>["Development cooperation", "Children & youth"]</code></td>
<td>

Up to 4 categories that describe, what for which causes you need volunteers.
Results are translated to the requested language.
Possible results: "Animal & environment protection", "Culture & sports",
"Children & youth", "Development cooperation ", "DisabledEducation", "Elderly people",
"Human rights", "Refugees & immigrants", "Invalid", "Local help", "Socially deprived"


</td>
    </tr>
    <tr>
      <th align="left">activities</th>
      <td><code>array &#124; null</code></td>
      <td><code>["consulting/coaching", "office work"]</code></td>
<td>

Up to 4 categories that describe, what for which causes you need volunteers.
Results are translated to the requested language.
Possible results: "consulting/coaching", "crafting/gardening", "doing sports",
"doing the chores", "group care", "nursing/parenting", "office work",
"organising/managing", "painting/designing", "tutoring/reading",
"visiting/accompanying", "writing/translating"


</td>
    </tr>
    <tr>
      <th align="left">imported_from</th>
      <td><code>null &#124; string</code></td>
      <td><code>somewhere</code></td>
<td>

Where Betterplace imports volunteering from.

</td>
    </tr>
    <tr>
      <th align="left">import_information</th>
      <td><code></code></td>
      <td><code>TODO</code></td>
<td>

Meta data concerning the import of this volunteering offer, if it
was indeed imported.


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
      <th align="left">carrier.latitude</th>
      <td><code>number</code></td>
      <td><code>52.499007</code></td>
<td>

Decimal degrees based on user input

</td>
    </tr>
    <tr>
      <th align="left">carrier.longitude</th>
      <td><code>number</code></td>
      <td><code>13.44947</code></td>
<td>

Decimal degrees based on user input

</td>
    </tr>
    <tr>
      <th align="left">carrier.name</th>
      <td><code>string</code></td>
      <td><code>"Viva con Agua de Sankt Pauli e.V."</code></td>
<td>

An organisation name, Users will be added later

</td>
    </tr>
    <tr>
      <th align="left">carrier.street</th>
      <td><code>string</code></td>
      <td><code>"Rosenstr. 3"</code></td>
<td>

Contact data for the organisation

</td>
    </tr>
    <tr>
      <th align="left">carrier.city</th>
      <td><code>string</code></td>
      <td><code>"Berlin"</code></td>
<td>

Contact data for the organisation

</td>
    </tr>
    <tr>
      <th align="left">carrier.zip</th>
      <td><code>string</code></td>
      <td><code>"10123"</code></td>
<td>

Contact data for the organisation

</td>
    </tr>
    <tr>
      <th align="left">carrier.country</th>
      <td><code>string</code></td>
      <td><code>"Germany"</code></td>
<td>

Contact data for the organisation

</td>
    </tr>
    <tr>
        <th align="left" style="white-space: nowrap">
          <a id="carrier.picture-ref" href="#carrier.picture">
            ↓carrier.picture
          </a>
        </th>
      <td><code>null &#124; object</code></td>
      <td><code></code></td>
<td>

TODO

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

### <a id="image" href="#image-ref">↑Nested Attributes: image</a>

  <table>
    <tr>
      <th>Attribute</th>
      <th>Types</th>
      <th>Example</th>
      <th>Description</th>
    </tr>
    <tr>
      <th align="left">image.description</th>
      <td><code>string</code></td>
      <td><code></code></td>
<td>

Image description

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
      <th align="left">contact.name</th>
      <td><code>string</code></td>
      <td><code>Till Behnke</code></td>
<td>

Fullname of the contact person.


</td>
    </tr>
    <tr>
      <th align="left">contact.phone</th>
      <td><code>string</code></td>
      <td><code>030 - 7676 4488 44</code></td>
<td>

Phone number for direct contact.
No validations on input apply.


</td>
    </tr>
    <tr>
      <th align="left">contact.email</th>
      <td><code>string</code></td>
      <td><code>support@betterplace.org</code></td>
<td>

Plain text email-address for direct contact


</td>
    </tr>
    <tr>
        <th align="left" style="white-space: nowrap">
          <a id="contact.picture-ref" href="#contact.picture">
            ↓contact.picture
          </a>
        </th>
      <td><code>object</code></td>
      <td><code>https://betterplace-assets.betterplace.org/…</code></td>
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
</table>

## Response Links

<table>
  <tr>
    <th>Linkname</th>
    <th>Description</th>
  </tr>
    <tr>
<th align="left">

self

</th>
<td>

Link to this resource itself
(<a href="volunteering_details.md">volunteering details</a>)


</td>
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

inquiries

</th>
<td>

The URL to which inquiries about this offer can be POSTed
(<a href="volunteering_inquiries.md">inquiry details</a>).
Templated, needs insertion of the client_id.


</td>
    </tr>
    <tr>
<th align="left">

carrier.self

</th>
<td>

Link to this resource itself
(<a href="organisation_details.md">organisation details</a>)


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

carrier.picture.fill_200x200

</th>
<td>

200×200 Pixel

</td>
    </tr>
    <tr>
<th align="left">

carrier.picture.fill_400x400

</th>
<td>

400×400 Pixel

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
    <tr>
<th align="left">

image.fill_618x322

</th>
<td>

618×322 Pixel / DEPRECATED, will be removed after 5/2015

</td>
    </tr>
    <tr>
<th align="left">

image.fill_270x141

</th>
<td>

270×141 Pixel / DEPRECATED, will be removed after 5/2015

</td>
    </tr>
    <tr>
<th align="left">

image.original

</th>
<td>

Original size / DEPRECATED, will be removed after 5/2015

</td>
    </tr>
    <tr>
<th align="left">

image.thumb

</th>
<td>

Thumbnail size / DEPRECATED, will be removed after 5/2015

</td>
    </tr>
    <tr>
<th align="left">

image.medium

</th>
<td>

Medium size / DEPRECATED, will be removed after 5/2015

</td>
    </tr>
    <tr>
<th align="left">

image.regular

</th>
<td>

Regular size / DEPRECATED, will be removed after 5/2015

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
</table>

## Response Example

```json
{
  "id": 78483,
  "created_at": "2021-05-07T22:14:13+02:00",
  "updated_at": "2021-05-07T22:14:13+02:00",
  "latitude": 52.49847530000001,
  "longitude": 13.4486537,
  "street": null,
  "zip": null,
  "city": null,
  "country": null,
  "content_updated_at": "2021-05-07T22:14:13+02:00",
  "title": "Test 3",
  "description": "geht geht",
  "carrier": {
    "latitude": 52.49847530000001,
    "longitude": 13.4486537,
    "name": "betterplace.org (gut.org gAG)",
    "street": "Eschenweg 76",
    "city": "Berlin",
    "zip": "10997",
    "country": "Deutschland",
    "picture": {
      "links": [
        {
          "rel": "fill_100x100",
          "href": "https://betterplace-assets.betterplace.org/uploads/organisation/profile_picture/000/013/865/fill_100x100_bp1529503770_Logo-betterplace.png"
        },
        {
          "rel": "fill_200x200",
          "href": "https://betterplace-assets.betterplace.org/uploads/organisation/profile_picture/000/013/865/fill_200x200_bp1529503770_Logo-betterplace.png"
        },
        {
          "rel": "fill_400x400",
          "href": "https://betterplace-assets.betterplace.org/uploads/organisation/profile_picture/000/013/865/fill_400x400_bp1529503770_Logo-betterplace.png"
        },
        {
          "rel": "original",
          "href": "https://betterplace-assets.betterplace.org/uploads/organisation/profile_picture/000/013/865/crop_original_bp1529503770_Logo-betterplace.png"
        }
      ]
    },
    "links": [
      {
        "rel": "self",
        "href": "https://api.betterplace.org/de/api_v4/organisations/13865.json"
      }
    ]
  },
  "vacancies": 1,
  "image": {
    "description": "",
    "links": [
      {
        "rel": "fill_618x322",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/fill_618x322_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      },
      {
        "rel": "fill_270x141",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/fill_270x141_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      },
      {
        "rel": "original",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      },
      {
        "rel": "thumb",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/thumb_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      },
      {
        "rel": "medium",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/medium_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      },
      {
        "rel": "regular",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/regular_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      }
    ]
  },
  "contact": {
    "name": "Amar Maier",
    "phone": "",
    "email": "tjo@betterplace.org",
    "picture": {
      "links": [
        {
          "rel": "fill_100x100",
          "href": "https://betterplace-assets.betterplace.org/uploads/user/profile_picture/000/021/312/fill_100x100_bp1584570872_image-4.jpg"
        },
        {
          "rel": "original",
          "href": "https://betterplace-assets.betterplace.org/uploads/user/profile_picture/000/021/312/crop_original_bp1584570872_image-4.jpg"
        }
      ]
    },
    "links": [

    ]
  },
  "location_fixed": false,
  "working_time_selection": "egal wann / nach Vereinbarung",
  "working_time_weekends": [

  ],
  "working_time_weekdays": [

  ],
  "begins_at": null,
  "ends_at": null,
  "topics": [
    "Sozial Benachteiligte"
  ],
  "activities": [
    "beraten/coachen"
  ],
  "imported_from": null,
  "import_information": null,
  "profile_picture": {
    "links": [
      {
        "rel": "fill_960x500",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/fill_960x500_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      },
      {
        "rel": "fill_730x380",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/fill_730x380_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      },
      {
        "rel": "fill_618x322",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/fill_618x322_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      },
      {
        "rel": "fill_410x214",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/fill_410x214_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      },
      {
        "rel": "fill_270x141",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/fill_270x141_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      },
      {
        "rel": "original",
        "href": "https://betterplace-assets.betterplace.org/uploads/bettertime/job_description/profile_picture/000/078/483/crop_original_bp1620418453_Bildschirmfoto_2021-05-05_um_12.57.45.png"
      }
    ]
  },
  "links": [
    {
      "rel": "self",
      "href": "https://api.betterplace.org/de/api_v4/volunteering/78483.json"
    },
    {
      "rel": "platform",
      "href": "https://www.betterplace.org/de/volunteering/78483-test-3"
    },
    {
      "rel": "inquiries",
      "href": "https://api.betterplace.org/de/api_v4/clients/%7Bclient_id%7D/volunteering/78483-test-3/inquiries.json",
      "templated": true
    }
  ]
}
```

