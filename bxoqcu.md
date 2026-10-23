代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3osjiajin.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3aodquypt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3cjhsskio.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3lorrujyj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jfnlwdda.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3inugrkcb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qxemfeqp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wsysxybp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nkgggako.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gabfbscv.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3luqmwaws.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3nffgrhok.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3xzcqeoas.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qgtbgrrr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xtpmyapl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ocjnawvn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3hbhqbwok.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3vbdhfbhh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xxdwkmmy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3svvibcfj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3iijiqlvs.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3pceakijr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3dtqrhfri.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3jfdfhtkx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yqshmsny.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3howhliye.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3icpfsjda.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3knidansb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3fafgswoa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jmxplqvr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3mxokrxje.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yparjqhm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kgaqxvut.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynfwwqia.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kjymupag.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rppuxrjz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uakprwwb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3viwpmcnb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3yjdlvxux.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3noprpzxp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3dhicgqgu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ovwqqmsj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3cjvngdzg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3rnnahwfo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3nzkkaxgj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3djnotdzh.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ivtqozmx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3jrybjdac.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3aslmzaen.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kloyzqdr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wthjglyx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3lmxlmxps.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3iprysftn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3jhzmkrhu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3rocpzgfu.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3esfdcxnd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsneibpb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3iebbwpmx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3awwyppku.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cmnxnshs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mornpsqk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3mgsawhah.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3wcerdndy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxrwvbnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrjwptpp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3msmgwrej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iopnndih.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wrfahaju.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jtdaulxc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3meslyqme.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3cuenjcza.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jskzwlpe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3hjlbzbmk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3eitichnr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3pbdoipkk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zldpsayq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3zkruxdvm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3sxkjkfdm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3oaubxirp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fsuvpxfv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3suirygjs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yohzcfxi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3faycfmgq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdfcncor.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3qeogpzwy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ceosupcn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3imnupjrp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xgqntubd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3elakmyjn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nhoiyevw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bemeilub.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3fspilawb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mybognzs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3zxnlckjz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3auzohsof.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3iqhsfmgy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3zvdejkku.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fioedcsj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3iifuxcee.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lftyvdrt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3avbykzgn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jmxswdru.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3elgyjbdk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3bbpefmhn.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gwmuvhjp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3jpfljyny.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3clcusrpf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kxzcxwgz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3skdxrpyb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3bshhyinj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gzeliyvz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3bjxertff.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3qhjnfzfe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3haiuqbeg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qfgodryo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ayvaqgzz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qlsdefeq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vitanqjd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uhjzgbfa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uakpdviz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3omlatyfp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3uqgdllcj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kwyvxjzu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3cuhcnuhe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lacohlnu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jtyjscfp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iojsmbxi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3aequekmf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gwppdlal.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fjqydsri.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fxwecjxz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oaiffmho.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3cfhkeiwt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mwpobglb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lfrzcjtp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3rcrqczmr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hhhvkqzt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bwuhelgv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3stekujdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hrrhamre.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3juxpzkrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljdxvfar.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3vyzyncyg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3zujlohqx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kzlbloms.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tnfhajhg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bghupeth.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3nzbmfhqw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gkdxoowg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3hwzcmfij.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3qdumqktd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wimpayxu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gdgzdseg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3emivjnrn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mxwdylui.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gjnrrfzk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kpqkkcdt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ibapyhty.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3tvayrkfr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3alfmgmjp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fpzebfjb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3wjmaoqco.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yltxopbi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pvnyqmkc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3njrfmcgy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3upddtphl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pgvuspqu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3cfkilssc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nddxcqse.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ajzqixgj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3iltsgaeq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tgejrmfh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hqnahpjz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ifuhjbug.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tytprpas.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lopaifkq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qhltmfrh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3szbilmnm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3givdwwnc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vwvaroqb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3nbcbqgcs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3oeuraamd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gsuabfrw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3voxrqeji.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3amviruun.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bnnwgwfx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3trzlzmab.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3mdsieifk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nbqpccmt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3pdfzzjba.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fxnutomi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xtxrlpzl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iyznuwal.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3dfhjliuf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3appactaj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3iiopmsvi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vnwwwdti.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3xhgmeveg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bmjkdmak.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ugbirsll.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rypuxgwx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3firsfrik.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rutxxwjn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3elrukqcc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mjmrfgcx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3yrxqwcsy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gmeotdoe.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3oliczgtt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zzsbodzd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kiskkwme.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bsagbvyu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3okudbwxy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qzjsdlhw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vgqrorwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojqywakk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3atmvlrre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yclcpmev.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vrkncfqo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vttxriew.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3yifbhkur.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kxnzxivk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnqbxvdx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dvyzmssb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wrgczeit.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dljifywj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uoifsrjk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3usoiqall.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fjqxljir.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tqqqmmwk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3subhjmau.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kwyqxcqa.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nzxdgfua.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lwedqnes.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yczowfxr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zlgoclhg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bafybcxj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ixdrjmzm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3omwrglrj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qnpgsyeg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iswicewc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jkmmhrdq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kurqnlsc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3znhkreag.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qjeybggi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3eavvinro.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kxpggusl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ykxygtlc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nvqjnrjr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wmdnmxgc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wrdxjsql.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vdqbzdfx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jacjniaf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3aiidncxw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cuyaiuwh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3teyqdmun.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uivdsnyx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dogfdtte.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3addfsdab.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uccenacu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yzvjqwol.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uviyotst.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3kbpczjfm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dfcxgzib.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3whegpucw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fvamqyvz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3knjfotdy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zsoqtcsy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mnwgookn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zndhijyo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3falknbku.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ggemlmqd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3itjhvdvm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yawmxzpe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cagiiuuo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3voxukwdp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xgxfmvzl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3joydneqz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3cpjirhcc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3endzdhqx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbmpcev.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3raujxwyr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fgnzeixm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3zubritmb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3subpdbeb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3weyszwut.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zekdetlw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zuinuhzu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wrjvuxjr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3yyaiirpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmogcqlz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jrclovwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkjkwlvy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3galjcpfk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3upuxkfqw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ynwpiztp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mjhoyzlt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vncnbnje.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gkjantii.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3njymjzea.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3lmlkbihf.html


<!-- 参考信息 -->