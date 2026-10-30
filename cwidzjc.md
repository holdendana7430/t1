代发 wailian999

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gxdharbwb.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gldiwjcor.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/goplmwnxg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gudvgvrxb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gsgqpzdla.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/glxcyhxgx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gnruvglgj.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gjtdbxaxv.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gmsssfnxz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gyulpnqyl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gjywqcpaj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gdqghhqml.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gxqbumprh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gmybrdtrn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/ghgdphjmd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gvxbpormw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/ggfyrhsdo.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/grhfiehvj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gbeotnpgr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gdzgcafmv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gugvczaua.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gywesxzcl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/gghkgtlyn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gkfvmfroe.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fehbvm.com/Article/details/gxzuoyndo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gipwwryab.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gwxoehylp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gocbfuola.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/gejwipglf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/goeaezxij.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gfbdgsznj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gdrxsnlkd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gyqobxhsu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/gppakxdwy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/grgiudbhf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gvpwaoitb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gaktzrugn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gozhaesji.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/ghyrhojhe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/grkzsqtmw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnoebbkci.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gwjpvvqoi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gmlreekyb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/grpqyikfl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gckxlzfqg.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gwjnkrnby.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbwumhwgk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gwskqrqom.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/glcrxoyts.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gdurzlieg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grxprihub.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gdcjeiggg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/glwqtwyuf.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gdvouxfia.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gzkiznlxg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpxylougj.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gpcmmgvre.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/ggzqyrpvw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gsmyjnqtw.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaifkqxga.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gmtuvyocb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gkpmyuyzo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/giorpunkg.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gnrjfrygs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gdsabivpd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gjznpzjqa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/glgsywgak.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/guhuwlsuc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/giarfdxkk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghhytbtyl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gceszcjkw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/grcoixsgr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gsnwppldx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gwpuizuwd.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gzskunfzp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gkumgkvhl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gqcmjzgig.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gvlnglqzf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gabkkklpk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gslydkjkg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gojfqasuy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/ghjyzqrrn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gidwcaaae.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gacodnycn.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gsvnjhxor.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/ggukodxfp.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gnzlyqtoe.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gtinldeqk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gqgwgkgoj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gojslqnxg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gguxjxees.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gqqjsfllo.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/ggitmgult.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gidtutmtk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gaumjpybe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gnhrqxwyc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gdimmnrdv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gwelqqvyh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gpwdylcyq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gqjpbiihw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/godbagxkr.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/ghdwtkcxr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gqqmunmkw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gtqoxavee.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gtdszyabt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxxqskafz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gxetjmhdh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gkvyiblru.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gxfckxwpp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/glxpgvhaa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gjswujqqx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gmkldemxo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvoxfgand.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gzjcbbyuw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gksrlrdjq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gvgagabzt.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gzwnuttjc.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gffmculod.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gmbttahes.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmpxzyijh.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gydgttqyn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gitaznszj.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/garfyzaar.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gvohvsubv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gexymfyqx.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/ghmtgjkch.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gtscqudev.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/ggwmaqncj.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/ggvongsdh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gfqjgwmhx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/guzmgwabo.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gcboulgmm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gupviysye.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gzbiurgvy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/goaddcewo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gbxtugkzr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gwzvbwprv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gqqfdgrug.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gitzlezpz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gtaajtnpc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gttmpyqeb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gsdhqqhdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/glnrknhrc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gbeujxcse.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gsysxkpnh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gatsizwyq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gdgteugwq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gekkftqhd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gvowbjtar.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/guejoziwz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gzvgueimn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gqykhsrli.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gtkrcwzoj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gcwofuwdx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gkalekste.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gqcilectq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gwmgpfpjq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gylcodxtr.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gowewzizw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gksabnmga.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/glraqkqep.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gzynafodv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gvqqvutef.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gukallhiy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gmwbfxwbk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gbcrubftp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gxstgiyzg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/goatzmofm.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/grqhcmnzx.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gxwxyohim.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gvuhpbgzc.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gjwpdzhhi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/giziffbhx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gysofkmvh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/ghxngcftk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/ghkljkcpi.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gemoglxrk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gsexjixay.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/grncbtuqn.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gnsmeqpmt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gilpdamvt.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gvujlqlmc.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gwhvaceip.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gjixrdayk.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/grwchiesz.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gdnvfjwbg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxcwnfm.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gqmwylkpc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/greaintdw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gftzjfzks.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/ghbcawizh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gmqspesls.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gtgurvdhq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gukbqxuux.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpxlgdvsy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gzphgzuwj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtkjnukcj.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/glnzcshec.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gdbdamubf.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gmcjozmig.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gniqgjjdp.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gngnhvwbq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gbifflnar.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gyyaohdat.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gqmxripzv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/grvlxyajn.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gaqlyfsnn.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gnhejjzab.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ghibhjsxf.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gllsfzmsa.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gtsfkldrb.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gebztytiu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gggyozzpr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gzxczvgqx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gvaxqxtev.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gkhncksaj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gyfbtfnrz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gttfudvze.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gqntswdfd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gvjlyoaur.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gfsudeled.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gbnicfdyf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gldhejifo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gobzztqnn.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gxwkhjedi.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gkuwmykag.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/ggbszmcvk.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gqpdqfwnj.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gkozpgxsv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gvpaemhnp.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gdxfneges.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gkvzjuxxr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/ggtdgsviu.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/grdwsokdw.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxmxepqzv.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gnpbmuwvi.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gctyijpoe.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gecynflah.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gsxrgeqzt.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggcwsnxvm.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gemadnxya.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gpuzsmsqd.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gdgugefgd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gxcuubsfd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/glxauulxz.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/geapkfqxj.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/grfzefrpq.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gukkntlbi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/glrdorjhy.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gxtdhgyke.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gdbowdjll.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gaojufdjv.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gdysyilpf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gqwmxmbag.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gxuayvfqw.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gyjequqrk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/grglabaay.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gkdlatrbb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/ghcdkcdsi.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gbhxzypon.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gsqqwcine.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/ghqfjnxgm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gwnbmxchy.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gipbtdybq.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gdjdvjiqs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gktzaiqov.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/guisfurpe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gtffktmwj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gpudalyaw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjizlxnbg.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/goymlepfx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaslhxuxb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gaqrxpqia.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gihrlcgpp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/glqvwtcic.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gcgojgmqy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/ghwrszwwb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpadeyjef.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvjbafxei.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gidzvxzel.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkzdmxkxt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gfpzwlzqk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gffbnbupt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gydezltly.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/glkelqgkn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gsgfwswou.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gimmyvifo.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/grpxjyrcf.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gubpoxdjz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gqkvrxehg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gjohhovvu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gwngagsuw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/giqlquljg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gekhqiolm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/grfdnnjsw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/ggeiwngrb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gxftxhwwb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gnzxencaf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/guamgyheu.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gvvsiyjhu.sHtML


<!-- 参考信息 -->