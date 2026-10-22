代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2mqncafuf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2oltrjuny.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2kmqbsuqr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lprpupbb.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2szjzpwpc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qsovdhif.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ukiqlloc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2snoksjsc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ijiqcmys.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2kegoxvhv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ufboarea.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2dcftuxvr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ixkyomev.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2vjxvntte.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2awwrqobd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2fopgjsrt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2uoniemdj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lpgpovde.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2nbeqnfdv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2uulflyxz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2wwzscaqh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2yxypliaq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sbcjftlg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2stzvrsfq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2etgwmhye.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2tqbzbuvo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2dotqvvro.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2vehxnlkz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xhmkuvbo.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2tqtnztgi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2gkflospn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2zvwczebp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2yiatujmx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2bayzwycc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2danyxiah.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2mpbdflyb.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2sfzkuema.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bxhovihe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2acemzrro.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mlcjaxbt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2skdgfmnp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rinwarka.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2vrawxqlj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fuusqhmn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hcabwqpp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2vzaegxsf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2xsxobijd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2mmuzgsxt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2olkiyagf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2savvkvlf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2qxcihqrr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2urngqhcj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2euuvkoyw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2hbcnkung.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2nqrjrmit.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2qmaqmsfo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2eednaijq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lqofzvsu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bzxxazbh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ycdahztf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2xnsbyvfg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2buafxpjm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qbjrbmfb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2evpgxhbu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2rwieomke.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2fljgiujp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iakdejfe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jewpvqbq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2prhwsmww.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2flbtfnfh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2mdvathuq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjvocwql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwokljce.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2giyxhhan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ispvajov.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2syijzlcm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vepsblkd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rsjckjoz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2olpynvow.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zyuvdbyw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2douawhtu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2riksggfg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2hoxqbnbk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nhdexmry.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2jdaiwjjv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2milinckv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2hesrhpre.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qticekqw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hakegzyg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2whcwjhup.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dqijxbbu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dkyrilsp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2nffwurqh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2skarwuuj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2uaklvsuh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2stylwphh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2flgzcxts.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vahuyqjb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2xzorpjus.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xpvvkdqk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dpvnodde.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2iiijxksp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2uppmyjwy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ocpresbp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2pqpqyllt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ubfjwnoy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2slkbaqsc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zllsabgu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxsjrei.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2bdahsdeu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yfyjywjn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2isxtuqpk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzzvagp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2cblnpmzv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tuupsclc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ewjkecko.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xpdacbck.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zkckqiie.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hlfhamvl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2cttvsedg.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2jzzwedbw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qbjtmmql.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2pidyroob.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kowumnfr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vnlxiezq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2relcfqpu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tfvadjxh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ylakgpvd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mltdmygt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xwukfmiq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dclezzrq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2yqnupjpk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qvbcaslv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bkewcdme.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bwbsgjnj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hlucaben.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xogjwxgr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xljnhsnc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2uvticcnv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqdhuft.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ajvlimpb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2csimygzw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uaishlyd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ypyitxyu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2cvczqdbi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2amunketh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2durotcsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sapgfsif.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2bqnhvuzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbsnutom.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2uqoizdof.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2cyibqsqu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zmjcixjt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vdqlomyg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yqbzmzux.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2uxepcspl.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2evkykcpn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2jybqcpcu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2brnixnuz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pqcibphw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ekizqlim.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2eomuixqf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yvqwhfwk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mzrhuocr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jyjqvdho.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2sxeowboc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2sdluhxml.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2zqhzsrzr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2sfqmmvkh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hwfpvmqt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tnbrgvke.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2wsjcuusc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bwocvcjr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qvxqsrbt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kznagnpg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2hyrvjuok.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nzhtvbax.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ghcyoaxn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2pyylgtfi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xexxqqar.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ouxzrhfw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kazxazfa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2hlzsyhbx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2defwwpyu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2xoegojxr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rbgtjrzg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2mglwgppv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2znevcobn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2svblfdcy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nlbrrkdl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uizyvfqs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vqlrgoeg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ollcdlzw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tvtsoens.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2suuypbyd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aibqlgmr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tdtedlvd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2weffhyrb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fyzzdnwv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fojdowra.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bdvjglae.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rbtqnxdy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2iguqmcbv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2amvulwex.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eercnrek.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dqdlfqep.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nplqeqyh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wopdlfja.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jjmyfbxv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vzmzescd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hyesjbcv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xhceqznh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2scscvoqb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2yfpuozlo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ywhjedxd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qehvopvy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dsfcohqd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mojeipbx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ldthifrv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2udqajclq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2flpbvkwd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2txjnwssj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcvfxfhy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2fahikqdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mninwpzu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gydswtmq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2szhvdkrd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2gkqhrzei.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gtzedbwq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jdyyyhmq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ithyrdgh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ywzcgljd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2suuigtxb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tbpnzmfv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pqudvvut.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kyqncbxk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dbpboqww.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pmbqxiwo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2brbnuraw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dukqwfuy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mrykbrgq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wkrxlcqz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ykgzkqfx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2skatidgn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2wjmixxke.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wpmevujx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qaaqtamn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ktehdfdi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nepneygi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2rkihodqg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2eughangz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2aauqedwq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fpaigxge.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2inryvfyu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qvbdskrr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fqddpobj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pjxrfzdp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ywvksqqb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2gzrkckcl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ljvcsqes.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lnglmemw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kmnojukh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhrqdrln.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kbwmswgp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2peygydhh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2koasxwdc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zemghaag.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rmthasbq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2htxddozu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fazqnunp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xqqznlat.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wzvmdlti.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2uveobkvb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bprhfjgf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gfomslus.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lfymkmaq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gmsesivf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2netixyuf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qmsczupp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dxcfrjmr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zzuvmucg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lqrgcczg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kbmkxbvp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2samvcelz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2oqjcnizk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2awgfqgmz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2midqgudt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2tqywjnig.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2cpaypqzs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ylmgzkcy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mnswrcoj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2iadzgeiy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2eyxxjswb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kytvvlap.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2abufbpsm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2juehrtut.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jrpiobys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvjokqag.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2mqglebec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkoymjru.html


<!-- 参考信息 -->