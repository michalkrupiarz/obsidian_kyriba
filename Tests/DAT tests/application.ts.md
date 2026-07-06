const domainName = process.env.DOMAIN_NAME ?? 'diamond-preprod.treasury-factory.com' //'kapp.kip1.proto.kyriba.io' //'diamond.treasury-factory.com' //'ruby.treasury-factory.com' //'onyx-sandbox.treasury-factory.com' // //  //'diamond.treasury-factory-dr.com' // //'onyx-sandbox.treasury-factory.com'  //'diamond.treasury-factory-dr.com'//'neo.proto.cloud.kyriba.com'//'neo.proto.cloud.kyriba.com'  'ruby.treasury-factory.com' // 'localhost'  
const port = process.env.PORT ?? '' // 8080

const headLess = process.env.HEADLESS ? process.env.HEADLESS == 'false' : false //'true' : true

baseUrl: `http${secure ? 's' : ''}://${domainName}${port}`,