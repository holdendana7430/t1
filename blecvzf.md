代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/grnuctqve.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fanxiaobao.xyz/Article/details/gpvhnrrzr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbwbdmht.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gduqmaimq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fanxiaobao.xyz/Article/details/gjwaoqesj.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fanxiaobao.xyz/Article/details/grvhqsena.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fanxiaobao.xyz/Article/details/gkbpoeqms.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fanxiaobao.xyz/Article/details/giplqmgxg.sHtML

[J07] 比较两个日期
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrsiplrr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gcfzompgt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwhlkcya.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fanxiaobao.xyz/Article/details/ghjentfww.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/gwschfhzc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhlugpio.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gamuuapsv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwvtsixj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhssmtiu.sHtML

[J08] 提取年月日与星期
来源：http://baike.fanxiaobao.xyz/Article/details/gvrnpcjvi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtogzzoxx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfhoptcg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlxdyvgr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fanxiaobao.xyz/Article/details/gkxtjbszo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fanxiaobao.xyz/Article/details/gltchzejv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fanxiaobao.xyz/Article/details/gyulwyuik.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjznrygt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fanxiaobao.xyz/Article/details/gpwvqeqha.sHtML

[J09] 时区处理
来源：http://3g.fanxiaobao.xyz/Article/details/gixefmgew.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fanxiaobao.xyz/Article/details/gbnfbjdmg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvahpojjq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gnlzovqsc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrtihnir.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcvwangl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fanxiaobao.xyz/Article/details/glexptrrj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fanxiaobao.xyz/Article/details/gocitodle.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fanxiaobao.xyz/Article/details/guqjblhvi.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtzxflgg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsrkfcybp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fanxiaobao.xyz/Article/details/gurtleqre.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfmhcyvo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/grbzuskfy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gctytasfr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fanxiaobao.xyz/Article/details/gxzpevpdh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnaermxp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmsylxclf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgepdbny.sHtML

K. JSON 与序列化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbccukmit.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzswsxhm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwprprlll.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqewpwzsl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gshwqnmbp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqnzsgnd.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gvstikxsp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtekgadg.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gccqajwdp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvponshld.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjnfiuyg.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fanxiaobao.xyz/Article/details/gjtyehuet.sHtML

Py:   json.loads(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkqzvvzlo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fanxiaobao.xyz/Article/details/glklraecc.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gouvejovi.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfrlpqns.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gonqswnmz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/gmxfxnmdq.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcersmab.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gqtdfdieh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnpaceth.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkghnbgs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gjnrtntrw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxriqutd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdrubotao.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatrpkask.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fanxiaobao.xyz/Article/details/gpbgsafnj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkmdjlyd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gfojqxmio.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fanxiaobao.xyz/Article/details/gefflheaj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gstndzfmr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnwlpens.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gjcmplvii.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbhphzdp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gnlaheawx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/grfyhpgzn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggscpcgyh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gncjjkeli.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlhrrrcx.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzeleokm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlwtcppr.sHtML

JS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gsbnbvjbj.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goofafiqd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczythmjx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fanxiaobao.xyz/Article/details/gazlxtzsp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gdjjycsgo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fanxiaobao.xyz/Article/details/gkhbveuqg.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fanxiaobao.xyz/Article/details/gucjgzvjt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fanxiaobao.xyz/Article/details/guhmyqhnc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fanxiaobao.xyz/Article/details/glvhajrep.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gguyoisld.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gomruhnsi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gutddspbs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuovtwap.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfabhaga.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/giqkfucow.sHtML

[K07] 进制转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxjdtfgx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gmjunoxns.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fanxiaobao.xyz/Article/details/gpagbwkef.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkgfsnwz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gfbsipowu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjhzopys.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/giglobhgh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwewcpci.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gaofxhafx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fanxiaobao.xyz/Article/details/gryvogtvm.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gmgzxaauu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnikbwwwh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gyllzwuks.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gfupxfcsc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/gbefgczzt.sHtML

Go:   encoding/gob
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxxcprdc.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gtafqolrt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/girgqlicg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gyjbpzmow.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/gvpxhdzzg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltifswwx.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdokpgcun.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fanxiaobao.xyz/Article/details/gymsyvjbr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fanxiaobao.xyz/Article/details/gysiasvbh.sHtML

JS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/goectgchg.sHtML

TS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gzopoptkm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fanxiaobao.xyz/Article/details/gqyhzumbc.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fanxiaobao.xyz/Article/details/ggensffso.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/gpzsmqdaw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczgdbbkn.sHtML

[L02] 发送 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gqocvupsz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fanxiaobao.xyz/Article/details/gahrexwso.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fanxiaobao.xyz/Article/details/gamnvedtn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkdubowg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gitzpptnv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvkteimu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gmwfnyfnx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fanxiaobao.xyz/Article/details/grhtyhuji.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gibuxuqpz.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeertxmo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fanxiaobao.xyz/Article/details/gugotwjsk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfquixam.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsrgzawn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/govsauqnk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fanxiaobao.xyz/Article/details/gddyzwpty.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsflzsvlw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fanxiaobao.xyz/Article/details/gaingbssy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhaqtnce.sHtML

[L04] 设置超时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrtypvbq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gosmfrezm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmgfzaik.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fanxiaobao.xyz/Article/details/gsxmtxvfq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gtxldzvie.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gaupwyrcx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fanxiaobao.xyz/Article/details/gpnwyeqem.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fanxiaobao.xyz/Article/details/gjjzeqmll.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/glpjqgsuj.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fanxiaobao.xyz/Article/details/ggvpdifgy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fanxiaobao.xyz/Article/details/gudmwzjcx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtslitgo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gftwgjwsc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fanxiaobao.xyz/Article/details/gdivpdnfb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fanxiaobao.xyz/Article/details/gnlfexukl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fanxiaobao.xyz/Article/details/gumntkins.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fanxiaobao.xyz/Article/details/gzspaxhrv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gzgrrdvdl.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhrayvpa.sHtML

Py:   resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gungaapfx.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhxnuikg.sHtML

JS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gfmmxwghm.sHtML

TS:   await resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkbzjfvl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbrzhawr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzeqoyfm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fanxiaobao.xyz/Article/details/gjsfmxjth.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvrkvbug.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvwiaoqz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaomyxhk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gjfodnmxh.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhzdtwye.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkzpgtrh.sHtML

Java: resp.statusCode()
来源：http://read.share.fanxiaobao.xyz/Article/details/gecwawchb.sHtML

Go:   resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/gmrubdueh.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjmlpgqv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhehlfgi.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmxsglck.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/gqppsadaz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrdiakjj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gbozpllbr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/glpdexpyq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fanxiaobao.xyz/Article/details/gevrurcgz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknajydtv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcbprwjf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gmxrizcyx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjppdlfja.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gcslcpwkv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gporodbdf.sHtML

[M01] 读取命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gxnroscgm.sHtML

Py:   sys.argv[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gycespois.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcokmgzln.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcivughyo.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gndjcbpps.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhvzxqwr.sHtML

Go:   os.Args[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gawhcwpdz.sHtML

Ruby: ARGV
来源：http://3g.fanxiaobao.xyz/Article/details/gtazbqhyz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/gwypyhehm.sHtML

[M02] 读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggcbbbthf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnozakfvc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gpzrwfjgt.sHtML

JS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlyyynrq.sHtML

TS:   process.env.HOME
来源：http://www.share.fanxiaobao.xyz/Article/details/galwwywzw.sHtML

Java: System.getenv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/giyveagew.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfampuszi.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtssashvq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrdvlqro.sHtML

[M03] 执行外部命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrzwgfsq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsocskxxh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulwveocq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/ghuroyqma.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzotpmey.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnugrozb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtvxbxle.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibufiazw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdughebeo.sHtML

[M04] 获取当前工作目录
来源：http://3g.fanxiaobao.xyz/Article/details/gxqezmrms.sHtML

Py:   os.getcwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkmuilrz.sHtML

PHP:  getcwd();
来源：http://wap.fanxiaobao.xyz/Article/details/gzteahyvk.sHtML

JS:   process.cwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/glkvtzogt.sHtML

TS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gezhxejer.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjghsasz.sHtML

Go:   os.Getwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctjqardg.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gnreaxolj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbpqezkt.sHtML

[M05] 设置退出码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfzxwrdo.sHtML

Py:   sys.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjujibimv.sHtML

PHP:  exit(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcgxaxze.sHtML

JS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmpqzlcgm.sHtML

TS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmilnese.sHtML

Java: System.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gstyumvnt.sHtML

Go:   os.Exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdyeaeyq.sHtML

Ruby: exit 1
来源：http://baike.fanxiaobao.xyz/Article/details/gcatjbzwe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdankauf.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyelscqqn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeoulzdl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqyayldv.sHtML

JS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcsvvuvp.sHtML

TS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyingtfsf.sHtML

Java: System.err.println("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gtkmdksfw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehevycsc.sHtML

Ruby: warn "err"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdunoqdc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gjxbfmqot.sHtML

[M07] 判断是否为主入口
来源：http://3g.fanxiaobao.xyz/Article/details/guxibizhh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvitgfmnt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrmzljlr.sHtML

JS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gonnepxhh.sHtML

TS:   require.main === module
来源：http://www.share.fanxiaobao.xyz/Article/details/gnevmoavn.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqagkzrli.sHtML

Go:   func main()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxhqovwx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fanxiaobao.xyz/Article/details/gxklrohnv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/glycciaxr.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/guwqlsgks.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gocqdgylx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxewyrmlg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhpdfqvi.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnemeexaq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fanxiaobao.xyz/Article/details/gwzkdlxlt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fanxiaobao.xyz/Article/details/grdfbiofe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fanxiaobao.xyz/Article/details/gplypzlda.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnbpdrop.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdizlmwdz.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/guqlkweyw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpigrefbj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvndcjwx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gemvuhzay.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxwmmjog.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gxbpgmffd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzejdoxj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gconsuukv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfojdtpd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fanxiaobao.xyz/Article/details/gaujtkmee.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/getrqzzqk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fanxiaobao.xyz/Article/details/ggktpulct.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbllrzsq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gslgtilqc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnkbfjbv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gncqxqtde.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fanxiaobao.xyz/Article/details/ggzfgfjjk.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmkazusfb.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gogvserqt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gumhfxusc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsalikiky.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/grpzvxlzg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpncvsqj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqczywfr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvgykxnt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjyeepfy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbpwjayr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gsehxbzvo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fanxiaobao.xyz/Article/details/gcrvjhuwt.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgulsxox.sHtML


<!-- 参考信息 -->