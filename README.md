# checkout-react-native-module

Formulário Checkout PCI Martins - Smart

## Installation

```sh

yarn add checkout-react-native-module

```

## You need to install all peer dependencies if they are not installed:

```sh

yarn add @react-native-picker/picker
yarn add prop-types
yarn add react-native-picker-select
yarn add rn-material-ui-textfield
yarn add axios

```

## Getting Started

```js

import { Checkout } from 'checkout-react-native-module';

// ...

export default function App() {
    return (
        <Checkout
        baseURL={'https://api.com'}
        storedId={'BTB'}
        deviceType={'MOBILE'}
        installments={'1'}
        purchaseOrderId={'34234'}
        transactionType={'SUB'}
        binRestriction={'NAO'}
        validListBins={'1|10|100|1000'}
        tricardIndicator={false}
        cardBrand={'VISA'}
        onSuccess={(data) => {}}
        onError={(error) => {}} />
    )
}

```