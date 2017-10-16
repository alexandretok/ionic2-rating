### Rating stars component for your Ionic 2 App
#### Installation:
Copy the `ion-rating` folder to your `src/components/` folder and import it on your `app.module.ts` and add `IonRating` to the declarations arrays.

```
// ... other imports ...
import { IonRating } from '../components/ion-rating/ion-rating';
```
```
declarations: [
  MyApp,
  HomePage,
  // ... other declarations ...
  IonRating
],
```

#### Usage:
On your view:
```
<ion-rating
    [numStars]="5"
    [readOnly]="false"
    [value]="3.2" <!-- this can be either a number or a variable -->
    (clicked)="starClicked($event)">
</ion-rating>
```
On your controller:
```
starClicked(value){
   console.log("Rated :", value);
}
```

