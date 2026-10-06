# Reference
## Marketplace
<details><summary><code>client.marketplace.<a href="src/marketsdk/marketplace/client.py">get_marketplace</a>() -> MarketplaceObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Settings are changed in the dashboard, separately for test and live.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.marketplace.get_marketplace()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Sellers
<details><summary><code>client.sellers.<a href="src/marketsdk/sellers/client.py">list_sellers</a>(...) -> SellerList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.sellers.list_sellers()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**external_id:** `typing.Optional[str]` — Find the seller with this external id.
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[ListSellersRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="src/marketsdk/sellers/client.py">create_seller</a>(...) -> SellerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.sellers.create_seller(
    external_id="external_id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `CreatePartyDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="src/marketsdk/sellers/client.py">get_seller</a>(...) -> SellerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.sellers.get_seller(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="src/marketsdk/sellers/client.py">erase_seller</a>(...) -> SellerObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Removes the name, external id, metadata, storefront, and review text, and takes the listings down. Orders and reputation stay, without personal data.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.sellers.erase_seller(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="src/marketsdk/sellers/client.py">update_seller</a>(...) -> SellerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.sellers.update_seller(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `UpdatePartyDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="src/marketsdk/sellers/client.py">put_storefront</a>(...) -> StorefrontObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.sellers.put_storefront(
    id="id",
    name="name",
    slug="jane-templates",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**slug:** `str` — Lowercase letters, digits, and hyphens. Unique per marketplace.
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**metadata:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="src/marketsdk/sellers/client.py">create_onboarding_link</a>(...) -> OnboardingLinkObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

The first link creates the seller's connected account on your Stripe account: Express, with Stripe collecting what the law requires, your platform paying Stripe's fees and bearing losses, and only transfers requested. Send the seller to the link; their payouts status follows as Stripe reports it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.sellers.create_onboarding_link(
    id="id",
    return_url="return_url",
    refresh_url="refresh_url",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**return_url:** `str` — Where Stripe sends the seller when they finish or leave onboarding.
    
</dd>
</dl>

<dl>
<dd>

**refresh_url:** `str` — Where Stripe sends the seller if the link expired. Create a new link there.
    
</dd>
</dl>

<dl>
<dd>

**country:** `typing.Optional[str]` — The seller's country, two letters. Used only when the seller's Stripe account is created, on the first link. Defaults to your Stripe account's country.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.sellers.<a href="src/marketsdk/sellers/client.py">get_seller_profile</a>(...) -> SellerProfileObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Callable with a publishable key. Shows only what a buyer may see.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.sellers.get_seller_profile(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Buyers
<details><summary><code>client.buyers.<a href="src/marketsdk/buyers/client.py">list_buyers</a>(...) -> BuyerList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.buyers.list_buyers()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**external_id:** `typing.Optional[str]` — Find the buyer with this external id.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.buyers.<a href="src/marketsdk/buyers/client.py">create_buyer</a>(...) -> BuyerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.buyers.create_buyer(
    external_id="external_id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `CreatePartyDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.buyers.<a href="src/marketsdk/buyers/client.py">get_buyer</a>(...) -> BuyerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.buyers.get_buyer(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.buyers.<a href="src/marketsdk/buyers/client.py">erase_buyer</a>(...) -> BuyerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.buyers.erase_buyer(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.buyers.<a href="src/marketsdk/buyers/client.py">update_buyer</a>(...) -> BuyerObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.buyers.update_buyer(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `UpdatePartyDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Categories
<details><summary><code>client.categories.<a href="src/marketsdk/categories/client.py">list_categories</a>(...) -> CategoryList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.categories.list_categories()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.categories.<a href="src/marketsdk/categories/client.py">create_category</a>(...) -> CategoryObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.categories.create_category(
    key="ui-kits",
    name="name",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**key:** `str` — Your key for the category. Unique per marketplace.
    
</dd>
</dl>

<dl>
<dd>

**name:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**parent:** `typing.Optional[str]` — Another category of this marketplace.
    
</dd>
</dl>

<dl>
<dd>

**attribute_schema:** `typing.Optional[AttributeSchemaObject]` 
    
</dd>
</dl>

<dl>
<dd>

**fee:** `typing.Optional[CategoryFeeDto]` — Overrides the marketplace's platform fee for listings in this category. Null uses the marketplace fee.
    
</dd>
</dl>

<dl>
<dd>

**prohibited:** `typing.Optional[bool]` — Listings in a prohibited category cannot be published (section 9.4).
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.categories.<a href="src/marketsdk/categories/client.py">get_category</a>(...) -> CategoryObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.categories.get_category(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.categories.<a href="src/marketsdk/categories/client.py">update_category</a>(...) -> CategoryObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.categories.update_category(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**name:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**parent:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**fee:** `typing.Optional[CategoryFeeDto]` 
    
</dd>
</dl>

<dl>
<dd>

**prohibited:** `typing.Optional[bool]` — Listings in a prohibited category cannot be published. Listings already published stay until moderated.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.categories.<a href="src/marketsdk/categories/client.py">get_attribute_schema</a>(...) -> AttributeSchemaObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.categories.get_attribute_schema(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.categories.<a href="src/marketsdk/categories/client.py">put_attribute_schema</a>(...) -> AttributeSchemaObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Refused if a listing already in the category would no longer fit.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK, AttributeDefinitionObject
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.categories.put_attribute_schema(
    id="id",
    attributes=[
        AttributeDefinitionObject(
            key="format",
            type="string",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `AttributeSchemaObject` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Listings
<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">list_listings</a>(...) -> ListingList</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

With a publishable key, only published listings are listed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.list_listings()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**seller:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**category:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[ListListingsRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">create_listing</a>(...) -> ListingObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK, MoneyDto
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.create_listing(
    seller="sel_034XtPDs7UJ0TXzTsdaHZa",
    title="title",
    price=MoneyDto(
        amount=4900,
        currency="USD",
    ),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `CreateListingDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">create_listings</a>(...) -> BulkListingsObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK, CreateListingDto, MoneyDto
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.create_listings(
    listings=[
        CreateListingDto(
            seller="sel_034XtPDs7UJ0TXzTsdaHZa",
            title="title",
            price=MoneyDto(
                amount=4900,
                currency="USD",
            ),
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**listings:** `typing.List[CreateListingDto]` — All are created, or none.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">get_listing</a>(...) -> ListingObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

With a publishable key, only a published listing can be retrieved.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.get_listing(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">update_listing</a>(...) -> ListingObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.update_listing(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**category:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**title:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**price:** `typing.Optional[MoneyDto]` 
    
</dd>
</dl>

<dl>
<dd>

**quantity:** `typing.Optional[float]` — The total. Cannot go below what open orders have reserved.
    
</dd>
</dl>

<dl>
<dd>

**attributes:** `typing.Optional[typing.Dict[str, typing.Any]]` 
    
</dd>
</dl>

<dl>
<dd>

**metadata:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**expires_at:** `typing.Optional[datetime.datetime]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">publish_listing</a>(...) -> ListingObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Needs an active seller, verified when seller verification is on, and a category that is not prohibited.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.publish_listing(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">unpublish_listing</a>(...) -> ListingObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.unpublish_listing(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">remove_listing</a>(...) -> ListingObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.remove_listing(
    id="id",
    reason="reason",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**reason:** `str` — Recorded with the removal.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">list_media</a>(...) -> MediaList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.list_media(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">create_media</a>(...) -> MediaUploadObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns a signed URL, valid for 10 minutes. PUT the file there, then complete the upload. The file is stored under a path that begins with the marketplace id.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.create_media(
    id="id",
    content_type="image/jpeg",
    size_bytes=1.1,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**content_type:** `CreateMediaDtoContentType` 
    
</dd>
</dl>

<dl>
<dd>

**size_bytes:** `float` — The exact size of the file, in bytes. At most 10 MB.
    
</dd>
</dl>

<dl>
<dd>

**position:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">complete_media</a>(...) -> MediaObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Checks the stored file against the declared type and size.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.complete_media(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.listings.<a href="src/marketsdk/listings/client.py">delete_media</a>(...) -> MediaObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.listings.delete_media(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Search
<details><summary><code>client.search.<a href="src/marketsdk/search/client.py">search_listings</a>(...) -> ListingList</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Full text over title and description, with filters and sorting. Only published listings with something available are returned. Callable with a publishable key.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.search.search_listings()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**q:** `typing.Optional[str]` — Full text over title and description.
    
</dd>
</dl>

<dl>
<dd>

**category:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**seller:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**min_price:** `typing.Optional[float]` — Minor units.
    
</dd>
</dl>

<dl>
<dd>

**max_price:** `typing.Optional[float]` — Minor units.
    
</dd>
</dl>

<dl>
<dd>

**attributes:** `typing.Optional[typing.Dict[str, typing.Any]]` — Attribute filters, as attributes[key]=value for equality, or attributes[key][gte]=n and attributes[key][lte]=n for numbers. Numeric filters need a category.
    
</dd>
</dl>

<dl>
<dd>

**sort:** `typing.Optional[SearchListingsSearchRequestSort]` — Relevance needs q. Default newest.
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**cursor:** `typing.Optional[str]` — The next_cursor of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Orders
<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">list_orders</a>(...) -> OrderList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.list_orders()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**buyer:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**seller:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**listing:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**state:** `typing.Optional[ListOrdersRequestState]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">create_order</a>(...) -> OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

The buyer commits to buy. Quantity is reserved at once. With payments off the order is committed; with payments on it awaits payment.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.create_order(
    listing="lst_034XtPDs7UJ0TXzTsdaHZa",
    buyer="buy_034XtPDs7UJ0TXzTsdaHZa",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**listing:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**buyer:** `str` — The buyer placing the order. The actor for this transition.
    
</dd>
</dl>

<dl>
<dd>

**quantity:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**checkout:** `typing.Optional[CheckoutUrlsDto]` — Payments on only. With these, the order's payment includes a Stripe-hosted checkout URL; without them, a client secret for Stripe Elements on your own page.
    
</dd>
</dl>

<dl>
<dd>

**metadata:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">get_order</a>(...) -> OrderObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.get_order(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">list_order_events</a>(...) -> OrderEventList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.list_order_events(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">claim_order</a>(...) -> OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.claim_order(
    id="id",
    actor="buy_034XtPDs7UJ0TXzTsdaHZa",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ActorDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">confirm_order</a>(...) -> OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.confirm_order(
    id="id",
    actor="buy_034XtPDs7UJ0TXzTsdaHZa",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ActorDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">back_out_of_order</a>(...) -> OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition. Writes a backed_out reputation event against the actor.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.back_out_of_order(
    id="id",
    actor="buy_034XtPDs7UJ0TXzTsdaHZa",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ActorDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">propose_cancel</a>(...) -> OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition. The other party can accept within the agreement window. A declined or lapsed proposal changes nothing.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.propose_cancel(
    id="id",
    actor="buy_034XtPDs7UJ0TXzTsdaHZa",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ActorDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">accept_cancel</a>(...) -> OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.accept_cancel(
    id="id",
    actor="buy_034XtPDs7UJ0TXzTsdaHZa",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ActorDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">decline_cancel</a>(...) -> OrderObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.decline_cancel(
    id="id",
    actor="buy_034XtPDs7UJ0TXzTsdaHZa",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ActorDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">list_order_reviews</a>(...) -> ReviewList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.list_order_reviews(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.orders.<a href="src/marketsdk/orders/client.py">create_review</a>(...) -> ReviewObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Called from your server. `actor` says which end user is acting; we check they are a party to the order and may make this transition. Only on a completed order, inside the review window, once per party. Hidden until both have reviewed or the window closes.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.orders.create_review(
    id="id",
    actor="buy_034XtPDs7UJ0TXzTsdaHZa",
    rating=1.1,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**actor:** `str` — The buyer id or seller id of the end user doing this. We check they are a party to the order and may make this transition.
    
</dd>
</dl>

<dl>
<dd>

**rating:** `float` 
    
</dd>
</dl>

<dl>
<dd>

**body:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Reviews
<details><summary><code>client.reviews.<a href="src/marketsdk/reviews/client.py">list_reviews</a>(...) -> ReviewList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.reviews.list_reviews(
    subject="subject",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**subject:** `str` — The buyer or seller the reviews are about.
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reviews.<a href="src/marketsdk/reviews/client.py">get_review</a>(...) -> ReviewObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.reviews.get_review(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Reputation
<details><summary><code>client.reputation.<a href="src/marketsdk/reputation/client.py">list_reputation_events</a>(...) -> ReputationEventList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.reputation.list_reputation_events(
    party="party",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**party:** `str` — The buyer or seller whose events to list.
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.reputation.<a href="src/marketsdk/reputation/client.py">void_reputation_event</a>(...) -> ReputationEventObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

For the customer's team. Writes a second event pointing at the first. The voided event stops counting. Nothing is deleted.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.reputation.void_reputation_event(
    id="id",
    reason="reason",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**reason:** `str` — Why the event is voided. Recorded on the voiding event.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Payments
<details><summary><code>client.payments.<a href="src/marketsdk/payments/client.py">list_payments</a>(...) -> PaymentList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.payments.list_payments()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**order:** `typing.Optional[str]` — Only the payment for this order.
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[ListPaymentsRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="src/marketsdk/payments/client.py">get_payment</a>(...) -> PaymentObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.payments.get_payment(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="src/marketsdk/payments/client.py">update_payment</a>(...) -> PaymentObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.payments.update_payment(
    id="id",
    metadata={
        "key": "value"
    },
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `UpdateMetadataDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="src/marketsdk/payments/client.py">retry_payment_release</a>(...) -> PaymentObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

For a release that failed, for example because the seller could not yet receive transfers. A release is also tried again by itself when the seller becomes able to receive payouts.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.payments.retry_payment_release(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="src/marketsdk/payments/client.py">list_refunds</a>(...) -> RefundList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.payments.list_refunds()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**payment:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**order:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="src/marketsdk/payments/client.py">create_refund</a>(...) -> RefundObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Recorded at once with status `pending`, then made at Stripe. If the seller's share was already released, the transfer is reversed in the same proportion, so your fee is given back in proportion too.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.payments.create_refund()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**payment:** `typing.Optional[str]` — The payment to refund. Give this or `order`.
    
</dd>
</dl>

<dl>
<dd>

**order:** `typing.Optional[str]` — The order whose payment to refund. Give this or `payment`.
    
</dd>
</dl>

<dl>
<dd>

**amount:** `typing.Optional[float]` — Minor units. Defaults to everything not yet refunded.
    
</dd>
</dl>

<dl>
<dd>

**reason:** `typing.Optional[CreateRefundDtoReason]` 
    
</dd>
</dl>

<dl>
<dd>

**metadata:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="src/marketsdk/payments/client.py">get_refund</a>(...) -> RefundObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.payments.get_refund(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="src/marketsdk/payments/client.py">update_refund</a>(...) -> RefundObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.payments.update_refund(
    id="id",
    metadata={
        "key": "value"
    },
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `UpdateMetadataDto` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Trust
<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">create_verification</a>(...) -> VerificationObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a Stripe Identity session on your Stripe account and returns its page, once. Only the outcome and the session id are kept; no document image or document data. When seller verification is on, a seller can publish only once verified.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.create_verification(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**return_url:** `typing.Optional[str]` — Where Stripe sends the seller after the verification page.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">list_verifications</a>(...) -> VerificationList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.list_verifications()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**seller:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">get_verification</a>(...) -> VerificationObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.get_verification(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">cancel_verification</a>(...) -> VerificationObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.cancel_verification(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">list_disputes</a>(...) -> DisputeList</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Filter by `stage` for a queue.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.list_disputes()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**stage:** `typing.Optional[ListDisputesRequestStage]` 
    
</dd>
</dl>

<dl>
<dd>

**order:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">get_dispute</a>(...) -> DisputeObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.get_dispute(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">list_dispute_evidence</a>(...) -> DisputeEvidenceList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.list_dispute_evidence(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">add_dispute_evidence</a>(...) -> DisputeEvidenceObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Only while the dispute is in its evidence stage.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.add_dispute_evidence(
    id="id",
    actor="actor",
    body="body",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**actor:** `str` — The buyer or seller giving evidence.
    
</dd>
</dl>

<dl>
<dd>

**body:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**links:** `typing.Optional[typing.List[str]]` — Links to files the party provided, such as photos you store. HTTPS only.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">close_dispute_evidence</a>(...) -> DisputeObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.close_dispute_evidence(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">decide_dispute</a>(...) -> DisputeObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Your team's decision: who it went against, in writing, and with payments on, how much goes back to the buyer. On a claimed order, deciding against the party who disputed upholds the claim and completes the order; deciding against the claimant cancels it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.decide_dispute(
    id="id",
    against="buyer",
    note="note",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**against:** `DecideDisputeDtoAgainst` — Who the decision went against. They get a dispute_lost reputation event; the other party gets dispute_won.
    
</dd>
</dl>

<dl>
<dd>

**note:** `str` — The written decision, kept with the dispute.
    
</dd>
</dl>

<dl>
<dd>

**refund_amount:** `typing.Optional[float]` — Payments on only. Minor units to refund to the buyer; the rest goes to the seller. Defaults: a claimed order whose claim is upheld refunds nothing; one whose claim is rejected refunds everything; a dispute on a completed order refunds nothing.
    
</dd>
</dl>

<dl>
<dd>

**decided_by:** `typing.Optional[str]` — Who on your team decided, for the record. Up to 200 characters.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.trust.<a href="src/marketsdk/trust/client.py">open_dispute</a>(...) -> DisputeObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

On a claimed order, by the party who did not claim: the order becomes disputed. On a completed order, by either party inside the dispute window: the order stays completed.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.trust.open_dispute(
    id="id",
    actor="buy_034XtPDs7UJ0TXzTsdaHZa",
    reason="reason",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**actor:** `str` — The buyer or seller opening the dispute.
    
</dd>
</dl>

<dl>
<dd>

**reason:** `str` — What went wrong, in their words.
    
</dd>
</dl>

<dl>
<dd>

**metadata:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Moderation
<details><summary><code>client.moderation.<a href="src/marketsdk/moderation/client.py">list_flags</a>(...) -> FlagList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.moderation.list_flags()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[ListFlagsRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**target:** `typing.Optional[str]` — Only flags on this listing, seller, or review.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.moderation.<a href="src/marketsdk/moderation/client.py">create_flag</a>(...) -> FlagObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

On behalf of the end user who reported it.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.moderation.create_flag(
    target="lst_034XtPDs7UJ0TXzTsdaHZa",
    reporter="buy_034XtPDs7UJ0TXzTsdaHZa",
    reason="prohibited_item",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**target:** `str` — A listing, seller, or review id.
    
</dd>
</dl>

<dl>
<dd>

**reporter:** `str` — The end user reporting it: a buyer id or a seller id.
    
</dd>
</dl>

<dl>
<dd>

**reason:** `CreateFlagDtoReason` 
    
</dd>
</dl>

<dl>
<dd>

**note:** `typing.Optional[str]` — The reporter's own words.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.moderation.<a href="src/marketsdk/moderation/client.py">get_flag</a>(...) -> FlagObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.moderation.get_flag(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.moderation.<a href="src/marketsdk/moderation/client.py">get_moderation_queue</a>(...) -> ModerationQueueObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.moderation.get_moderation_queue()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**target_type:** `typing.Optional[GetModerationQueueRequestTargetType]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.moderation.<a href="src/marketsdk/moderation/client.py">list_moderation_actions</a>(...) -> ModerationActionList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.moderation.list_moderation_actions()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**target:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.moderation.<a href="src/marketsdk/moderation/client.py">create_moderation_action</a>(...) -> ModerationActionObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Resolves the target's open flags and logs who acted and why.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.moderation.create_moderation_action(
    target="target",
    action="dismiss",
    reason="reason",
    actor="actor",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**target:** `str` — The listing, seller, or review acted on.
    
</dd>
</dl>

<dl>
<dd>

**action:** `CreateModerationActionDtoAction` — `dismiss` closes the open flags and changes nothing else. `remove_content` removes a listing or a review; a removed review stops counting toward reputation. `suspend_seller` suspends the seller, or the seller of a listing, or a seller who wrote a review: they cannot publish or take orders, and their listings leave search. `reinstate_seller` lifts a suspension.
    
</dd>
</dl>

<dl>
<dd>

**reason:** `str` — Why. Kept with the action.
    
</dd>
</dl>

<dl>
<dd>

**actor:** `str` — Who on your team took the action, for the log.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Webhooks
<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">list_webhook_endpoints</a>(...) -> WebhookEndpointList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.list_webhook_endpoints()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">create_webhook_endpoint</a>(...) -> WebhookEndpointObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns the signing secret, once. Every delivery carries `MarketSDK-Signature: t=<time>,v1=<HMAC-SHA256 of "<time>.<body>">`.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.create_webhook_endpoint(
    url="https://shop.example/marketsdk/webhooks",
    enabled_events=[
        "*"
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**url:** `str` — An HTTPS URL on the public internet.
    
</dd>
</dl>

<dl>
<dd>

**enabled_events:** `typing.List[CreateWebhookEndpointDtoEnabledEventsItem]` — Event types to send, or `*` for all.
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**metadata:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">get_webhook_endpoint</a>(...) -> WebhookEndpointObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.get_webhook_endpoint(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">delete_webhook_endpoint</a>(...) -> DeletedWebhookEndpointObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.delete_webhook_endpoint(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">update_webhook_endpoint</a>(...) -> WebhookEndpointObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.update_webhook_endpoint(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**url:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**enabled_events:** `typing.Optional[typing.List[UpdateWebhookEndpointDtoEnabledEventsItem]]` 
    
</dd>
</dl>

<dl>
<dd>

**description:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[UpdateWebhookEndpointDtoStatus]` — Turn the endpoint off, or back on after it was turned off.
    
</dd>
</dl>

<dl>
<dd>

**metadata:** `typing.Optional[typing.Dict[str, str]]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">rotate_webhook_secret</a>(...) -> WebhookEndpointObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns the new secret, once. The old one stops at once.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.rotate_webhook_secret(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">list_webhook_deliveries</a>(...) -> WebhookDeliveryList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.list_webhook_deliveries()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**endpoint:** `typing.Optional[str]` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `typing.Optional[ListWebhookDeliveriesRequestStatus]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">get_webhook_delivery</a>(...) -> WebhookDeliveryObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.get_webhook_delivery(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">replay_webhook_delivery</a>(...) -> WebhookDeliveryObject</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a new delivery of the same event to the same endpoint.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.replay_webhook_delivery(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">list_events</a>(...) -> EventList</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.list_events()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**limit:** `typing.Optional[float]` 
    
</dd>
</dl>

<dl>
<dd>

**starting_after:** `typing.Optional[str]` — The `next_cursor` of the previous page.
    
</dd>
</dl>

<dl>
<dd>

**type:** `typing.Optional[ListEventsRequestType]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.webhooks.<a href="src/marketsdk/webhooks/client.py">get_event</a>(...) -> EventObject</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from marketsdk import MarketSDK
from marketsdk.environment import MarketSDKEnvironment

client = MarketSDK(
    token="<token>",
    environment=MarketSDKEnvironment.DEFAULT,
)

client.webhooks.get_event(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

