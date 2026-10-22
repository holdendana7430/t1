代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fvvqzuin.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xfywbgbv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ibgubctz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2opyfjrwr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2dyllkypj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2uugvesht.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2dcyzaenz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hbyqyuqx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ckoudukw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2xwbhqhhm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zwkwyokw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lfzrsedm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ocuydxxt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yrfnfmuq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ytiklyus.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2idwhgawy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2rkepdwih.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2yzobdmvq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2wmumllhq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hbawphps.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lwpccwvr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2aqrapisn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2levqohxh.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2omophovk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ffenhwxd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ftdmmbwn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ahrwousv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2algqjuvs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kwgyimvy.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2xhyebicw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qllkngys.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2aocwpeph.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2eduovfnw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qnuchesv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2wbzmisga.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tdjikqxp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fparbsyd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2bejuxpuq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2fxsqzfqe.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kqklqyge.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vdinemjq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2bpcqrhws.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2hwypzpwa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2dndqutap.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2jmcgerxo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2dzgqrtvv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2czkpfqzf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2khesgpsl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2qnmqeekg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2brcnfunj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2czuuveyp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrsvxoa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2lsjjnhoo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fulkxytz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mvzcctst.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2lycxsqvy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2yigmdehk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2owajqbqp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2siidfitt.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2azcckvei.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ryqzcjup.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2yyvtqzfp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aebpkarz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nxexnmwl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qzlttelm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zieqexxx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2oeqgppsh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2xejxezhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umunhwau.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vtldyfkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpyqmhqt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2orhmcaag.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2roenpabb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zoaygnqd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xhdairsr.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wryhpipa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2nxobpyrq.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ddpssypv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2dbqpalda.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2lmyrtmlq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2exwlgzxg.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjrxdffa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2unyfjhri.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yacfkkdy.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2unombcsv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ocpeoogb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2akrzdsbk.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bfxzysrs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2dpexcoht.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2mqewlzow.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cwnorped.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nzjvbxtq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mmsaryte.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sakjeezr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zxfqsahu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2clnitynf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2pwhtydba.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2yygykddx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xiddonad.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2roeifmau.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2hzwfpasi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2soinsdlj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nskmgqpc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ijiqtsfn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2unnhxoxp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2utwidysf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2olaahluu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2hcrvzage.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fzwotwln.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2fpcoeive.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dxshflms.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lzaenbjl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ouxsyfjo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2lkidyfbm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mjhmlnkj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2lknikasw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ybrzrfct.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wxmisfvs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2giaqokom.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lprbptby.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hwosbkpv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2stgzymio.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jgtmaaot.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vkapnmcx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tvrpvyfh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2qlowiymi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wbafhyux.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2uggaypqr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hcsidmgg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nmmdgvyx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wblcskcl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hpugmbvb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ohhwpecc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fjhcadlf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2vyxkkogb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kwnwhwzw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2aitvinlx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xhrfuntr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2fwgjhrtd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2onhbakoe.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hpnjiake.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2zrnyypdi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wcqaefdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhpzvxxq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fvodzjlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbcxhwfw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2saxrisof.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bpoczqqk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dmoztwas.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zloroisb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lcwxedap.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2zqulddhl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iwghcuov.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2kofvgvii.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2cjujityr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kdesoker.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2oiayttlt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xfmjpcde.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jyhuduev.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ujhtwgvf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ryghewvq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2slulzxrf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ltzaacet.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2vfqwoavp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2uajqflhy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rnymeper.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lypyhrhg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2isxzichm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mpqreopo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ufkecjis.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hdzyiktz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2irdbsdap.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2deuniple.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qibnhtaq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2kjvkwrak.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xsuipvnh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kssazkhq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ccrllxnl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zchvihrd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rlkfslat.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2oelchhba.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vpnrotjs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2oyrpafmk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ccevotmg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2yqphwwee.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jcfwdnuu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gbokxfaj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2mkrlwkft.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yswmcfek.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nrwkjtml.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2imcxnuef.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zfwvqewc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nshpvdbf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uqrvylqf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fuakuovf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2uurtowwm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rbqvuozz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mzspbxrx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ghputitg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2hmktgynz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mmzsfksx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2edsajwur.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2bkhlsmyo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rokicdem.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2agxjulbc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2chlminic.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sxzeduub.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2lfjgjhmp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xxbxkscj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ktazktet.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ewsegedy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2qbttafqx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pelpotwr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gcpsbmiu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2akjsuows.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jsqnlhva.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2efrzrjvd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kuepgfdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jblgocaf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2msgoyxam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzdomkcj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pqdwfeht.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rcvwlncc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zlwehdiq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2brwwufnp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ramvdtww.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kbnthifj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2obwgpeup.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fgbhgvhu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bmisafor.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wmyzxgkq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2khkxvkye.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2quwbytjh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fxesvmor.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ctfsaawu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qsoshnww.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eldpavtm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2knvupecu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hcqeqmak.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bfntezkb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2besfpbjd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ymuoaevk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bqxxcnmt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ksoabbvq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cpkhjjkz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qcranfjl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rczbjgre.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2nxyewsbj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2updmxkhe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wgnzersb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2cmrgvnpm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ntbtuuqz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ebukoant.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xnvyhvht.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2enamnebx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2eorgymiw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vauxsvpo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2embufpml.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqtalerp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zlepqilp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fuolzpsg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bggikbfb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfqvzvlu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tuymhjrs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hlluxppy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kcnabnui.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mhafwtwb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aewurnje.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ydmgeglz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oqewnvjy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pulguuop.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dkdnhdov.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2konefnhz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gwqcnqsd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ljhpnuey.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2bllpyqkv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hxrnqsky.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xgjwioso.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xgcyonks.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fayglvla.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2efbinhpb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fvoxcmhu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2odejxmgd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gxvrmmaz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rdalpkqy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qsbyhspc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ayviqypy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ecdxtfsg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nbkjhhgz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mbczjvkj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2okuzwwef.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2shvpkhjt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yylmpqpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhcggcoq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zgkyemid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cnbmcjku.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2llcitroa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktsceddq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wowzmpjw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2soymnpnz.html


<!-- 参考信息 -->