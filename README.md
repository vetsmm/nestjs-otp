<p align="center">
  <a href="http://nestjs.com/" target="blank">
    <img src="https://nestjs.com/img/logo_text.svg" width="320" alt="Nest Logo" />
  </a>
</p>

<p align="center">
🔑 One Time Password (OTP) / 2FA for NestJS - Supports HOTP, TOTP and Google Authenticator
</p>

<p align="center">
  <a href="https://www.npmjs.com/org/vetsmm"><img src="https://img.shields.io/npm/v/@vetsmm/nestjs-otp.svg" alt="NPM Version" /></a>
  <a href="https://www.npmjs.com/org/vetsmm"><img src="https://img.shields.io/npm/l/@vetsmm/nestjs-otp.svg" alt="Package License" /></a>
  <a href="https://www.npmjs.com/org/vetsmm"><img src="https://img.shields.io/npm/dm/@vetsmm/nestjs-otp.svg" alt="NPM Downloads" /></a>
  <a href="https://opencollective.com/vmm#sponsor"  target="_blank"><img src="https://img.shields.io/badge/Support%20us-Open%20Collective-41B883.svg" alt="Support us"></a>
</p>


# NOTE: This is in active development
### Installation

```sh
npm install --save @vetsmm/nestjs-otp
#or
yarn add @vetsmm/nestjs-otp
```

## Getting Started
Add and initialize the global module to your App.module.ts

### Using `.registerAsync()` for dynamic values (preferred)

```typescript
@Module({
  imports: [
    ConfigModule.forRoot(),
   ],
  controllers: [AppController],
  providers: [AppService],
})
export class AppModule {}
```
Also supports `useClass` in `registerAsync` if you have a configuration class.

### Using `.register()` for static values
```typescript
@Module({
  imports: [],
  controllers: [AppController],
  providers: [AppService],
})
export class AppModule {}
```

### Usage
**NOTE: If using the `isGlobal: true` option, you do not need to import this service into other modules that belong to App.module**

```typescript
```

### Contributing

* [Mark Tripoli](https://github.com/triippz)

### License

MIT


### Thanks To
Based on yeojz's [otplib](https://github.com/yeojz/otplib)
