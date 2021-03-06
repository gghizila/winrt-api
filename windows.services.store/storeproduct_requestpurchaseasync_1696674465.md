---
-api-id: M:Windows.Services.Store.StoreProduct.RequestPurchaseAsync
-api-type: winrt method
---

<!-- Method syntax
public Windows.Foundation.IAsyncOperation<Windows.Services.Store.StorePurchaseResult> RequestPurchaseAsync()
-->

# Windows.Services.Store.StoreProduct.RequestPurchaseAsync

## -description
Requests the purchase of the default SKU and availability for the product and displays the UI that is used to complete the transaction via the Windows Store.

> [!IMPORTANT]
> This method must be called on the UI thread.

## -returns
An asynchronous operation that, on successful completion, returns a [StorePurchaseResult](storepurchaseresult.md) object that provides status and error info about the purchase.

## -remarks
If this method is not called on the UI thread, the [StorePurchaseResult](storepurchaseresult.md) return value might indicate that an error occurred, and the [ExtendedError](storepurchaseresult_extendederror.md) property could have the value 0x800706be. This value corresponds to the [RPC_S_CALL_FAILED](https://msdn.microsoft.com/en-us/library/windows/desktop/aa378645(v=vs.85).aspx) error code.

## -examples

## -see-also
[RequestPurchaseAsync(StorePurchaseProperties)](storeproduct_requestpurchaseasync_1703896342.md), [Enable in-app purchases of apps and add-ons](https://msdn.microsoft.com/windows/uwp/monetize/enable-in-app-purchases-of-apps-and-add-ons)