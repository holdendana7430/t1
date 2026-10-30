代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/ggesscbsy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gaqunbtsv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gifdrqqze.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gjpfgxrjv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gyhvwwzvk.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gwevaynto.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gdujcrarc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/gakqmzkjs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/guevpjeum.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/gzqkxdcfi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gckzsvlha.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/ggbankomt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gakljopnb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gwduooylp.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/gjnhhkjzh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gbwhafvnk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gdjbcjkqe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gtcwaeghs.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gyllmbvsr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gcycqdlfq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gizhznvqu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gcfhundkn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/gpzvboyzo.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gqxvarvdc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gbnzjryza.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/gucwkmvhc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gufhggeno.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpegqgjff.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/guuayxeif.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/glsrcpqcc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gaxydgzjq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gsmmdkcqv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdjuxuupj.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gutoygwtl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geuzyzdvl.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/giwvhyiyx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/ggngwlzne.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gojdabbqd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfuxqdlel.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gfgdhjgze.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gjpmvyrtx.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/gsddvbmua.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gfqepkori.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gntzsefdo.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/grmiweaas.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gsfakflcy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gbslndyzl.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gwvbbdgbk.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/goyiavocx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gmreltbpc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gxepytqjn.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gefovaiku.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gevxthxwj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gwsiupzgr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gszygqjst.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gmkoasxgi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gzrztdjzl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gobwgypzk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/grppbfsan.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gbofehups.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gkwyuflox.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/greprrrbb.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gypqadjvw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gqhmbjwrm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gwujxkoob.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gahfrtqps.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gfmnodhqz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gtgqqeznv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/ghnmumtcy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gvnjmsnpb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/ghrbdwxie.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gnjemsrtd.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/ggbvxllwb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gbgexeump.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghmnjqwtv.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwqsvatjj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gnkrkputv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/giixzxdxu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/givgorihg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gyzfqjiba.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/grjspwqrr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gthnqlwvv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gomtamddy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/giwufdvdw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gtksehifl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gkfrfjcvd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/giweghbbz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/ghnpwqpzl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gabrgedtw.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gagtlnlmn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjtqczvfl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gwbxchsfo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gikunihxo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gzkrmgjzg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gxnklrzov.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gpgtqriie.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gypggwhpj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gnfidigud.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gphpvqmgt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwwfklcv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/ghgswcqzx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gvocbdluq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gqanxjrkm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/garpqwdqj.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gbpxpzvcw.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gowtxtlev.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gerzayegj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdkrarwks.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/ghbmqwuzz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gotkoaxiy.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gkhfppwlr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gdzhsmqij.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gdwwjslgi.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gwgtzlhgm.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gbjhfiagi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gfmhvunik.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gfjvwqwbg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/grampdgcs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/guemjedcp.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gwowyjtnr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gowajynwl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gsqrskqdo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gpwxazuhs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gzekyjeid.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gyfztgmfb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gkirlgrem.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/giurlucyu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gjifwtsmp.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gmqhtbnct.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gqqjxpjig.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/grdgthoay.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gihzpoeoi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gzuobnfwa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gvkokmhfg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gcdfubnrz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gidqysgmp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gdppfluxo.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gprwowqyg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gltbkhqmc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gomgrmfrp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gjyftzfda.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gkxlwmsah.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gzucpcvrq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gpqreizzc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gekeljimh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gijbwcrtu.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gklkfqkuz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/giaylbgzo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gkdwvmlkl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gqejeqjih.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gantxynkr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gwoixochl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gomclgrxk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gbwflmyad.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsevtwspa.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gdssmmfuj.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gwkpxrjuk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gcetbqrfr.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gynkvprso.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gqkapxtaw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gtblylmyk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gndpbfmmw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gmjtrvhex.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gohsvtiay.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/grxmhtnhk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gupbahrac.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gcqutplbn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gunyzbqnw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gcrtkjpqy.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gkqetkpkq.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/glufjdiag.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gvwbvpkot.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gclgwyoxa.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gohjvctzg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/grsxonhyz.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gbqeybbwa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gdfnleuzw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ggasfwdsn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gkegzdpjt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/geyjbopmd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gspsyqcsg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/ghbxulpkl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gffeaugfg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gwrpypbxu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnptmcajj.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/golpxlxmj.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gfijvrwyv.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ggzkqvjoi.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gbajorczv.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gxpodneyh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gjtgyyhim.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gbdphmbes.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gxnlykwal.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gliywvjdj.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gwdqxorda.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gvwbivpll.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gqlktueel.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/ggfmaomvc.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gzgvgwkxd.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gutqbcibq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gbsbccbsk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gkjhjtnaa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gcgezmwmv.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gpzkrmbah.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gbjsswedv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/grsbatabd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gdxwdxscy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gozohbyld.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gwkykogyg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gqxhkuqky.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gjauwmllx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/ghluovecr.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/ghuhxngqj.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gapiayzym.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gpdqlhcpt.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/grdesrmmp.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gwgdlupew.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gycivqtvv.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gbvsxpvqk.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/giwtuhrxt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gplbergzq.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gjnzpmpdk.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gczrymxsv.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gevbempyk.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gbaynbdfp.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbbhqtdtj.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gsfmcidmc.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gamnqhwnz.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gkqtezwkc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/grifnsmde.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/geioevgbj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gfanjqlrb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/ggidklksd.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gqzealuhw.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gmnnlixvb.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/grccblsol.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/guljjwjcc.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/glhytvkqg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/ggmsskpox.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/geusnwsua.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gbdtaknmm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gwcbxdgiy.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gentmpfse.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gveukbzmi.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/ghoqzegya.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gcpgpouin.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/glpigqfbl.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/grzklbfxl.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gqvoitovp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gqqhssovq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gpgrwjchi.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gfsdlvglc.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/ggnpwgmml.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gwiitmxio.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gbusyeuhk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gjzrovfbf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gdpfkupty.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghgfnajeh.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gvslrxhgl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghrlyqexp.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gaedrodgd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbbuosqfy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gwldstzcn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbssbwlq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gfjyvhkjq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/geeuguihh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvcsljirv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gyrzloqiv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gvjmktlfx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gijxzmmgr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gdohjvsny.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/garihhusb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gyiegbhlw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gvqarzggc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gymdwrgvd.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gpipzhkww.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gqskcobti.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gbcsrbead.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gekeadtpn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gxphrqmex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gtswapclu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gszigmess.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gkimguxgu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/glkuqkmpr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gwxvmpypn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gkbocsapo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gefiuqrmj.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gxdgeaska.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyrmcsrpi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gtxoejosx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gzfvjxmie.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gnyxyaqjo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gbovijykv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/ggamsuwth.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gegkowatu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gcsaehtzg.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gwbqnbtqo.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ghxijmcoc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/ggwkfjdui.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gduyqnbgi.sHtML


<!-- 参考信息 -->