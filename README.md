# button-radioButoon
add purple button and primary radio button
.btn {
  &-sm {
    height: toRem(40);
    padding-inline: toRem(18);
    font-size: $xs;
    @include align-items(center);

    .btn-normal__icon-start {
      margin-left: toRem(6);
    }

    .btn-normal__icon-end {
      margin-right: toRem(6);
    }
  }

  &-md {
    height: toRem(48);
    padding-inline: toRem(26);
    font-size: $sm;
    @include align-items(center);

    .btn-normal__icon-start {
      margin-left: $p-8;
    }

    .btn-normal__icon-end {
      margin-right: $p-8;
    }
  }

  &-lg {
    height: toRem(56);
    padding-inline: toRem(34);
    font-size: $sm;
    @include align-items(center);

    .btn-normal__icon-start {
      margin-left: toRem(10);
    }

    .btn-normal__icon-end {
      margin-right: toRem(10);
    }
  }

  &__label {
    font-weight: bold;
    @include flexbox;
    @include align-items(center);
  }

  &-icon {
    &__sm {
      padding: $p-12;
    }
    &__md {
      padding: $p-12;
    }
    &__lg {
      padding: $p-16;
    }
  }

  &__loading {
    width: toRem(21);
    height: toRem(21);
  }

  &-fill {
    border-radius: $border-radius;
    border: none;
    transition: 0.3s;
    color: $white;
    @include flexbox;
    font-weight: bold;

    &:disabled {
      pointer-events: none;
      cursor: auto;
    }
  }

  &-outline {
    border-radius: $border-radius;
    background-color: transparent;
    @include flexbox;
    transition: 0.3s;
    font-weight: bold;
    &:disabled {
      pointer-events: none;
      cursor: auto;
    }
  }

  &-text {
    border-radius: $border-radius;
    background-color: transparent;
    border: none;
    transition: 0.3s;
    font-weight: bold;
    &:disabled {
      pointer-events: none;
      cursor: auto;
    }
  }

  &-block {
    @include flexbox;
    @include justify-content(center);
    width: 100%;

    &.btn-sm {
      padding-inline: toRem(14);
    }

    &.btn-md {
      padding-inline: toRem(18);
    }

    &.btn-lg {
      padding-inline: toRem(18);
    }

    .btn__label {
      position: relative;
      width: 100%;
      justify-content: space-between;

      &-value {
        margin-inline: auto;
      }
    }
    &__icon {
      display: initial;
      text-align: center;
      position: absolute;

      &-left {
        left: 0;
      }
    }
  }

  &-primary-fill {
    background-color: $primary;
    &:hover {
      background-color: $primary-dark;
    }
    &:focus {
      background-color: $primary-darker;
    }
    &:disabled {
      background-color: $empty-state-dark;
    }
  }

  &-primary-outline {
    border: 2px solid $primary;
    color: $primary;
    &:hover {
      background-color: $primary-white;
    }
    &:focus {
      background-color: $primary-lighter;
      border: 2px solid $primary-darker;
      color: $primary-darker;
    }
    &:disabled {
      border: 2px solid $empty-state-dark;
      color: $empty-state-dark;
    }
    .spinner-disabled {
      stroke: $empty-state-dark;
    }
  }

  &-primary-text {
    display: flex;
    color: $primary;
    &:hover {
      background-color: $primary-white;
    }
    &:focus {
      color: $primary-darker;
      background-color: $primary-lighter;
    }
    &:disabled {
      color: $empty-state-dark;
    }
    .spinner-disabled {
      stroke: $empty-state-dark;
    }
  }

  &-secondary-fill {
    color: $white;
    background-color: $secondary;
    &:hover {
      background-color: $secondary-dark;
    }
    &:focus {
      background-color: $secondary-darker;
    }
    &:disabled {
      background-color: $empty-state-dark;
      color: $white;
    }
  }

  &-secondary-outline {
    color: $secondary;
    border: 2px solid $secondary;
    &:hover {
      background-color: $secondary-white;
    }
    &:focus {
      background-color: $secondary-light;
      color: $secondary-darker;
      border: 2px solid $secondary-darker;
    }
    &:disabled {
      border: 2px solid $empty-state-dark;
      color: $empty-state-dark;
    }
    .spinner-disabled {
      stroke: $empty-state-dark;
    }
  }

  &-secondary-text {
    color: $secondary;
    &:hover {
      background-color: $secondary-white;
    }
    &:focus {
      color: $secondary-darker;
      background-color: $secondary-lighter;
    }
    &:disabled {
      color: $empty-state-dark;
    }
    .spinner-disabled {
      stroke: $empty-state-dark;
    }
  }

  &-primary-white-fill {
    color: $primary;
    background: $white;
    &:hover {
      background-color: $primary-white;
    }
    &:focus {
      background-color: $primary-lighter;
      color: $primary-dark;
    }
    &:disabled {
      background: $empty-state;
      color: $empty-state-dark;
    }
    .spinner-disabled {
      stroke: $empty-state-dark;
    }
  }

  &-primary-white-outline {
    color: $white;
    border: 2px solid $white;
    &:hover {
      background-color: $primary-dark;
    }
    &:focus {
      background-color: $primary-darker;
    }
    &:disabled {
      border: 2px solid $empty-state;
      color: $empty-state;
    }
    .spinner-disabled {
      stroke: $empty-state;
    }
  }

  &-primary-white-text {
    display: flex;
    color: $white;
    &:hover {
      background-color: $primary-dark;
    }
    &:focus {
      background-color: $primary-darker;
    }
    &:disabled {
      color: $empty-state;
    }
    .spinner-disabled {
      stroke: $empty-state;
    }
  }

  &-secondary-white-fill {
    color: $secondary;
    background: $white;
    &:hover {
      background-color: $secondary-white;
    }
    &:focus {
      background-color: $secondary-lighter;
      color: $secondary-dark;
    }
    &:disabled {
      background: $empty-state;
      color: $empty-state-dark;
    }
    .spinner-disabled {
      stroke: $empty-state-dark;
    }
  }

  &-secondary-white-outline {
    color: $white;
    border: 2px solid $white;
    &:hover {
      background-color: $secondary-dark;
    }
    &:focus {
      background-color: $secondary-darker;
    }
    &:disabled {
      border: 2px solid $empty-state;
      color: $empty-state;
    }
    .spinner-disabled {
      stroke: $empty-state;
    }
  }

  &-secondary-white-text {
    display: flex;
    color: $white;
    &:hover {
      background-color: $secondary-dark;
    }
    &:focus {
      background-color: $secondary-darker;
    }
    &:disabled {
      color: $empty-state;
    }
    .spinner-disabled {
      stroke: $empty-state;
    }
  }

  &-neutral-fill {
    background-color: $text-dark;
    &:hover {
      background-color: $text-gray;
    }
    &:focus {
      background-color: $text;
    }
    &:disabled {
      background-color: $empty-state-dark;
    }
  }

  &-neutral-outline {
    border: 2px solid $text-dark;
    color: $text-dark;
    &:focus {
      background-color: $text;
      border: 2px solid $text-dark;
      color: $text-dark;
    }
    &:disabled {
      border: 2px solid $empty-state-dark;
      color: $empty-state-dark;
    }
    .spinner-disabled {
      stroke: $empty-state-dark;
    }
  }

  &-neutral-text {
    display: flex;
    color: $text-dark;
    &:hover {
      background-color: $background;
    }
    &:focus {
      background-color: $text-gray;
    }
    &:disabled {
      color: $empty-state-dark;
    }
    .spinner-disabled {
      stroke: $empty-state-dark;
    }
  }
}

&-trietary-fill {  
  color: $white;
  background-color: $trietary;
  &:hover {
    background-color: $trietary-dark;
  }
  &:focus {
    background-color: $trietary-darker; 
  }
  &:disabled {
    background-color: $empty-state-dark;
  }
}

&-trietary-outline {  
    color: $trietary;
    border: 2px solid $trietary;
    &:hover {
      background-color: $trietary-white;
    }
    &:focus {
      background-color: $trietary-light;
      color: $trietary-darker;
      border: 2px solid $trietary-darker;
    }
    &:disabled {
      color: $empty-state-dark;
      border: 2px solid $empty-state-dark;
    }
    .spinner-disabled {
      stroke: $empty-state-dark;
    }
  }



  &-trietary-text {  
    display: flex;
    color: $trietary;
    &:hover {
      background-color: $trietary-white;
    }
    &:focus {
      color:$trietary-darker;
      background-color: $trietary-lighter;
    }
    &:disabled {
      border: 2px solid $white;
      background-color: $white;
      color:$empty-state-dark;
    }
    .spinner-disabled {
      stroke: $empty-state-dark;
    }
  }
  

  
