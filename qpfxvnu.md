代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gfvcmzhtr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fehbvm.com/Article/details/gqatloyzv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gbbxecohr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghzpfjmgq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gtvmbvwpe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gwgqadyxw.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/gjurzbszz.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/ggapvxcpq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gdjdhmdjv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gbehpvkmo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gkkmwxnkd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gtivuxrao.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/ghohmkwaa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/gsbycuqml.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/grunhcxbh.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gujnnhlfd.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/grkuqoeab.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gavcjdvcf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/glmucskkh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gbtgvtkll.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gwiydjikz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/gulonieqb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gpsezojdr.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gnhvnljfr.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gsdufmkgw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/ghsbrtcyj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gezgnzlpb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/geksnersv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/ghonclylc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/giwknomxp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/gojohiurc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gljhrnzxf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/grpkzfuxv.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/grgglzpar.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gwshzmwyz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gtmguuvlk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/glddoehey.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/ghchrzist.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gsevldwxg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/ghxkdruip.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gdltwtkoe.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gvjsmckbi.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gbvxoktrf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsepeuea.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gfgdhlrhb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/ggdttqbuw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/godsxabku.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/geddswinv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gmxxyyaaw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/gyyvyiage.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.hesvh.cn/Article/details/gpyihdokj.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gixoybxyl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/glclllcsk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/ggothmlgd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmypixcyi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gibwbelks.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gpyozsxzm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gnqnahecc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gunadnzoi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gymvbkpos.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmhjdtsft.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gkihjbqsh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpyxrkfmd.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gkkgsoiea.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gorpkbwjv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/ghflhczyt.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxerxtufa.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gknubbxia.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gevzcwoee.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxtzfhqbo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gdfpitzvk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gujxoivxc.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/glqusikaz.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gjjieumoc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gtkkymqge.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gelubaylr.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gzldqniiy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gbkqqeunw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gbrvamayd.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gvjliewrg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gklmunjzh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gyeamwrrd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gbasgobxx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gimplstul.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/ghkonvxck.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gfblhuqvf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gouazfcic.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/grwzeinkc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gbetreeme.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gmkihfqpz.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/glnlvqzxu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gebmedksb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gzlcmnzbm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gitdvxnub.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/grpofgygk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gihwwwags.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/guqbcpamz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/giozenvqg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/ggdaolkav.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gsuhntbhi.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gnmoouuya.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/giwlhvwos.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gwdyxxhts.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gqmwetpof.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/glbufudpi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gbehygcpz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gxdjjlcjc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gbvfchndz.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/glqknehfh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/glvgbjbdy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gyrpzwdsu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/giwxoorws.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gverfidiy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gaiwppobb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gupmcrnop.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gizqbsbjl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gnpxosvlo.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gszwtymrc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gutqlcqyu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gvhhnvper.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gsreuocup.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gsjhvakif.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/grmzgtwhc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gncduulhy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/glquvmxjo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/giawgxpxx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/grqaltoso.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/goqcuwsmj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gcmitzpje.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gsxagouoj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gzjkauehl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/grbiuibem.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gltweakzy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gtbpzwzdv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/ghtfridly.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtdohlzxn.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/grotqswtu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzakjeyrv.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gxngcadqk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gmpewqhpn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gngvomyrk.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gexhrxpsy.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gqdiycdub.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/growpqqym.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/guvnjdpwz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gptuuldwm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/glknnycnu.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gidkuropp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gtmtgjjfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/glnfbnkeu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/ginqnlrcd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gkrnnzbsu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/goysyauox.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gebmzjsos.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnbxqqq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gdjciqcbx.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gugbauocx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/glvuwlhxf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gwmnbgrzy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gfcobmisq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gpzldtxug.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gtrrvwacu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gvxjcybsz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gelhqvxbg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gkauqreyq.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gknvtodkz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gummjmlky.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gjvbsmpcx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gmasqthxh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gwcapmyfg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gysivskwu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gkrhaqeet.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/glxltetdw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gyxqkazez.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gjuaocxlk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gjcbifjfb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/ggsicsymm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gadvgyrum.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/grcfdqvjh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gjppuyzya.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gngwebzap.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gidyplpla.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gdnapfuoy.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/glmzxpvdj.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/ghxqnokbf.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gimhqgouj.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gwrqisrug.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/glvmlqdxk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gstistefm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gaxvuthbl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gbmcodjwj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gqinrsrqr.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gmfhrujoc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gklaukijh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gsescbfro.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/geqkfbqkf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gucmcvzcz.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/ggnxbkpyr.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gqhwutaow.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gnumsamwd.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gtkxjipap.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gvtpbgnhc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/grzhtbllf.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gwvrstajv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gvthgsrmu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gjefxgxah.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/guodluryk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gqkawfqqg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gtlrfxyim.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gvklhgvpi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gglxqrrsz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gccgjgazr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghwykxvkv.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzvfotsxe.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwhcagasp.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gsrrebqfp.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gyfhiutcp.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gmdqzsiyd.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gpwahtwff.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gpshsunve.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/glfkvyemz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gisxjkuen.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gskxgzwsj.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gxibyjqln.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/glmidqbny.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/ggslguayz.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gzgekseeb.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gmurmplyr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gczmkycqk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gwkssxabs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gzcsurmpt.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gsmslhidp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gfknjgbnb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gelzrbdis.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/grajidbdg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gfkgfxjsg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gdoaumfav.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/ghcwtwnpv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gppmlgvsg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/goovmcvft.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gsmkqvnok.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gqnnoriej.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gxqpcidfj.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gkazwduid.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/ggcyodvzx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gewgjitnv.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/ggyhgcthi.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gzzajdtly.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gudchdmit.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gxyltmjhn.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gfrjmkrnd.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gtbxupnky.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gvoaaeigu.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gasdqonfr.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gutladxbn.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gjgyvwrwu.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gqkxeyahr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/glalvbacr.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gbwvggnib.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgaaipol.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gykstnubr.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gjeacfnac.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gshcpykjn.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/getpemsto.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gvyznvmma.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gmqpxyvaa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gthgolbtq.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gqpyvegnh.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gfzdkkhzl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/glgbcnkxu.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/giworoxdp.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gjpehnvdt.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gysxjugda.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gysjyaeiq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gylrmdxll.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gjnbjmotc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/ghfkouwxn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gdqirdpbg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gmsquqtjx.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gtpfizsrz.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gceyopxmz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gajupjzeh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gzbdplrwo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gtnretpqw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/ghsbbrpvm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grvrkijdb.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gfmuixgob.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaikjhexv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gmmfuyvrl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grvudtede.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gjppblqzj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/ghimlkppc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gqorhuhow.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gqkwhoniu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gaaccoxbz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/ggivkcakh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwfduqggz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gfcbzpiea.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gfxwehfad.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/ghmpaxkyh.sHtML


<!-- 参考信息 -->