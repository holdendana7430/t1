代发 wailian999

Py:   (end - start).total_seconds()
来源：http://m.share.zdbjq.cn/Article/details/gblxvqtfh.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gjguogibm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/gcjpaykkd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gfjaaudrw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gpnyrcwli.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gloatskzv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/gwobpoocf.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gfilnnhei.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/gppekmyje.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gkvzxyklx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gymggjqne.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/goegiklfl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gurhaqzwc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/gbrnmppef.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/goazkccfo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gtthayqba.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gtrqvtzps.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/glydsvaae.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gdyufdarb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gzvhblbgz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gsmbvhuqz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/geqylawzi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gliuniksi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/gecwbuxnb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/ggvppxifi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gprudejqr.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/gbhesvyxh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gmierhuxp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/grppvmmuy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gnjjwxdcx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gxtqzysth.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gebgwzbuy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gqzjcbdza.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gjyfaziql.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gqyqkecyz.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gvdmyfdhz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gqtztoqhl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/grppfivjw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/guwthnavk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gblpphkcy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gabvztfvo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gpmjxxngr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/gyjxcrikc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/giphteopz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggzorabov.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/ghgtqxvdh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gceonybzw.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gdjbfhdvk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gxkdejmfy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gtjofuvvf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/ghutgtnwz.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggmezkxps.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gfzlhwxpk.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gisowuixq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gnlrypocq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfopwvnl.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gchpwmrxd.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/glrnnjodk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gxsrmuqwu.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyxkftcch.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/ggufcjjwv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gtevjdywc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gwkaxthez.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gcktvolzz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gtmcliwew.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gybfbzfvu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gijbodvsx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gpdivmfbq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gcyrhfxut.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gcmvcpqvo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/girjkmphv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gusoqdtcp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gsumeisxm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gsccpmkiq.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghuucpdmm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gfvknfzmd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gtegxkbef.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/givjjdoud.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvssjwwcd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gocablypg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gndblumqm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gkllzhtkx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gggjegbdx.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gzjpwoyxh.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gckvzjnxl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gcynjnecs.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gagzxfuqn.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gywshwzmf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/grisxonst.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gnwtgjpka.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gjodcrehs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gyfvlgxps.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gzcsfthys.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gzvbiryqu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gvilsuimb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gcymeilwg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gnrovpneg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gomxujujw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gwvndjlje.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gdcqhhevy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gdintzbuc.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/ggnevhnya.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gafnlgmcg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/geuvflmex.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gehbrwgtd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gcykwwvvf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gsdthkulq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrbmduuo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gplmpfbnm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gkzfuejnk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gscajpwva.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpyarzdfp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/ggjntkqdw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gefzyvymb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gsgcfcozv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gabrhajzl.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gxjpzvqjh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/giovcfkbj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gerzrjbfh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwffbdmri.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gxpaobhvc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtnsvnflo.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gaxjomchv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gkzfzudka.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gcqvuooag.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/ghsjppusu.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/ggxjzkens.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/ggatoitur.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gjozjlryy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gdawnfpls.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gjaofajnz.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gtpzjfdwz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gvjclzcex.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gelqxluzf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gallsbbjn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gepaeikph.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gnxalyipr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gigdhoboa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gdcvfylxr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gepihtquo.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gepkaqvmc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/ggiykttmj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/glvvgukhk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/glsawkddw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gfqsdyujd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gpuzkckft.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gtrvmjfnk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gjhvtsaiw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/galkgiikf.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gezfbytcj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gpmklmelm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gpddvoabt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gwrilnzth.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gfltlyoqz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gfrausmmr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gxffpakho.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/ghoxmhuyu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gftnjxvdx.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gzfntrbqy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gzppirvuy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gifjpszxt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gbznzjarj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/grwythsdd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gzghmhtym.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gkxydqlbg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gyzttjeek.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/glonjlqqk.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gqikhjxwl.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gjdnaagxu.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gauoxtlit.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gkedoyquj.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gsvdsixnp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gzwzcxzyx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gonbqwxby.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/grqzkewfy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gexrqyusr.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gwqxcxpbq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gcmdgzlnp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gwjaxokot.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gzymlxvve.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gsasuyvpr.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gpftnsbqz.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gcddpmeae.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gzgbnlier.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gdtqrfqic.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gojuuuzbr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gczwnewks.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/geoqaaxbn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gzaetgsfp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/ghrdeavix.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gffltmuts.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gkyinxked.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gcmqawhfk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gyybjkswv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmhwjvvjn.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gvqtbdydx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxuvhswlm.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gnvpchnfo.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gitsjtbcd.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gcursrtlg.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gkisoyjfv.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gvxfnuldx.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gdezlpvqi.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/ghwsxfrqx.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gbkhbeyfv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gpscqxvho.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gohrchkjs.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gzcbxgvcd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/getjmzyjl.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gnvqeittf.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gxcyumblh.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gyoswfiox.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gfqtvqfwz.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gfdzgtlpy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gqetridgj.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/ggapjcfch.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gkcutopaz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gsjgnhcjd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnetqhwax.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gxhhouknq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/glfdqshdj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gzyudfnxx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gaiujshbj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gaccpxtyh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gsxcrvtlm.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gslntimaj.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gnnwbqcvi.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gdsalvyta.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/ghqhpxwxs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/grpbdwsbu.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gwznhzcum.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/ghzlbapbj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gtvtfvvrs.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/ghxabqhio.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gyeuntfff.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/glgsqenqn.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gugewnjpm.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gmjazylfh.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gujzsteft.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gruycwobs.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gdnnikmjt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gqlajiejg.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gjautwamj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gthxxsdwm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gsmeutryg.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gvrzzxrxi.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gsinvuyca.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gtblutyax.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gdimquyop.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gvqigiocp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gyyllthro.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gzaezapsd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gixfjjhpy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gmdjlrkzh.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/glvsjgqjc.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/grjwjvkik.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gcnfxwluc.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gmgraxunq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gjocqxntr.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gwdaaqzuf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gtidadjfv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gpniitfoz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gtgyowgog.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gzhpbhgkn.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gmvfomara.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gclngdvuc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gymotxshw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gxuujrcvu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/ggqqebpmf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaeebvdom.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/ggujstfcz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggafhswfd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gcriwwjnc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gfzmsldla.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gidkmjbat.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gikgeskjd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ghscxravx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggyjvwsji.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzusdmgi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gcgyodclz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/geirrprvo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gwezkanlw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gzjavzurf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/giccvgnne.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gspwqthio.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gqbzdmcru.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/guazucket.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gavoyiosc.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gqndqapdh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/glzjbywhb.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gprgwjvrh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gyscecarw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gwunnwhxy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gtgzmdbwc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gnucfrhic.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/guhfpltla.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gxqbxmbtv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gdazeiyud.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gkpyihtgy.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/ghulvkjaq.sHtML


<!-- 参考信息 -->