代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3cnvcpetr.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3splqpfjh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3vcgddikk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xjfzmijk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3akivlzih.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3xpseyjnq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3bybaqhcg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3edpxxtrw.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3datibgld.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hygqfpmp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3npsawtje.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3evomtffh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3todjphjy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3stryqiyq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3wncwcnst.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mljefiuq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3aclkyjwj.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3cwhjqyeg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3bxmgqklq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ixpqljml.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xnmxwffr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3zfdgeeqh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3nyuhetrc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3hbofvztn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3mplasusu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3soqtwnif.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3kztpxkox.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3wqpffjdz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3crqjprbh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3blzaidoa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rekxodvb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3orxrxnfl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3avtvyios.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3zcunrrae.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3tlzfywzg.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3nabxyyne.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qruseidq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3vdcqkqrs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ihrhflec.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ivzuymre.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ectwpgaj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ibejqdqt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3uswyzdph.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3cwaattal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccqdyqsy.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3juirxphb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdrvxdrz.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tjglaocs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ruvjgoyp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3sljkamwq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3sunmyfgb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vkvxudoo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3tginjgyy.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zyuueuit.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3uhszlrij.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aqpcrpyi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ocyzhovu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyrvhve.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3yzrwongl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3trxvyixr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3azxtfaff.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kzhohykm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vfdbexph.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jqkpedtz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3inhxwuvz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3reijvubf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jmbokcua.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yisrruwc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3whcckpju.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3eoqjnshv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mirzhijx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qnvqaeuu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nppukzrt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3gfheuzhi.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3puihbysw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mrvreram.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wrornxwg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qxtgcxdu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nqhlucsd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3agggccvy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3msdpuagj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tzaynkkk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3bdwksxrg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3atwajfas.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkbbakk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3znwloghy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3apffgzun.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wwnqtkhh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3gzcfeymb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3dodrljus.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3igtvaryc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ervowlxk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3jzktrjmt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gfilzfux.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3nvyqbpsl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kjlvawst.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kmxfcgdv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qioisfpw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hfppkyav.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xecfmspc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vbavnmqd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3aiztptfp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pwvrkefc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3nmfhtiws.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vwtxswdm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xpjlocjg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3npxlseds.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3wkolkzvz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lvaknkdp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tajzalcz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3bqkvndpz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3botnycdc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3pyqyahde.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3diwxamqi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lwcycwwn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3gtmhnayz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3rnnmalmm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3frzxpgso.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rucovmvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxjdonve.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3enkumaer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3voicushm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3unybnyqj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3tfblfscp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3lnwoymbw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fbfigsyt.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wtebeikz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3bdpdwsvv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pibigpsl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mwefbtse.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3xgfcjfjb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ebfzwqnm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xejbpmzo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3dzxjlzrw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xjjloazk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qiohrnzi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zbwgrrhg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3tzgylgni.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xdnbqvgf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rjwzjhwa.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3qvkuplrh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zfsnsipr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3txvexshn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cfsuptsv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xcareoah.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bgvzsbxg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lvuhblqy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3aogvjdtt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sbwrqlxs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bymtamft.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ewgoidpq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3umspyfop.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ondhylje.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lzmalmbf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3afrvtbqp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mffgpsri.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3oquwzrvw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ryyyeias.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3njdeynss.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wtcsygav.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3utnpcjkw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nwqvacvz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nyfsygkh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3mflmahqf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3etnhgkkm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3iweqezxi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzpdblqw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gxtltjbh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lltagcfd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3jsslnpgf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tinrcqoz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ctuokrns.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fqafjsep.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3dskwgfdk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ukhebqfp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qtqniaus.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fzmnzssy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3iyuunqpr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rsqiycwy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ugujszci.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3iaaliqud.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3siqejwah.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wpsfeauf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3xhgaikmi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kfgoicia.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ublwrkmb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3feipdyzz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jijmqkli.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kuqsbqln.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ywfsawpi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zxmkljkj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3orrfdlri.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lbakvmcl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hutonoqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryusgusz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3tqwxiyow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avbmbaiw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xzispwlv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3smbkvrmw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3yopkfhso.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxbtjbnn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmsbddrn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hhrjxtwx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qsqpvxcg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gwtjfiwu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vdkvwdfk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qbvqjkpb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yhqdgnat.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mdduxelz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gxybqdkt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zkjsztgs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3emxckajw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kcmskmow.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mpyzturc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fltodkwq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rlehfmvp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3baaohroq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ybmkigka.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lqdcvcmc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sdkooozh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xktonorb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3brmuntdv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cthoyphe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kfvdgryu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zqkmyqyr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3damwmbfj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mmquclaz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wdllquqg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ayongzfp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3knkakmkg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3oasjgxyx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zhmishxi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nxvroyok.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bemsjjxv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kilcoznp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wgxvxmph.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vacpghga.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eibsdpnk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3szqusrgs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhjppjth.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yzuapedg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3afgpqegi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3iywpklip.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bfsevmed.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mszvlltu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ajofmcyz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oyswqguy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vcxnnsnr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ttuhztwg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ioyibbip.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dbkgeziu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hekuhhgx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hwqvjdyv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rudayant.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uanvxedl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3umgorsyb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ufkolkls.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3djvatilk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kgdcilxv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lodufwvx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3sbivxelc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zdfksszm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pxnkskii.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3skbinopg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3phskgfvx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3otgyvidg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lirsgmms.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ibdgussr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ptxtilvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsenqhtu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3njrqwpsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmuwwbpm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xwvdrcma.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zubcwenw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ikbrdpwq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rwkflyyy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dmvrvlcq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dxtnmvzo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3foyggugq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fetlmiik.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwuifsik.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wpbijldo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3chmjamlw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ezzombtf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eqtggrfv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rfnhioqy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3uxkqxzjb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tnlpwlqn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hrugdpok.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3usblxtrx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xepdfpvm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3azukppuu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3lkugfsnz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ilkjjknb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sobvvecv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3henyqssh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ebumugve.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fymdulei.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lkmtmnvq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ezglnfjx.html


<!-- 参考信息 -->