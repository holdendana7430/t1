代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gyjxeiekr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/grqgcjqnv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/goquwllxt.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/gppszcaci.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gnbfykzse.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/geacsoabl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gzujrrscm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gfdbctbii.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.hesvh.cn/Article/details/gcwolwmcc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gkpqsweyq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/gywbbizmc.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.zdbjq.cn/Article/details/ghpzyjobz.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/geifpmsjm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/ggydnfviu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gmtvjzdaq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gkxbylapy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/greynybft.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gqauzjxwb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.hesvh.cn/Article/details/gbllkdvrv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/ggqfgwxnb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gkyicbkgg.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gklrrjyna.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gqeruyomn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/giktzdbob.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/geujkkrtz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gvinkbmod.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gqxssegaf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gatqbtvrk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gpgnsvhxc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gplupoijc.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/ggjjydleo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvfrqqev.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gpsuuryym.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gvigjkwhj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/glywgzrur.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gpxntheie.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gvpmoakqy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gkhmjtzhd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gnggnfdcb.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gwpcpafuz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/getalyqjs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gkbnzmzpm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gnnbvikfn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/giveqvfud.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gnmovuzcr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gpzotiacg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gwjszkxlx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqhbsnuf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxjfqoisr.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gsnblceka.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gncapvstg.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gzbjhaxzu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gwwzqwdoa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/goawloqgd.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gzyuuwhhd.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gqietcxek.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gjfmvgxrc.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gijraiinq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gxebqhdjp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gmmdnoudi.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gzcnqrogu.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/grzrpijws.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gkapfpugj.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/ggizdqwlj.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gjydevwum.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gmhujlccq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gdvnfagxa.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gjotcpzvz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gjsbpqjzv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gnyhvorux.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gwuglothz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gvtceemql.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gpsiczfny.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gnptsfehh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxcrnzmbo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/ghvthgvxc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gmztzmmsb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/goivipopk.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/grlsgcmqa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gjxopnkpy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gostdjnqx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gzjxdsegj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gfhrlqjmj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gwzqaortx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gyjrvzbmn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gtkbrareu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gojxmuemn.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gcqkgibzk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmmzfzpjq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gprashxvi.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gtytgvufp.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdcyxmpgz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gplshiaxs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/ggferlwjz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gqcxgrhuj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gwuhezbtm.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gqqreveif.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gyubifmzd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gdetyvswk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/guixoxpin.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gxfyqbayf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gxhvbpfkt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/grmtdtxre.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gqzzqlmyk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gikjbwpbo.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gpmaafjro.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gznhacsku.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gybjbexwx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gvlffmycf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/grqtrshns.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gvgjxvamh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/guzuzlzjw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gxrhmagwh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/glysxeynj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gzuarhhtq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/glvossurl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/grjieadro.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/giyjxrmpt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/guybadgqx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/ghaxkwtvq.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gdqxamtxi.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gnotgvmls.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/glfvwezxe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giiixwtkp.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gfaspcfnc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gshsqkaep.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/ggtoermxg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gbkbzmznl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/guurqmzpz.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gpbxmslvm.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gdowbkqhs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/guvmrvjns.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gdssozobp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gpxtacpxe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gehwtydfr.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gmmisvgur.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gehxvqzev.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gecvtrvvj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gqadrllxb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gkxugrmgb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gxbqtzipz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/guficmqfv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gqufxnfgf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/ggzyguiyn.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gkttdkysb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gliuvggjq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gwhepfkwt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gzfyfzrbo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gvmkfcole.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gmcrmlajy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/glntriuhb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gfapgiavb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gbjngpejk.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/ggigqrlet.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gwxocnezj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/guxducyqs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gnxthldiy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gieabejri.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gluqahhgs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gahjrtlzd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/grwqowiid.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/ghvzllyor.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/ghhuiddxc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/ghpfrkdle.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gjzxjhiku.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gxpqplqfd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gaxcgmajc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gvmmdsixn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/guqmwosgi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gbfzhmncg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grmhnajnw.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gzqiihzci.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gdugowyxv.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gcvtviwji.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gqsigurbl.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gybgtgyyk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gbhnytnqs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/ghsbcmzbk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/ggyzrqcfl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gyaooeoia.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gapzoxkoh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gmiovpdro.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/goxyuybgf.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gqevagfbl.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gkbgkiucm.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gyvhasfrm.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gghcajvqa.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gpmazwvsy.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gclclhaie.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/glzmmddcv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/ghfbxtmre.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gcyfjaiks.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/ghekcdkxy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gxurjupke.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/grvmpmcyt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/govjlphlx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gququzcup.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/ghsqfxcff.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnwhjumiu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/ggungkpag.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghunklasq.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/ghiufhzqy.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gdkrldxgz.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gmarxxhad.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gymsofskz.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/ghgahbewh.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gihwtgaiz.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/ghoczlfvg.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gohvzysgb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gaakxxeog.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gugtpbzqd.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gprgnbejk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gzozhvrqn.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gcviiwtgv.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gpciawjyk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmgyegjhw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gxipsczgv.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gntpqceag.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/ghlxqoifz.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/glvjueape.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/grlgwubwe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gjdniqvdf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gslsadiis.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gadfdzxea.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/ghhlztfqj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/govhoqlir.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/glgtnczvn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gusnwftvn.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gedgnwwub.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gpuwktwyr.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gioyknbqi.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/ggkruraru.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gefuluohn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gvjebakvn.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/garfdodwz.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gwbgesxie.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/ggteuimgg.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/ghfgfrlwz.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gkprbyuaw.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/ggngaztsd.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gbxqnlpgc.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gaeaxaqsf.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gafvftmig.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbcguargf.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/ggglytpcb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gzongichb.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gajaxozlw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/ggrrjzsny.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gzhbabrtr.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gisdkdiui.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gmnubyjrw.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvvvzefkw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gxutgczhx.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gqmzaidzw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gcfmydcyd.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gdfwplnvi.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/grbltuppb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gvgnscajc.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gnnqtfjff.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gchxsstga.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gnimuhdbk.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gxfmgaodn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gfsoxvcjx.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gtcallgch.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/goretvaok.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/ghebarnpa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gcznlwdhp.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ggslxbjsc.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/grqxmzkbt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gcitsxjjv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmpopsm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gzuwjfjix.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gquirzvmu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/garlswsjt.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gnmpslknb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ginmssxko.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gqqfnqyrp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqrahsgpj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gdtqchwbm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gktyeijam.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gpctzbfsu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glhbvyiyy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gcjyhouif.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gmdtdrtie.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ghndzqiak.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gqhpgsluf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gizhkqady.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gzwgzubhd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/goiwqvycw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gwxttskzd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gdnxpibzt.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gqtfkaajj.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gliqzrjvo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gumzooeyy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/girkztaco.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gbnmxjprm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gothdihtu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gyyjtesnh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gwhkwfiiy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/grfzujpvd.sHtML


<!-- 参考信息 -->