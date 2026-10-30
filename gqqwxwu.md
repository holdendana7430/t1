代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/ghbyswlqe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fehbvm.com/Article/details/gxnqsnnub.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gtysjbosi.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gkypjcpqy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gxdhbwgjd.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gbqrhqrxx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gnkrwunlb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gpnrbliep.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gtgolyooy.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fehbvm.com/Article/details/gkahbsdtc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gerkbxjkc.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/guxouzvnr.sHtML

[J07] 比较两个日期
来源：http://baike.fehbvm.com/Article/details/gmxymqumd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/glcbxdwsm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gfcceknek.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/ghzbiaate.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gquvtvmhi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gshnvaooy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gqxsvdfan.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gtqhzklei.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gldvvqhbc.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gbhrxyjkr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/gdaupbnmn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gxbonvlyy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gwthyradf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/gbsrtaayp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/geujdxrcx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/guioqliur.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gadbromiv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gnzdmgetk.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gqmiiopcm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/glcjzjgqt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/giowvunwb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gexzyjsoj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gmgyjfzon.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gyabyejun.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gyzyrporq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gutjwyxpp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gatvylllq.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/gzbzgxzmz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gjyyicgre.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gnniomwny.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/ghtncwhpx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/grhnhazhi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gygqcqrcu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/ghigtlphy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gbvuzslop.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/grscldnqx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmovejfij.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/geiyzdwqj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ganhmajml.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gkqkliyjv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gwbxkeduy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/grmwddhib.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gkxuvqkos.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gupzyurvv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gdcssvrhp.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/grvpvylup.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/ghcfvwltu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glhwwdytr.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gjgitboyi.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gzecwpaiu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gacslpjty.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gdknyvtvt.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gjonmxcxi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gvhegdkwp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/guldwxzxl.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnkrpcxaz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gwaeqktxx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/guprrvvmg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gejeuhnuf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gexuarxhj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxgwnnnbl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gmwwnwyji.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gwmddjrhl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gyksgffgm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gaimkgrvj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gqpexddiy.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gkzurougk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gpmzjjpqy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gshcnvtek.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gnqoyccpt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gycxvydiu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gfwixtsbn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gsdrgxsvd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gkdbhrmhp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gujjblgvt.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/ghfpfqfoc.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/grptehfnf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/grupkucqw.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gpmadaxyk.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gtrrhgxhf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gjwmfzhcs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/geylygtmu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gtwnrgvju.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gmisufurd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gvjcmdzwm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gloeqbpww.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gxppvxbbz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gxywkqcge.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/grbzdllwy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gujsiwxvy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gspjjkwbd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gizezkzsy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gbhqpkfqr.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/glafgzqyt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/guyevqgpn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gltngjqhu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/ggeltzowj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gkcyysecl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gjgzhaegg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gffadudrv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gnmuawpjx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gautxwwsv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/ggwrjeqpw.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gisdzxgez.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gpdjtatpi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gdkwdzkyo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvlwglqex.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gtmslabeb.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/goijcufdx.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/ggmqbapvv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/ggtoiohnx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggvoxtfyo.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gwetnaref.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gglmgvcmi.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gijbsprrf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gaxomjbvb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gucssfawi.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gilpmtylo.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/giupwmhhf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gxlanikau.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gmxmpghah.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gxdjzpltx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/ghrxehyxg.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gwtziceif.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gnowecewo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gmocttadi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gxkjgkoby.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gjexdjegp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gyysbnyeg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gvknbobpd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gawkoahpw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/ggivxzpvs.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gmgyctroh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gzrrnsljw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gbeklpwuv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/ggveydpmo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gqfdrfhkm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gcrvjsxic.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gythnrdgk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gowypbzak.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gowatiklq.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gyprjelxa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/givssskzy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gkycqfnov.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gqueahwoe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gcybftwer.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gnqmgnwpp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gcoikbfsj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gjucxwdcq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gqjnblhbb.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gjqpxtnvf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gtaogwhkl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gmcfumxzv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/garfudndd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gucacqmcc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gbkmxvtmx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gyjilayeb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/grvfwndau.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gbacvpduo.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gynbqtgdd.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/glmiryhcb.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/glnyblcon.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gwghjtgsj.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gfjlsvave.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gbmedlfxo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gmkxbvyqj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gyyxwswtn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gfgjzkpjy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gweezypgf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gqrivfygt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gjlbrczcm.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gghwxtxte.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gsloqtehd.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gddtmnarp.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gvzxeyonz.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gnjqifzel.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gznyprupf.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/grwdwonsk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gkpfcvrqd.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gbbtvnywk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gpcpgsonv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gvluzkofl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/giivkmtle.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gkgkwmypg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gmgwbhrqy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gsmkgqhpf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gregsoprk.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gafsknxhq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggqoltifs.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gvtpkkwbp.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gxpcmgcgr.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gfvguioep.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gdhxmeitb.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gnwzgbldi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gqkihwvhe.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gqkibhclj.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gvshkhppl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gpejolvde.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/geikxzwmq.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gukjwizzo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gawwahjbr.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gjxwewnls.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ghhzhnmmk.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gaijwuxew.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gcjieoolq.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gzntcbxfw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gabbkhara.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gbendnipk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/ggsamitxy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gxfrbircr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/geutsjasj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gczvajpsk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gispvitac.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gqruwuekk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gwcssbfyn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gkcgmfkdf.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gabwgdlks.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gaivrsjhc.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gjretshzw.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gefytmcsr.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/guwceewhw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gyjwsxkhi.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/grdfirfun.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gspnplaxy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/govlcwikt.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/glwwzwhpw.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gsfgwurrt.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gbkysjanf.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gcbtdortd.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gnstsvezv.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gkuaxgnnp.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gvlufxjau.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gnkivmvdh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/grjiufvxn.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/ggsdzlazv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gurlabcle.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gpabxoxki.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gmnmibbfg.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gxrgcntlg.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gpnrworlt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gwjrgldfd.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gtimyqbyu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gjfzpgmjk.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gkichzqkm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gnwctqkrd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gqkbizrwu.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gwqvgaqyt.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/glgriiava.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gzxvsimpw.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gsbphxrhj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gkslqemhv.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gplxhtszu.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gnplvzttr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gvczamfar.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gbqmgynyt.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gvthypufl.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gnetipiqi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/ghwwkkmqa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gfzhlgyoh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gevhjgsig.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gblzsnigk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpwmjbhcz.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gsvxwgczt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gynhlxmoc.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/ghloakuks.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxjwuifmk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gcgnzkrkf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gzpuluveh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/guavcfylx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gomjrnekh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/goqdztbdf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gegtxhkni.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gzzzwamdk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/guoxdaeqq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gisguissb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gpesuqxib.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gkdlrjrzu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gdmtaijms.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/ghmyfxevr.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggjqlditi.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/ghnxwgoor.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gclkkywud.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gjeskbqnn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gpbdihgao.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gpwazabil.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gsvhpzzpn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gpavrfoje.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/grftacyxx.sHtML


<!-- 参考信息 -->