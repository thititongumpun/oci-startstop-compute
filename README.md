# Start Stop OCI Compute

# Table of Contents

1. [Rule](#Rule)
2. [Singapore](#Singapore)
3. [Tokyo](#Tokyo)
4. [Manual](#Manual)
## Rule

นำ ocid ของ instance ที่ต้องการ stop คืนวันศุกร์ 00.00 AM start คืนวันจันทร์ 06.00 AM ตาม region ด้านล่าง
> Singapore เติม - ตามด้วย instance_id\
> Tokyo เติม + ตามด้วย instance_id

## Singapore

- ocid1.instance.oc1.ap-singapore-1.anzwsljrk644ttqci6oacrgenwsfge4qdknq26uc64ye2u25vkrqrub4hq4q
- ocid1.instance.oc1.ap-singapore-1.anzwsljrk644ttqc7jub553aepgufjdx6kbuf2sl3jixbabt6yscdxw4z7nq

## Tokyo

## Manual
```bash
curl \
  -H 'Content-Type: application/json' \
  -H 'x-api-key: SOMEAPIKEY' \
  https://oci-startstop-compute.vercel.app/task?region={sg|tokyo}&instanceId={instanceId}&action={start|stop}
```