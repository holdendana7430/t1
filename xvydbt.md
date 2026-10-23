代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3tugvwemc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3axnkmiqg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3hlsrsscw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3udthywzu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ttveiosq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3eisetukf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejwwojsd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gagerqpn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3eaurphvs.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ierfwkbo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ujldjdxo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3aqdqrfps.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3rbuzreid.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3zndpemiy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3uxtagouy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3dpdukebp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3wbenugoh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3xrqswjag.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3unplelbo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3bhvuoqad.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3kmjgoiva.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3omydjpjn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rgkrfsju.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3gpyaqvbp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3wosonqtx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3vdpbijar.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3bjmnctcf.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3kpwrmwek.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3rptreasx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3lxsaidxh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3mepviltj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ybghvtyf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gnmuvuqj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3vqzgzlac.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3qntcvgqt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvklhaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eswngwws.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3mvgrpbzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igiiwcrv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3bjbjwwxz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3flebmqyg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gokycbaf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xzxxjuvl.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xahdrnzu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ojymlkoo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3fpzoyanr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3squodvdy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3adhgbpwd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3uobtlhaz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3cztkznnq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3cfzwztya.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cybslzrs.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dtqumobn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3liqrdaxh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bywvrtcd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3krsknqol.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfeahgdh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3dppghyee.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yrycqecb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dxkdorsw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmjxioia.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3gdtjcoqd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3iakjhexw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3bwjaxlrb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3zehyfcgt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3fqqmhptu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3wqyaolhe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gsksdbln.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ttlkpkoi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3tjnsgpby.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qpthixyv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnxhjuv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bynpodok.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3czjadtmz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3heourmwt.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hdqevnik.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3etdujvgq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3nromoewv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vxnekdkb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3awqwvdla.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3jaercdsf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3lxqeraug.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xgpaqtcm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ungzpnfg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3svcwrgls.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wbaccemv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qcdigbiz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fqzlcquw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yexhuexo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3udumnafk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mgtksjqx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wifrnfbu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wpjhnfba.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3qwlffmzc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ctqnqmcj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mrwzsukf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bmmtnael.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3izmgrmtn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pnggytxh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3fmgmbuso.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ewrkibvj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rwjdybhc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3msbsoypu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3wmifysmz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3zandtahi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xufagcve.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yovdpcbx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3yegeswns.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3bwcayojn.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bgxixxbg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gronomkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqpndfrn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3extqkggh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blhjtwie.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hvygzjni.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3gsthuqei.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3cktknrjz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ovhidlbn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jlauobfo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3pusmxpmg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pzadestm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3kersmkku.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hzpngfhe.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ybpsdlch.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zmtoeatb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lebwekmo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xpwwxoqg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lqpxgunc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zsfrgygx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3whjxzvuk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3aukdciis.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uhrufots.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3xcjcxysz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3lrxaqoib.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3uodlpdmv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bcdsyqhn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kxqssptd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ouygfezh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zkoasrao.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ifzxcitp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jwvxgazm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3osdtupet.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3txctujtu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vidrvvko.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ifanlrpx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3imtfmdec.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jvxebuju.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qpvovctn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3nknfloda.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3nanqymwx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3odbfrmuf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cffwphev.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3gftdsszl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kqhuivcq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mbemholr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3kxuatqzs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xpbzgnlr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ravpwmea.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wpvikdso.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3gmegmpek.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rqsaoizm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rcnwfqqe.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qbvaeayf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nzluasgp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uwvplgbg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tgnbagps.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ejiqqczt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zdkhmgzz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kdygpznq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3bgqlxdwd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cnlygtav.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ntzbqmnw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yryknfee.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xexruuju.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pmrudmxy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qyxrihju.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ucdqupec.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3zceyonow.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3uxhtjtgl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zismuayq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3egxcettx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kcyflmgw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rrponaaq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3rmgxblal.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3svluypff.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bzwfqmea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwlttcgq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mcnkwrsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uovueksf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mmdztooi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nboohtxx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3isjepvnf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3prablhwq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lrkqqevw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3spthzsas.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mqugpzjq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3oxgahtst.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iwehvvlm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3trkvxhxd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3puzsfgrh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3oszxpose.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3szvzrmgz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3avuqhabb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mesfbfjy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oefttmtq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jbvacybj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yfqxkyxo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dtevcnqm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ubuseygm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3efhjbspa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mwytwcui.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gosorjve.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ieztkycs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fyhqhpnm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3sdfegozr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tpgykbro.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3krzmqkzf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iildcmfe.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3sbicqixe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kyikinbe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vetlafur.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3waygnjoq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mliwnapw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ydysahkt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3wkiggluk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jnfypcqz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qfljgxdr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zqaxzzsy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3enndvbon.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfytylkk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cqueedgq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3egauqbzo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ragrexvz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wwizgymj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3syrlwvxr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iwqpjnss.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3laevbeon.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cnsmqtwm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mlzdgziw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3vvyaygty.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dmpzfets.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3btpgflba.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lczukimf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3okmnzqho.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rbgmrurb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3usmlwgzl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yjlsnhrz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pgbvijuz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ycbtvigb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zebkczpz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xcnghvgu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vizflcjc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dlcwgzbu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3abihuhkx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dzdnzmcm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cnyvxosi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zvrxlidd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nbolmxbs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gvkvpmfa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3snriygwg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3undyeedu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbcnpiiy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qvcxzkyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjhortom.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dzgidarq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3espjzcgf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wbzpdpdj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ixlyogzk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tncbvgiv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oekwpwfu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ajcdoiqn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3fhtongce.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3taewmyna.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dmydyvpl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lzmujivm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3iddwbwjl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3axnchfdn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3taypsiac.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zrcrweoc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fkxaeuea.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bslbesaz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vfbavjvn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pdbxhork.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tofrwlnu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3chesikev.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jhezasrj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uoyqoery.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3iukgvodu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ogvykjsp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qjbnndjc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rwcfuihr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rwwxdspd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3midcxanp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ukntonhy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tsrndmca.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oqhqknjt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3izzyxcgr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ynbpdtvt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kvgackur.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rotgvyir.html


<!-- 参考信息 -->