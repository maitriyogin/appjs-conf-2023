## App JS Conf 2023

![Krakow Dragon](photos/IMG_4171.jpeg)

### Wednesday

#### Workshop - Expo Modules

(Material)[https://hackmd.io/@EFXGBcSCR0-VcFBNI6D-ng/BkWnHLhW3]

Really well documented, communicated and with great exercises.
It's now unbelievably easy to integrate Native code into RN with the help of the new architecture.

```ts
import { FirstModule } from 'workshops-charts';
<View style={styles.button}>
        <Button
          title="Run async function"
          onPress={async () => {
            const module = requireNativeModule('FirstModule');
            const result = await module.functionAsync();
            Alert.alert('NativeModule', JSON.stringify(result));
          }}
        />
      </View>

      <View style={styles.button}>
        <Button
          title="Run sync function"
          onPress={() => {
            const module = FirstModule;
            const result = module.function();
            Alert.alert('NativeModule', JSON.stringify(result));
          }}
        />
      </View>
```

```ts
import { requireNativeModule } from 'expo-modules-core';

type FirstModuleType = {
  readonly functionAsync: () => Promise<string>;
  readonly function: () => string;
};

const module = requireNativeModule<FirstModuleType>('FirstModule');

export default module;
```

```swift
import ExpoModulesCore

public class FirstModule : Module {
  public func definition() -> ModuleDefinition {
    Name("FirstModule")

    AsyncFunction("functionAsync") {
      return "Hi from Async"
    }

    Function("function") {
      return "Hi there!"
    }
  }
}
```

### The beer garden

![Eszweria](photos/IMG_4143.jpeg)
![beer garden](photos/IMG_4140.jpeg)
[Eszeweria](https://www.google.com/maps/place/Eszeweria/@50.0506342,19.9445393,3a,75y,90t/data=!3m8!1e2!3m6!1sAF1QipM1A1aGMkP777Ueb06wiToingpHWz3pIEnKFwk!2e10!3e12!6shttps:%2F%2Flh5.googleusercontent.com%2Fp%2FAF1QipM1A1aGMkP777Ueb06wiToingpHWz3pIEnKFwk%3Dw114-h86-k-no!7i4032!8i3024!4m17!1m9!3m8!1s0x47165b6a2e7d8bef:0x62672e9c1bce5ed7!2sKazimierz,+Kraków,+Polen!3b1!8m2!3d50.0485563!4d19.9447183!10e5!16zL20vMDJ2cHk4!3m6!1s0x47165b7d5b894933:0xfff2cca5d376a5e6!8m2!3d50.0505691!4d19.9445711!10e5!16s%2Fg%2F11gmt9t0bn?entry=ttu)

### Thurday - talks

![SoftwareMansion](photos/IMG_4150.jpeg)
![Audience](photos/IMG_4151.jpeg)

## Keynote

- **_Charlie Cheever & James Ide
  Keynote - community and workflows_**

![Eco system](photos/IMG_4166.jpeg)
![npm trends](photos/IMG_4157.jpeg)
![expo](photos/IMG_4158.jpeg)
![RN Enhancements from Meta](photos/IMG_4162.jpeg)
![Expo router](photos/IMG_4163.jpeg)
![Expo Enhancements](photos/IMG_4164.jpeg)
![Fewer people](photos/IMG_4165.jpeg)
Blue Sky the new twitter

![Blue Sky](photos/IMG_4167.jpeg)
![Brex](photos/IMG_4169.jpeg)

- Jon Samp
  Expo Application Services: Iterate with confidence

![Deploy your apps faster](photos/IMG_4171.jpeg)
![PRs](photos/IMG_4176.jpeg)
![PRs](photos/IMG_4177.jpeg)
![PRs](photos/IMG_4182.jpeg)
![40% faster builds](photos/IMG_4184.jpeg)

- **_William Candillon
  The joy of painting with Skia_**

![Skia](photos/IMG_4188.jpeg)
![Skia](photos/IMG_4185.jpeg)

- **_Johannes Schickling
  Local-first state management with Riffle & SKDB_**

![Local first](photos/IMG_4189.jpeg)
![Caching optimistic updates](photos/IMG_4191.jpeg)
![Caching optimistic updates](photos/IMG_4192.jpeg)
![State management is the problem](photos/IMG_4194.jpeg)
![Tristan Hume](photos/IMG_4196.jpeg)
![Local first](photos/IMG_4197.jpeg)
![Riffle](photos/IMG_4203.jpeg)

Realm mongo db

- **_Kadi Kraman
  Building 5 star app_**

![Decision fatigue](photos/IMG_4205.jpeg)
![Play is different](photos/IMG_4206.jpeg)
![App reviews](photos/IMG_4208.jpeg)
![Asking for reviews](photos/IMG_4210.jpeg)
![In summary](photos/IMG_4214.jpeg)

- **_Evan Bacon
  Write once, route everywhere: File system-based navigation for native apps_**

![Mobile Internet Usage](photos/IMG_4215.jpeg)
![Mobile Gateway Sites](photos/IMG_4216.jpeg)
![Mobile Gateway Sites](photos/IMG_4217.jpeg)
![Universal](photos/IMG_4218.jpeg)
![Universal](photos/IMG_4219.jpeg)
![Universal](photos/IMG_4220.jpeg)
![Universal](photos/IMG_4221.jpeg)
![CSS](photos/IMG_4225.jpeg)
![CSS metro](photos/IMG_4226.jpeg)
![CSS in native](photos/IMG_4227.jpeg)
![Summary](photos/IMG_4229.jpeg)

- Monica Restrepo
  How does Shopify change and adapt to the new architecture changes in React Native?

![Upto date](photos/IMG_4230.jpeg)

- Krzysztof Piaskowy
  3D and Canvas-Based Animations with Reanimated

- Kudo Chien
  React Native on Linux with the new architecture

- **_Saad Najmi
  Taking React Native to macOS_**

![RN on MACOS](photos/IMG_4237.jpeg)
![Invest](photos/IMG_4238.jpeg)
![WHY](photos/IMG_4239.jpeg)
![WHY](photos/IMG_4247.jpeg)

- **_Nate
  Tamagui_**

![Tamagui](photos/IMG_4248.jpeg)
![Tamagui](photos/IMG_4249.jpeg)
![Why](photos/IMG_4251.jpeg)
![Why](photos/IMG_4254.jpeg)
![death of creativity](photos/IMG_4255.jpeg)
![optimize](photos/IMG_4257.jpeg)
![speed simplicity](photos/IMG_4263.jpeg)

### Evening

[Alchemia](https://www.google.com/maps/place/Alchemia/@50.0522148,19.9450978,3a,75y,90t/data=!3m8!1e2!3m6!1sAF1QipOpEgS-hbJxkLkyERbXAKPiIGmhnWkkeOa0elEe!2e10!3e12!6shttps:%2F%2Flh5.googleusercontent.com%2Fp%2FAF1QipOpEgS-hbJxkLkyERbXAKPiIGmhnWkkeOa0elEe%3Dw99-h86-k-no!7i1334!8i1151!4m16!1m8!3m7!1s0x47165b6a5d7eda4b:0x71c57113b17f155e!2splac+Nowy,+31-056+Kraków,+Polen!3b1!8m2!3d50.0518711!4d19.9446205!16s%2Fg%2F123266t4!3m6!1s0x47165b6c64662dab:0x5daf119c1937989d!8m2!3d50.0521919!4d19.9450021!10e5!16s%2Fg%2F11fmlf4d1n?entry=ttu)

![Alchemia](photos/IMG_4268.jpeg)
![Alchemia](photos/IMG_4269.jpeg)

### Friday - talks

- Nicola Corti
  22 - A year in review for React Native

![Hermes](photos/IMG_4281.jpeg)
![Modern languages](photos/IMG_4282.jpeg)
![TS](photos/IMG_4283.jpeg)
![Web props](photos/IMG_4284.jpeg)
![Flex gap](photos/IMG_4285.jpeg)

- **_Alex Hunt
  Metro and React Native DevX in 2023_**

![Metro](photos/IMG_4292.jpeg)
![Flex gap](photos/IMG_4288.jpeg)
![Flex gap](photos/IMG_4292.jpeg)
![Flex gap](photos/IMG_4293.jpeg)
![Rapid app dev](photos/IMG_4295.jpeg)
![Fast refresh](photos/IMG_4297.jpeg)
![MS](photos/IMG_4299.jpeg)
![Expo Router](photos/IMG_4300.jpeg)
![Sym links](photos/IMG_4302.jpeg)
![Laz bundling](photos/IMG_4307.jpeg)
![Hear our input](photos/IMG_4309.jpeg)
![Debugging](photos/IMG_4310.jpeg)
![DevX](photos/IMG_4311.jpeg)

- Vít Horáček
  How Expensify works with the open source community to 'live rich, have fun & save the world'

- **_Cedric van Putten
  Debugging should be easier_**

![Debugging with vscode expo ](photos/IMG_4316.jpeg)
![Debugging with vscode expo step thru ](photos/IMG_4317.jpeg)
![Summary](photos/IMG_4320.jpeg)

- Wojciech Stanisz
  The art of React Native: How to make your app stand out
  ![Summary](photos/IMG_4321.jpeg)

- Simon Sturmer
  The long-tail of type safety

  ![TS is not safe](photos/IMG_4323.jpeg)
  ![strict](photos/IMG_4324.jpeg)
  ![ts reset](photos/IMG_4325.jpeg)
  ![io boundaries](photos/IMG_4326.jpeg)
  ![io boundaries](photos/IMG_4329.jpeg)
  ![better type safety](photos/IMG_4330.jpeg)

- Ankita Kulkarni
  The performance myths of React Native apps

  ![1](photos/IMG_4331.jpeg)
  ![2](photos/IMG_4332.jpeg)

- Arthur Lee
  Dark mode at scale with React Native

- **_Varun Dhananjaya, Ashoat Tevosyan
  How to integrate Rust into a React Native app_**

  ![JSI](photos/IMG_4335.jpeg)

- Alexandre Moureaux
  Lighthouse for mobile apps

  ![Lighthouse](photos/IMG_4336.jpeg)
  ![Flashlight](photos/IMG_4337.jpeg)
  ![Metrics](photos/IMG_4339.jpeg)

- Henry Moulton
  React Native end-to-end testing with Maestro

  ![Testing](photos/IMG_4345.jpeg)
  ![Uber](photos/IMG_4346.jpeg)
  ![What is maestro](photos/IMG_4348.jpeg)
  ![live](photos/IMG_4350.jpeg)
  ![Game changer](photos/IMG_4351.jpeg)

- Jonny Burger
  Making videos in React Native

  ![Remotion dev](photos/IMG_4353.jpeg)

- Panel Discussion

  ![The panel](photos/IMG_4354.jpeg)
