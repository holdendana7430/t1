代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2rqsawuzj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2rupphzqv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2pjykqkqb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2medghwro.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2uxcizpgp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2dusbbdcl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2axzbukbm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2btgwdgvr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2qscpbgex.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qslpmfqm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2njauwkjt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2orgdwuqg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hncxrlam.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzfgaxwn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2vgfolcwu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kgfznnuo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qatkqhdd.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2attkstme.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2vnrjxzpt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2vupxevkl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2brqlbnnk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xizcadpu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2vddcwnab.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ikdahyzp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2xdgjancc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2czesomnu.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2snrfaukh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xffafihr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2veststwy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2njcysvdv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xldkeovq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2yqgidmqb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ghnczsnl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ntjxrwun.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2flssauip.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2blttuqmf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzglxjfn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2mbzcrdro.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2lmcubzcj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2myektnrc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yigvbmrc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2vyholrzq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2yphlfbua.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqmrvajy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmqbqltd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2fgfdyrua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itkwidzy.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tboiqswl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lzqhyqrc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mxalapum.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hfgjpbgl.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2subvrwbi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ntjfhnku.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pgstdeqc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2kmkcgfmj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ialcuefq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2lvzsvbrn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2zkzgvyup.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2bikmiiua.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wswpdlxs.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bzxfojve.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ddxbiwya.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fvqrpxwr.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uqefhfrg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmyvxwt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2mlwmmjsr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jxlubysd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dagwzgnw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ltbuyyfm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fbemmdcl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2yaymlptd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2goxblwwe.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bknrqisg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2nmynlkij.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xetljwkk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2qjvpexjf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2hbcspscn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qejdumoh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ofwhapdq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ehtlpdlb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2steeoszu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2oudxwipl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fpdglajl.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2fuxedjlp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mqhiiurg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2pbwmlimq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2monmrntd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2enajllpl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ygetxbhf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2kotygevp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kbwskqzj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2crdhhhzq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2zycsurte.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ctqzfwrf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ujpwwrew.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ztjudfop.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yfvfiljo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2yctttdkq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pjcklpbd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2txmnisch.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2obwkzdih.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2adxvhlpd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xuibzljn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2lzosmjph.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xdlyymrm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2olnvnkqg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aehfrbwh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2vqiquohy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nwaseoqr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2glbzywot.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2kpjolggw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2piufopzz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gbinysdg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2emxkiema.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gemefsgj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hggicxtp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2aicrznae.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qhhntphy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2syaugoxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edrjejzm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bgedtrgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlagcdxr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vlubdwqf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2djtxszdy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ghndrbgn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cswqrrkn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lgkjlxmh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jlhloqhm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hgoscbxq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ehqsojjo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zlggozld.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dezbsffl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mkijztcw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zsovlsfs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nnbjhief.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ebseatfk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zxyeysjy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2mjnbhjhw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2lrsonrnb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2opjjaytv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2odypytby.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mdyoaaam.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rzskxotl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zpuwmhvk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vmexwows.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2tuyomvvh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pptiweaw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2kzykfgnu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ugngomjm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jmuigueh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bphahjkx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2dowmsuft.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mtpgvohc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kxjkfxzo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ixxnghbh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2xmeqqajt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bcnppknz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2suvyslel.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2pvffqykx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2fchdvsjh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2nzekhudc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2edbcarca.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2exbfkwsg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nghniury.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ynvebsip.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2oluhssxn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2prysewrt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2djkodbkq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lmpyvvih.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ixcuqema.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mzlmujfx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2putruvnt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zsjgcpgb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2heohlxug.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2qvnqcrhx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2beivvbgl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xqxnnfrl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ygaslabo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2kquejzlj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gdyqkxyh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tfypwcej.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fejynxrb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ywjzzxaa.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ntcedyhl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ihuybkqp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2heouolps.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rihbhrpn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2axanercb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ivvricze.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ablisxio.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lduipcin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ihftvasd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ilktowmi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2xwkhqddt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pummlpmi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ayaclghc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mytgaswf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vrheuoaw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kgbfdcfi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zasmilal.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qdftmrcq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rlnbmwln.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2meltxyuq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dsdjzeci.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2otnawgjl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fsmubrde.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hocncezj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rglsgiwh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ovgfmleh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jsxonmly.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ewybkauv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2knlrinet.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fhycvkzu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2sjyhhnnz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iswgsabi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2apmbhvag.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pzrhltnd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2akqrwmsv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xmlxdefs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zbspntzr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rhceyksw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gpocpjvi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ltkdtrch.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mpuqsbyy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2opndcqkc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dlcstugi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ynlgwqoq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xckyvcnq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qkqgpodt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zsjbhvee.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pwtqlvpd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xewmkerc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2gnxqfblx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vvsjcaiz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rbahfofl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2saopcjcs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzuywmff.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqbmjhzt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xbjpdqdi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uvfofzxt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ckrmlcva.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nurrnltf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2tabmckqd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ioppaaol.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vfqingcj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ywbeuhjg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2moronujr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dgjknywj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qxrymghv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2meqyrkar.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xwmxzgll.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tdrttsky.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jqxkeopf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2bersydpg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tscuqjab.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lqbvjwee.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zdirzwxm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xaqdfahv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rzmoywfs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bcqybmgc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nhegairf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2loqhlprs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tonhixrg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jowechpa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tqrcnama.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2srmpyvzq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2molydmpr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ipdxsbwd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2faszlchr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slvnvgti.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jmlzepkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjtgjzjj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cjxvxmhm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ctijolmr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ocjwzjrn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2msrnobtr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ixbjxdvz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xfrultyr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2juccxqiq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zibecmuw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zrcgcsfh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rpdvmigk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vzbvndbn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ohlonqcf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2odxufaeb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xdfwwntq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dnaquufs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jalyfjph.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rwhxpxrx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2bhzlbjuj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rgrwrcse.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gbemukud.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2tmvwgrnu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rdtbhnxq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2txvdoadp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2redmveed.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ykghierg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2iihbfzhe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uycyytrq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tlgnhfiz.html


<!-- 参考信息 -->