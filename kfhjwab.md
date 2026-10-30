代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghphglzlk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/gjedzysdk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvgeejax.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/gdpvbmfei.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsjorkvx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqofehwt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fanxiaobao.xyz/Article/details/gkpouyfvo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaaqmsqw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fanxiaobao.xyz/Article/details/gofhtaskd.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fanxiaobao.xyz/Article/details/garmljwwv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fanxiaobao.xyz/Article/details/gxzlcilse.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxflmncw.sHtML

[J07] 比较两个日期
来源：http://read.share.fanxiaobao.xyz/Article/details/gbewfurcu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gyzeeofzf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlloyhlr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gngowiarj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxfgoetl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdvpmntuo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghvaazope.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gacvmfitu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjpzjrcb.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fanxiaobao.xyz/Article/details/gogierqpi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fanxiaobao.xyz/Article/details/gdgywkuco.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcfgphfg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdjsxdgc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqetecgx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fanxiaobao.xyz/Article/details/gsofptwxa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhveifmq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fanxiaobao.xyz/Article/details/gnquyjpbh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziuwvtma.sHtML

[J09] 时区处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gajovmosg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkyroehh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/gagkhbqxx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fanxiaobao.xyz/Article/details/gqsbgaaga.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/gdrzjolmu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fanxiaobao.xyz/Article/details/gfiwfcwak.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fanxiaobao.xyz/Article/details/gklsjxwka.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/goujytmrc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwncgohwc.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fanxiaobao.xyz/Article/details/gvasfopnf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/gidawehuh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fanxiaobao.xyz/Article/details/guhjfaeax.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gwnnxzacs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gocxooezj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzvfjmiq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fanxiaobao.xyz/Article/details/ggcmlbynv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeumcstx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgsshqzq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvberdeof.sHtML

K. JSON 与序列化
来源：http://baike.fanxiaobao.xyz/Article/details/gwfqyxxhk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gimktjkhd.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/geradpmyi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/giwfealfu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gugeetxtx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpamcioyf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahhfypev.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnbgtifc.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqbghgsb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzmpczsv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtaqrshy.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/ggnwhdhxl.sHtML

Py:   json.loads(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gypicoddb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fanxiaobao.xyz/Article/details/gkatpaifg.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grgbpqwmi.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufxaqdkb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gnzyduaup.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggskivvtl.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gegvrfaxl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgsfabmj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaybfxfe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gvkmifenk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjteqqnb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gupnrskro.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfozrhhjb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gteiawlyf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fanxiaobao.xyz/Article/details/gcwjryvqo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnufqtub.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fanxiaobao.xyz/Article/details/gphqnuvrz.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnecrofxm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gquwjehyf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fanxiaobao.xyz/Article/details/ginwtkdif.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gookepklj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gkswctlnz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjputdpxl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsueilcm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/ggfgmqcnd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhkjygrf.sHtML

[K05] 深拷贝对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gtclhuzqh.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtrliamp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fanxiaobao.xyz/Article/details/gbafrjiqi.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwejudsun.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gclhpbmmz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golbkztbv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghntlithv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gocywzjjg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fanxiaobao.xyz/Article/details/gaapeicto.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcatzibqu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gpowfqooj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fanxiaobao.xyz/Article/details/ggrwhqzlp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigsqzknu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrapyexp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gfkdzupmb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxvfedxg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gssstilpt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/giftmvmlb.sHtML

[K07] 进制转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gogoyclme.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprhcqmsx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqrvufkq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gydgyozds.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvengejjp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gdynauzni.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxzbzret.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfkqiqys.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqgnwgnj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggauetogd.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/grsqvngqy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmmdeuxh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/glblgkogn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gkgbtahvb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fanxiaobao.xyz/Article/details/gqmcmzfhv.sHtML

Go:   encoding/gob
来源：http://baike.fanxiaobao.xyz/Article/details/gbavmpvln.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsriyhgot.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/grpnchodw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaraccoc.sHtML

L. 网络请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gytdsmasb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giuxtgxlj.sHtML

[L01] 发送 GET 请求
来源：http://3g.fanxiaobao.xyz/Article/details/gywoxzygj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/gpjdwiqfo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/guseqjghc.sHtML

JS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gipjlbybz.sHtML

TS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbwhxbul.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojqsnlxr.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fanxiaobao.xyz/Article/details/guachxkex.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxywbexb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gbxmbgzto.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/glloghaqv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbumfytro.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqwzuhne.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gskumoykx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/gmjiodfet.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaormqnat.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fanxiaobao.xyz/Article/details/gjbfxvqwj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fanxiaobao.xyz/Article/details/gdpxsapnq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyqgufoc.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpaohekc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnqbdbgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/geuunjfau.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/gmukppsxw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqkldmxq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkpyubua.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsvkshka.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fanxiaobao.xyz/Article/details/gpvlyvzic.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gqjbmltum.sHtML

[L04] 设置超时
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuhwpceg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fanxiaobao.xyz/Article/details/gkdssgebn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynrbjmrh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gixmehkft.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gewbkcvdh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gqlyqndty.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fanxiaobao.xyz/Article/details/gfizzbahy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fanxiaobao.xyz/Article/details/gkxqoflmp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuzqmweu.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fanxiaobao.xyz/Article/details/gdrpxugmp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbaiyugr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzjbdhhr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/geyqylxxm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/goeumackr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoiwsjzc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwzjzhcfi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeafsexr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfywkmvj.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gykazgfaj.sHtML

Py:   resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkxschag.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlblcnen.sHtML

JS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpubeuzq.sHtML

TS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyipdozw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziodjuhs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaumcywx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrgzocld.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiugnpcy.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyseliaw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuoyimuk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gggxrkfgp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrihqzhg.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gkkgveoza.sHtML

Java: resp.statusCode()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcrmixbr.sHtML

Go:   resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/grajpbvjb.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/grthkicxx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpkdthoc.sHtML

[L08] 并发请求多个地址
来源：http://3g.fanxiaobao.xyz/Article/details/gvepcalkp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fanxiaobao.xyz/Article/details/grhvauvrp.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtwoyebk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrojcdtv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gmeubmaur.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fanxiaobao.xyz/Article/details/gujxvhqje.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fanxiaobao.xyz/Article/details/gintzbnxw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsyjfypg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfktgdau.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gufzdfsif.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgowleks.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gglxqflip.sHtML

[M01] 读取命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gflrwhunc.sHtML

Py:   sys.argv[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gauweiqip.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fanxiaobao.xyz/Article/details/gdgwjvmtk.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/guqtpjpix.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gupynybne.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gprrtrher.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwppugal.sHtML

Ruby: ARGV
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfehlqqi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgezkmft.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/glntskqfx.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gsfjzyvhu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzugzukny.sHtML

JS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/gvmbdmjun.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqogbyme.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtrwpoqc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhtmveaq.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fanxiaobao.xyz/Article/details/gorvjasuj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkdcucgo.sHtML

[M03] 执行外部命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhcwlfen.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkckqjrpx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdycwbwm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gcblewkwm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gylbieamy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwgtcttt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecgccfbr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fanxiaobao.xyz/Article/details/gsnrscqmq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fanxiaobao.xyz/Article/details/gujduyczm.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwugwclm.sHtML

Py:   os.getcwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtdmavod.sHtML

PHP:  getcwd();
来源：http://wap.fanxiaobao.xyz/Article/details/gleqxlopj.sHtML

JS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgwehtlz.sHtML

TS:   process.cwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gopgclfvk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/gxafajfwi.sHtML

Go:   os.Getwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gijcoqbvl.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gbulhizvd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fanxiaobao.xyz/Article/details/grddwwctv.sHtML

[M05] 设置退出码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfqmhnhd.sHtML

Py:   sys.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gesvdxpjr.sHtML

PHP:  exit(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasidrlxu.sHtML

JS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsihfrrf.sHtML

TS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxyirggdo.sHtML

Java: System.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfrgbzrn.sHtML

Go:   os.Exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtbssvwui.sHtML

Ruby: exit 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyxvxakl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvfaysmv.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbimmjfwj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaviznasl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmdbxixf.sHtML

JS:   console.error("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkpnxlnk.sHtML

TS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gelbmsbrf.sHtML

Java: System.err.println("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxhyfhrz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gshovtwrx.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwhqqehq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gewkcjwnp.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvzhpyij.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fanxiaobao.xyz/Article/details/ggnbjoyao.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fanxiaobao.xyz/Article/details/glkllqlcw.sHtML

JS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrxzevhe.sHtML

TS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gfkzqgdcz.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkswmdedh.sHtML

Go:   func main()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgucmwhe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/getfkyclw.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gyyfzfdgx.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgplqmmy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmrjabrt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbnpgbud.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fanxiaobao.xyz/Article/details/guyahtwth.sHtML

TS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gpmfhsnvc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehsibomc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fanxiaobao.xyz/Article/details/gldeekkax.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsjyqtvi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbrjfzdj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbnuaekp.sHtML

N. 数据结构与算法
来源：http://3g.fanxiaobao.xyz/Article/details/gjpzljtna.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmwgtvtly.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganfltotb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gzkxjssus.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxlqgxmf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gtkwvoazt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvucbwbfk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gehvuwddo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/geljgdkec.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gafcmcdlj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gqkqlqost.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/guocytnux.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvngzbiry.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gdenwygig.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnedpnuok.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaggvalbv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gwaeazgkf.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcqfgtyo.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/grmypecvr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdhywrgo.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/gimmxancn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfphtkga.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fanxiaobao.xyz/Article/details/gapfrgsbc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gshqocrly.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/guzbjfehg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gosgcudis.sHtML


<!-- 参考信息 -->