# # Charity

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**donation_percentage** | **string** | This field sets the percentage of the purchase price that the charitable organization (identified in the charityId field) will receive for each sale that the listing generates. This field is conditionally required if a seller is planning on donating a percentage of the sale proceeds to a charitable organization. This numeric value can range from 10 to 100, and in any 5 (percent) increments in between this range (e.g. 10, 15, 20...95,... 100). The seller would pass in 10 for 10 percent, 15 for 15 percent, 20 for 20 percent, and so on, all the way to 100 for 100 percent. Note: For this field, createItemDraft will only validate that a positive integer value is supplied, so the listing draft will still be successfully created (with no error or warning message) if a non-supported value is specified. However, if the seller attempted to publish this listing draft with an unsupported value, the charity information would just be dropped from the listing. | [optional]
**charity_id** | **string** | The eBay-assigned unique identifier of the charitable organization that will receive a percentage of the sales proceeds. The charitable organization must be reqistered with the PayPal Giving Fund in order to receive sales proceeds through eBay listings. This field is conditionally required if a seller is planning on donating a percentage of the sale proceeds to a charitable organization. The eBay-assigned unique identifier of a charitable organization can be found using the GetCharities call of the Trading API. In the GetCharities call response, this unique identifier is shown in the id attribute of the Charity container. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
