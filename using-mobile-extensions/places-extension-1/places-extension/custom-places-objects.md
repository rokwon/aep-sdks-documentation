# Custom Places objects

## Custom native classes to be used with Places APIs

{% tabs %}
{% tab title="iOS" %}
### ACPPlacesPoi

#### Definition

```text
/**
 *  @class ACPPlacesPoi
 *
 *  This class contains data that is directly correlated to the properties maintained by the Adobe Places Database.
 */
@interface ACPPlacesPoi : NSObject

@property (nonatomic, strong, nullable) NSString* identifier;  ///< The identifier for the POI
@property (nonatomic, strong, nullable) NSString* name;  ///< The name of the POI
@property (nonatomic) double latitude;  ///< The latitude of the POI's center
@property (nonatomic) double longitude;  ///< The longitude of the POI's center
@property (nonatomic) NSUInteger radius;  ///< The radius of the POI
@property (nonatomic, strong, nullable) NSDictionary<NSString*, NSString*>* metaData;  ///< Dictionary containing meta data for the POI
@property (nonatomic) Boolean userIsWithin;  ///< Indicates if the device is currently inside of this POI

@end
```
{% endtab %}

{% tab title="Android" %}
```java
public class PlacesPOI {
    public String getIdentifier();  ///< The identifier for the POI
    public String getName();         ///< The name of the POI
    public double getLatitude();    ///< The latitude of the POI's center
    public double getLongitude();    ///< The longitude of the POI's center
    public Map<String, String> getMetadata();    ///< Dictionary containing meta data for the POI
    public boolean containsUser();  ///< Indicates if the device is currently inside of this POI
```
{% endtab %}
{% endtabs %}

