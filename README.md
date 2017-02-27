### Rating stars component for your Ionic 2 App
#### Usage:
On your view:
```
<ion-rating
    [numStars]="5"
    [readOnly]="false"
    [value]="3.2"
    (clicked)="starClicked($event)">
</ion-rating>
```
On your controller:
```
starClicked(value){
   console.log("Avaliaram em :", value);
}
```

