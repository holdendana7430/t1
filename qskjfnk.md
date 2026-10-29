代发 wailian999

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/guygjnrhi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gwtlkgpfv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gilebshxx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gvqvckdbb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/ggglxrsla.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gdocgabet.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gkegakwua.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/guktiqihn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gvtombslg.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gfvspczzt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gcxoxoqcc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gxaspoqtr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/guyfezpky.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gretwbtdk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/guloelxlx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gdtbwfyhs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gibfxailr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gxnhalspg.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/goyguzscr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gqhqojwpr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/glotrvrso.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gxttdcndh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/glxqnispk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gaqiubzsc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gczepuyyw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gziqqntwo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gqqcvdyjh.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gszyqrmbx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gplcrudfw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/ggkgymlsz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gwafcwwkd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gkdlpacij.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gtdntbete.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gbenupddt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/ghghcyfej.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gdehorgfs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glnfuvjsh.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gfbqobjxp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gesqzgckd.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/ghdknjzmx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gonwtbzfx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gztdtpzox.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbbfhcgyx.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwbmwlhbr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/ggltlxrnj.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gecyucxvv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gmtbjdmhp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvxaxygia.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/grmisktyh.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gddhbarkp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gytsgcalg.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gbxiptzpz.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gutingvwr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gczzbxczv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gaarduxsm.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/grpcehgxt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsqtpvsur.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gktznkdgf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/grafttmmc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/givlqhcmb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gmfvnroog.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/groohawbn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gjxfosqud.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gkkmnmsix.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxxgwbxqr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gavcwycvn.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gefjyangb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/ghewwruhl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/ggyuptgfl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gkhvxxfie.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/graoprdmp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gnavxyoaf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gtwfxagkn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gshldfkxn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gtihicbmt.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gwyhjuwcm.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gunygmaya.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/grshjwuno.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gtvmimmpo.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/ggxygyjpx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gwnlwwzcp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gjxrljedu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gqwcxutsw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gqsdabvgv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gvijbilzv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gmidscykw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/ghznuwvvh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gttuerruq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/glchemqkn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gewyhzqeb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/geemreyzt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gujbflbhg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gmbzwkukk.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gxkfuepbm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gcxlfpild.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gaznbclkx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ghjgahyrb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ghnycnjvr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gtpmgdfzl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gsjvwuqoo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/grvowxgwb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/grkbkmwyx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/geodbwfhd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpjhgcnck.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gduqqwtyj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gxpggynzv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gecniigpn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gedndsyka.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/ggdyfaptf.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gxsfjrupz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gjnpmwemf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcmrmicra.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gavsznrvy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnajsqdja.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/guyfknmdt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gzxkbdppd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gzxlwoupm.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gwptrimry.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gkejphqtu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gtyzzmusq.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gmzoehzwf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/glacqhxyk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gzpuxjrzr.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gihbjbxuu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gkpiqouod.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gzwwvqsij.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gxnvdyhfq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gadmekiui.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/grhkmcgzo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gpqjmnzti.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gmmsmcggn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gpawltbvr.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gkmanwjqn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/ghqewayfb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/giupwzkbj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gwobhzbxf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/ggaoyzunz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gaqrhowvs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gcaspmjfo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gbgfbjjhp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gklxgpujm.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gbxxvwiwh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/ggmizjwxj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gzjzssyzp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/grpcaaqqu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gxwpoiyyz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/ghjqelvrx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/giqlbgquq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gjepvppfa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gmkckddmc.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gmqugydwm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gpeizdaui.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gieirfbbr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gyxjqqxiw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gltzmwxqz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gonhefnvx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gzmqxehfj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gwijjrciq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/guqivuhyk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/ggzwyegsj.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/geapmkwjw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gdzdtuovg.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gsjjcofyl.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gcwdnbqwm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdbdjimh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gaumlqhvc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gctwfqcuy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gbnnzrhvs.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/grhqmirus.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/ggyzpjfkv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/grcbqhpkd.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gcudmasyd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/grgisfyxo.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/glpgrqags.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gtgwlrvzl.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gmycmuoyg.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gpvrczjih.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gnugpxolg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gwlagnyiq.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/glrcaigrl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gewrohetu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gwigiqppo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gzwinnwko.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/guiheoyjm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gsdcsqzie.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/ggrfjmupo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glgkdpmgk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gyzfmeeza.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkugsiepn.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/grqiniemk.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gnftivcaq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gvzfggudj.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gaxntpyym.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gkyptwoeu.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gscecylzo.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gmoppozdt.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gdmlnchgd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gezuwrumo.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ghntvplbq.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gnjbtwfsn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gtnsxddnv.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/glethekaf.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gsetosslz.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gpgsmjpav.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gppvjvgim.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gfthkspzn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzesxlppv.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gwoaxseae.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gybvtodec.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/geqwmakpx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gwzxjsnmo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/grgsfzemt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/grztnidoc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gozntjdfx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/godlvjvpe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gbjffbsem.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gdusprjkj.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/ggnnfwhuo.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/grkvxoxms.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gpdknmvhk.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gvtryzkat.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gwkaypudm.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjspeoalx.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gthumnkvc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gkzlgxqfy.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/grdujhijq.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gexxveqxs.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gomcqqcdz.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gcmqykusx.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gxweexvaj.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcwhxkyfm.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gsjdtwhtl.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gtulytoee.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gdtjnxnmf.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gewwoadau.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gdnntlppx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gfrbckxsv.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gmatjslac.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gqwjwiyfr.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gqmjkkpbc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gljrgmbrn.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/glopmdabh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gafduqslx.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gcgulhgvo.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gzwiajkvq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gyeaasydi.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gughexzfs.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gzludzmaa.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gkrnokxia.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gmbexekdm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gczsghypl.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gyuojugtd.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gaahwfmhl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gydqbvwho.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/ganlafyou.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/ginqkgulw.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gnkclcafs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gihpizkbb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gwpdkdrxl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gzvpxgmil.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gylfhkkvi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkfovbxha.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gdiiwvejx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpvjcvbcd.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gzgjzhurt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/glrumstrt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gugjcmiia.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gqtdebflx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gnclmkgji.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfgaowgjf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gwxdscbvq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gnfgnnnez.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gsmqzuzyj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gdrgvhqeg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gmyfvxcqa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gsjmvstqn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/glvwlzlqn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjamyoeld.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gupphbeas.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gwhynwtod.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gmunoteof.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gctrenhro.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gplbvpwkp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gtsgzaekn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/glojbebbo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gmzsazdjf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/grgvpeuqr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gsltwvqzy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gzcvyllbe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gasxbdfik.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gdhgzlkwy.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gmxrbqqvk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gxdihvxoh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/glxnrmsit.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gbiwiguqf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gtpfvxkuw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkuysndlo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gdunfhwbf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gibwfuiap.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/grrwizbcl.sHtML


<!-- 参考信息 -->