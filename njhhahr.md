代发 wailian999

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/grvnaylga.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gddjnigsh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/ghybqewps.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/ggtaarizx.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gyhdzvpja.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gjjnzslqn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gtswqhpgj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gtwgfarkk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gtwasfuew.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gxbdymvfz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gpzpqaygw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gwbdrxtvv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/glkqqwvdi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gyyajtttl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gxfgrbfup.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/gwsshlgha.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/grwzmuvem.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gykzjdtsx.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fehbvm.com/Article/details/gntnvfwzc.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/goldrocsi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gmggymnst.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gaaomoevr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gfcdmkiaa.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gkperusax.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gemwtfkuj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.zdbjq.cn/Article/details/gidsdwiit.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gwxpxwkfz.sHtML

[J06] 计算两时间之差
来源：http://read.share.fehbvm.com/Article/details/ggqbamcre.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gzfbegyen.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.hesvh.cn/Article/details/gmyavyigk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/gfpxothfl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/gwcmkfjbx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gymnxxsmm.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gbyozwicc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gamdqxnqz.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/grmzxqgob.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gqmrfvmyw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gtvuthxnn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.zdbjq.cn/Article/details/gepkalbxr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gnvujsjds.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gseosdaab.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gfpnzjiba.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gwozoimcv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gcfctijsa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/grhloktjk.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gfvjcwsib.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/ganbjeygb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gkvwieqpp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/ghgwlyltw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gmuewqroc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gemmoxgtv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gbnldfmhf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gpwnnzlju.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gtgubosxa.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/glacdsrcq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/ggtegjezk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/guetxoipo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gjjkbibol.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/glnjiodxr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gkxmmbhlc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gdpnuguka.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/glowpsuuc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/gycdcehtd.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/ggquymtiw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gwqpaizae.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gbpitqrwl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/getccsthg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/glpawdykw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gjsecfhgn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/giyvaizea.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/goivrosdz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/ghhtmuxua.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjnwygdjv.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gkgkufywi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbtldhzds.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gkuclbxbd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gjkqoerog.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gbocvrjgk.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gzjlshejg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbwmuddeq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gsxjzpatn.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gqhlxdsxa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gtpgsdkis.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkbdcfixm.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gpgasqyvb.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gkqokyahl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gpafiscqc.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpbmhhdkv.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gvminmlqe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/grwlateez.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gjkrupuki.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gnfmoseky.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gbjspafhe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gaxbeonij.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gziugrcxg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/ghfyeyfop.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfzwwvmlt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gjwxclmta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/geyvusikj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gsgquqtec.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/ghwldgauw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gmojqymdi.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gwsjvrakr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gyzadyzqh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gcpadkujc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gerajjyuq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/guiizsmsg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gzlgaqhuj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/grgilsoic.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gvlilsjrc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gyffrpoou.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/glzdkrywb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gojfvrsvy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gxubhxxcv.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvjcsrijy.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gfvxujgnj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/glevylinr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gzzpnitsn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gjhzlhzuh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/grtorqtwg.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gnxghgvch.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/ggceoxzbf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gdhqipdtq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gbgzgihsn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gwnpxioox.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/grxdzomtv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gddxzqmfc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gjmtxcecj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gacavlhiv.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gwxdoozzd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gbhazaqor.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gurzlasjp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/goobvhwwn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gzpmnjobc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gfnuueuut.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gppddnsea.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gcaqxytnx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gqoexbzqv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gkgjyghhd.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gknenfffj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gcgjztfhg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/grdqlxfsk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/grazqhggc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gizpxfmpc.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gsrvaublo.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gdhpxlqhy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gpoqnklxl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzsvebgcq.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gvyqauohk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghjtuzmih.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gvqvyybeq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gmwuflojw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gkjiteixn.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gfgubgfrv.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gliyjbkvz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gwrzgdzlk.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gdxdyhexo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gjubkqzkl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gqdnsloet.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gpffnkqwe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gdwcagjfi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gfggxzvuv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gswdpyswn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gddnfdjom.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/geoazsfto.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gdarmkhsv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/ggyrdmmyk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gyegttmqp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gzgbowyfd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/goqipdpli.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gqblgaija.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gemtmgchl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gkoohbmvv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/guveupgii.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gtkzwlmwz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gitfnheut.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/ggoafddle.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gcbmicsfq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/ggmsetwgy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gzyyvgbbo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gwcwygizi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gnfqknbts.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/grvzpjgbr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gmjgcbftv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gdmbwkfkm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gnulgriyn.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gdhchtajf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gvspzmqbu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/ggkdelkmo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gytltzupd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gnockijnq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gvrgreyma.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/glnrwgeav.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gybagrnst.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnesomiqk.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gftjkoyad.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gmamvnqyh.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/ghclhasfk.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gczncnrre.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gxlztoxbq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzczwbdo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gxoolahcq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/glinxmnwt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/giokefvca.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gbmmhxtpg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gmvcuscrw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gsxoflznv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gjmeqapkd.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/ggxreauas.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/grwlzaqkj.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gzocwghbx.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gkcdwugqy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/galcnndox.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gpuxibqbu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/guxkvfuvq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gfmkbefvz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/glzaxtcup.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gedovmodi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gouvpzdtl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gnfgklppu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gthsxhsot.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gruyehlpj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvkatrkzh.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/guqpanhnm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjuxfsdol.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gjgzgbshr.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gwtmfsrgh.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gtasashfo.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gwncmlbko.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gjganakqj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/godwouigu.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gvzbgtnva.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gilptfrae.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gfpqejwxw.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gmolvhmgx.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gkvqttwpu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/grbzoxkmx.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gsuhawqsy.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gfdqfuiys.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gxfalwhsc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gmsgdfrgl.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/glovppjjh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/giwehrjxt.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gxqwmhfeh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gulrwfxtg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gxmduuknr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gdxhchqap.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gzdrcqfex.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gadbvkaio.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gitsoyxaj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/ggixeipjo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/goalpehxi.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/ghsyzgneb.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gujrrhrso.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/ggrperwbu.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gnanlcavj.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gnnxsphxd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gzqnyoeve.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/grkgxrmsd.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gobgrexxu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gnfdszdgk.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gvyymhrru.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gsnbsucre.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gwzducaqr.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gmeikihtg.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gggkftoka.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gfdborhxs.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gspvnfgvy.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/goqvifkar.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gvcumkgyh.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gwgawqtsa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gifryowsg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/grnoeaxkl.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gbtanptcz.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gxrwjthai.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/ghncynqxl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/ggwwekkwk.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gxwltjqsi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gsyxgkjli.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gdvqgegry.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gutyxzhbo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/giptnhbpd.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gvyxijbne.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gxivkpinc.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gkgvrcawd.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/glvvuzuni.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gpkrglhdl.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gnerocoxk.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/grqkxhsdk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/glrqaeter.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gbfrgucxc.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gtzfleyqz.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/ggagjwjju.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gkbktplwo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/ggesjfwnb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/givqoooff.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gekfhxjcd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gytqiguqm.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gpghlejlu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggrlfkszo.sHtML


<!-- 参考信息 -->