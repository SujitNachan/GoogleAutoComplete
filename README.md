# GoogleAutoComplete
let gpaViewController = GooglePlacesAutocomplete(
  apiKey: "[YOUR GOOGLE PLACES API KEY]",
  placeType: .Address
)

gpaViewController.placeDelegate = self // Conforms to GooglePlacesAutocompleteDelegate

presentViewController(gpaViewController, animated: true, completion: nil)
GooglePlacesAutocompleteDelegate supports three methods:

placesFound(places: [Place]): Invoked whenever the Google Places API is called
placeSelected(place: Place): Invoked when a new place is selected
placeViewClosed(): Invoked when the view is closed
