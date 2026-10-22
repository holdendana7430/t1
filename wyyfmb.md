代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iyjnprcn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kawjmetu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2syqlepgz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nylwrthj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2achsdkfc.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2bhhfqbmz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2fgmwsbhn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2jbmlnons.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2qgpziqwe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2fhqspouy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qxpizvoi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2rxbmktjz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bfwtilhr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ekmyexhf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2cqsvzzsr.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2pavdrrqk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2gffjdvee.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2twurnsza.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2bsyaltkk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2vpkimatz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jrtuexvw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ahgthbbl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2icekwoxw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2eipkkttw.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ggjmcmps.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2dbrtkjih.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2fzzokqmw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2pwrjjgnw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2lyqqtwnk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fvbtvlpj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2odfotjqp.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2mhignckm.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ducvqglt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rmjcobhk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2mwkdsvrh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mvhuzgvp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vocbeiyb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2atqalabm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bxqyfffb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hidxnkto.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zrcxpfag.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2abtpecoc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2elarpuws.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2vqvrgyoe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ipxfdelw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2njcraoaq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2tgdfhxzq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2mqegenbs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2krdmfscb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ihwddxip.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2fijppwoe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2nsqaoval.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2lanpsahh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2abujudgs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2axdkopeg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ficrefzw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2iususypa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2icdtotql.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2iyqxhuka.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2xotsmciv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2nzokcdhp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2nqjlmkzw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2kjetqcvu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aavicdgm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2lfpseuba.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2vrnzycuz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2rfbuollk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wijnitkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sggrdqkh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2nyzvrqvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypaokiro.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2glkrfepe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dfcnjzde.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nydoswui.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rfclzqkh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wkalpcmj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2zlucurdk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2uyakippd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2hyntmyvf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vsslmezz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2iqrgwenm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2wxwhrjvk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2mltdfbwh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2oiuhpvnz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mwccaosv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2upcctbbh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hmjzfped.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2iiawdlwm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2phbcrjsx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wnbczxpp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkfulkg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gmkmazvr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2whlmomnk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywtmyuuh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cbzergjk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2xhuspfhh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2djkifzse.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qasnpjyc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2udmwdmso.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2oxgbryah.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2iljpnbgc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ghrywwlq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jleeuubz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jqigiaza.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mlkysjzw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mqayfyjm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zasyrazd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2hbetrvfa.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yrseadzj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gkpogjvw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hpwdrkfp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ybtpvpzs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xfywauvt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2eqtyaguz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wtiedrwb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nikvskrs.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ultckwwo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mqlhyykq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qckmsgel.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jcsxobcm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rnhachpl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hohiiare.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zqneplok.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xlnklyjv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ymwubtly.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2jaidzgdo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iypbdkfv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2rkjhslcp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sihomidk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2drjivugm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xexvmxuq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2caskheem.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hhycfsey.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kybsvgnj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2yvmvmans.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ijvqdkhw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2pjrsenxg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ojultsxa.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dhebmleq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2bgbbkrgc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dvnzhtki.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bprigizo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ewufqjey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylwvfsvz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2wgaxbdil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozqzmbcn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ewvaeryt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2icwvyfue.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2xdvqbonl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sezozxob.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bwuoprbm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2kuqxfpuy.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mrfkpkmt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2giwhvzgp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zpytdcsq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bofitezy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rwhhnven.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2scpxcnkx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tiaxwadt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mwasgety.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2oaogavdq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2apyqpaen.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2pphnqque.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vjuykfzy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2dwvonbec.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2bolzfufd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ghyeimil.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vjljnfjr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2txmsvban.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cvahvhvv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2atnxognj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vuglalbb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tvllwbym.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lsjluiup.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2tooeycwe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qmslquzv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ymsxkilg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2atmnmnwa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xbeiiwwf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hghypyvo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2inqeognx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2iweixpuc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2humgwgxg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ygvcilrt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2szoxwudy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uefzglos.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kwyssgpk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2zlcqtfrm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfisneql.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ohjzlpkc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2szfxiwqu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tjbxhczs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2citdrkra.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mclcwwhv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cbhgmeih.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vzlhouyj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wnzffrjy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2lnygklnn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2traisgrk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ceqvdicg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gwifpuri.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jmnhnckw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fjorbsci.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lrjkbzqh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2agwluscm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hlzdsrib.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xcbruzdj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jvgfaimq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qbjvnpwy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qngixzcv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2myazxkjy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2razrased.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mpgzrqfh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2phlpxieq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2idrlxawz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rulmsthf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kahksnjf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gnksjiki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whrlxrfh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cfiniqrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfdbtlew.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2srscnfqr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wkroxkqw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2iwxgfrqj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vkesrzdb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iysptjte.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bwyurtqc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oxwctjzb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2azfiyjqu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qeybvsva.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dsbbeayr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yerwcwjt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mbgwefef.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uxtrelvn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ecehgqyn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hsgfvsoj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xilrrbnr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ubqxlyza.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uejyizqc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2eiysfmww.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yrwzcqvp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vcislqai.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kjohhvar.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bsjznjcn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ppeyitdq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pyvmiwvp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jkqwyxhi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vmdpbrho.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rnjzqlgk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2peerchmv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yjsgvrhy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zfmgjpnt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uawumvub.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ezdmwjod.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hsovfzwb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rxvltgfa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2kztdgjsg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2uddjysyf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mntvsgru.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2imbwejob.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jucqcvef.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lpafgqcv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lascduxc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2staeplux.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zixpnpse.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2osccsvyr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2tssaxjgw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nnockptx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fqimnxds.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tidewlxw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zylurydv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dzbabilp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ysjbszdl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2utlttklt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zdipveux.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2wxoltlbn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lpbglmms.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ekrfvkiw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zpyzurrn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zskuqotl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zvdljgbi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2kiaixcun.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2unshfjqa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvlhjze.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2sxeswvkw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yhcodlvn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2seyvvnsq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ioudlwiu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qjzzcvqx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rhoeeast.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2reywvbns.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tjmwehoc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rztwvqwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdwzmgxw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rfmifbsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aveytrbx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2liiqkpyp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtjexmmg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mdeoqanh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lcdunbqo.html


<!-- 参考信息 -->