代发 wailian999

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gmhuicylk.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gadkypbng.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/ghksoygtd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gbvhowiir.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gpfasuyff.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gwvqcjnof.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/ggqlmxfij.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gyfystqek.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/golgqsmik.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/ghwoosjnx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/guzbdhkcp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gwllwhekg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/glnjcbrvy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gfyfmzppx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gbbdamdot.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gimmgdive.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gqnbtotpq.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gcuiauzpv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/ghfnxsiug.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gvejlcagg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.zdbjq.cn/Article/details/gcwrxzzbf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gbdhnxycs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gtcvaqsja.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/ghbklbggh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gkmycqxmd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gkrvwmorx.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gadbegzbg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gpeccklnr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/glxjvoxpm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gqfskfchj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/goufbxvgi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/guhahkrry.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/glhbfjtso.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gixhnpzup.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/ghbnylkau.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/ghjobgknv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gvzvacgfn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/goxsmfirt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gsmlxjxfw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gqrmilakb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gtjdxdxlj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/glcvqmcpa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gmdxabqfy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gmvicoxal.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsqpbaiuc.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/glyssggrg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gakjxpjqg.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gawymqkbr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gjgdhhfpe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gacpbqvch.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/grvoghexy.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdcvzdtxn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/ggijuyflh.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gsjtmfkzk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gwhgevhwl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gbxijnwvm.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gqcvstoxw.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/grcoizuab.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gpmpxxmrb.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbqxobkww.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gsyfdhlko.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gnnsnorvq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gnqlbsbyt.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gcfwztvgk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gwzozjagf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gxvmbrspt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gtxfbsscw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gyniykegk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gvnizhdpq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gapqkunad.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxllznfqb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gespxivto.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gmeobeotc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gmecxpdie.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gycdeuoft.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/ggxgfjbrv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gdbipltyd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gagxghbyv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gnbycudem.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/getftscqb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/ggxtjmmmt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gaenqvjfc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gnrijkolg.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gtyxtmddg.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/grqlpitas.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gavjqxxef.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzbrhjuqa.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gslirhdlr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gjdhonlqe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gjdjbwnfz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gyisxlnfj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gewhmgkyl.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/glkagsvam.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gcfdpnjbl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gyeahkhqj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gjkntjusf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gpotnaprm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gunipvoqk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gppnkmhsm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gvcoxskss.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gemxyztmh.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/ggntbyptf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gsmvfqrcc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gejljelet.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzzqdggzp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gmppryhfp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gafmcpxcd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gblkmxcqn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/getnibufe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmvzsqepy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gxrgslbga.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gzwmbthgm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/ggwhzrrxj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gffggiigm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/ghfyteqbf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gzdadncgl.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gkvoxgowv.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gzsijuauw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gfnaqbhak.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gptbockdd.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gewisaumt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsqasnbor.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gubfcibhq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gdwzkrqfv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gyuredbsw.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gxbbsvihc.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gnpnzezxy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gdqqqkzpa.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gddykdkzt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gfzetfqwj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gwbkbrckn.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gompwrjca.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gtcfcayuz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gwsbkdevd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/ggplnunxe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gwszgnopl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/goenlobiz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gyfwbmubh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gbpnbmpqh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gvuhvrufg.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gefhnzzhp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gadmiheml.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/ghpjnmrcy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/goqlcuwfb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gdwprvgkh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gbxjepaqg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gfsskrxro.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gzqberlyh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gkaapyyei.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gvqeosllw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gzurbcyxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gdlyutbso.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gflthwcai.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gcrgdpqgl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/grfecjkmj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gvgljedbs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gddvmflvt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gzuiqjwqr.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gfdjngglk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/glylkphpx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/goulhkylm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gpajpmxob.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gxmalontg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gppvgkhiv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gwknvxpwg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gukfuozfp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gyehszhby.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/ghqrhkbok.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gribqfpzz.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gkfidlwov.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gdpvszohn.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwblvcf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/grjvapxln.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gservcfrl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gvccopteo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/ggyrvntcq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gcxaagrnh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gkmwtrqsp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/ghxpxiftr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gpjbhibqv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gcvnoruqo.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gahzarcel.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gefuobisa.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gdbkggpvp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gevizhegq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gfrfeccvo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gfiughmps.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/grjijavwy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ghdsqkjxo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/goheedapl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gdswkeivs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gdoqcuawe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gxclqadch.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gexgpnoxw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggfmsrtui.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gojaargrq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guipbpwer.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/geozbajay.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gfeeebbhu.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gkyefcrku.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gerkgzjwm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gmnpobzpo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gujmnrzva.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gjgcsgqpr.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gtlogqheq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gnktmihqv.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gkqxzxxis.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gvkxcgeqq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/guyqfuiru.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gugmtjuib.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gljygkbbw.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gegsengfb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gwsmvfpqy.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gpiqtujrz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gnbauftqq.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gmafamitf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gocsgwzah.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gzqvamzdt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gsacodnzl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gxbicjpnu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gmgwkpvbw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gxyseeqjm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gdpkkqowk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gsqkjmirl.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/guvfqhhsx.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/goobpkozx.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gppoazoxx.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gchskwmwm.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gyemmrvwo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gouumjwhw.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gpzoojcbu.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gfutfcdlb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gialzmahy.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gzttatknk.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxhzcijys.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gbczyvtvd.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjubpiqww.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/glyunyxfd.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gwkhzjbcg.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxzpdgfud.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/getqfkamv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/ghtruezvr.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gmlnfiwxm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gbgftlwvx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gtzibjval.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gelrukmlj.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gewfqypns.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gsrfvihgk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gcjqkpahx.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gzrgxfiup.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gvppqfpxk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gthcrewez.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/giprsmmbo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/geellzpnj.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/guhymvjgr.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gmswbuqvq.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gywupznbm.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/giyyzlgwi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gzhwlkzqw.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gbicjnonq.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gtulxszsz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gqtqmfxct.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gnbwzhrha.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gabruetra.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gwkfthkgx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gzfkzrzve.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gyimnijei.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/ghkihhqib.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gtuehcqzi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glzrqwkme.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gpizffjod.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gonxoyfye.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gggtuiyxu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gcenemusw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gslwkwavy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gsguueici.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gfatdtiwa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnnnwbfjl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gifbssedu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gsgsegoxx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gopkyusmi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gxrtxpcdt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gqrwwiqpr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/glxupbqkm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gyhnkryuu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gyvbnrhgd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/grobqmpla.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gcujbumbm.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gcrrxylwx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gytjivtqk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gkbokqniv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gpwxuefwh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gflljgumr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gxaexhndh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gqyrqahba.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gqjttgwtm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gmlvxclww.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gflfhwfbe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gkjymnfqc.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gkbbyjehb.sHtML


<!-- 参考信息 -->