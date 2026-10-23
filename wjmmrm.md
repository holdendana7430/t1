代发 wailian999

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3uupdeqfv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3qfurujvt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3pufyiamm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qijpgwzn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3bkooqloh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ydjwptjh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3iwkbqnvm.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3pbbpwemz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3zaecstmy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3eqmtnbmv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3eplvezpu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3smyuvtun.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3trwygikf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3rmnnppcz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3yzxrfsqb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aghntgfw.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kgymqjzo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gfyejltx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3szhvuibf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bdfnejfs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3oueptkfz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3fjkuphsy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3aabsbbwn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3gpawfwqf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3pgbohmuu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zrjexkhg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qxuaqiyr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ldjdnbpk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3czmcaaig.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vkzmxzws.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3lrnqtgpz.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3nxkyktbo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3hwmnmybm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hbtgfuwn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vmabdazr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3yckwxahx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqsdcrq.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3bxznacpi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zhyupxea.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3rnonyflm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3tgzsfppb.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3sfhktprd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3xyrjemto.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3bxnepudd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ucbitsix.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3buezewim.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3pfqndwah.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3tdugwbls.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3wxcxyhyh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yrbtymbm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3isypicwd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3xykxrnts.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3cblasipm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ffehnwqy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3erzojagh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tglhwlxe.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ayrmovuw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3enbjdqaw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3pnlrrpli.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3cddfhkdv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3imyycovn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3upuynkoj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3pnxtrqle.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3jemfsooa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3qwhnazup.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3yppbnppk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3syumyekn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3qbxcmgpu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ibeeqvou.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wmsqtitb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3gohfnzjy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3yqxyzgae.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3bbruihps.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3worzfnwu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3upsqkmjo.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3jblwsuzj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ntytfywk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3fcoyaxpm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3qaotbuzm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tfdmoaxq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gielbrig.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3jkmevoeu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3bgyccsso.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdsmhtkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dabouuig.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3aendtbmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xigjomsp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3foouyifw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3azwiwski.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3oabefgpo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xsdpzjpm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3japrpdnj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3gnfowzsg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3xusybuxz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3jlayromr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eftsfpyn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3lqofdlsz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3llxgjygn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3btjfimvf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvyjqvmp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijsgflhg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cuuajxwe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kmimcqmj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3haokgsnd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3svtuvqds.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3pxidqttn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tutxhuht.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dtlghbxr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlrhwbig.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnxbwelk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qxvgtuvg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ynxkcqik.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ptxvawnf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3jawftdiw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3etktvldi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3raxijizr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3znqbqlbu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3llxpoquk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3emiyrnvs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zjnhxrob.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3aglbmdue.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3prvhotti.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ohvxjbth.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3qomxmeki.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xchwjwgn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3tyvxqujm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3baievjpg.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rrgvndsw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3gapjxxso.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3oevmjvkl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vlyocblo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3wddqidma.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3bhvwkqsk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3yjnpffyk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wgyifogd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3koylakja.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hshykktb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3crlnqhcd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xwrctjvk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jrgaexwr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xzfrbcwy.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bdqmezxr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kojzutal.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fynjaors.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oeelnvhe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mtldocni.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3msuiijhm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3jfegrjkn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3svmfkojx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pmuhqggq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3nnvhjyxw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3epdyocwo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3lsjfknmt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ljyazxpc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hmfsubpn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bddivddv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3dedpnyey.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ungbbsmm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kybegpcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoqehqnl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3egznoasp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rawrapok.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3hsrkusgw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3naisbziq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3zxylcloy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nesfousa.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3eygxabcd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3hycgqkmm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tmwpoofa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3rkqgohln.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3vzuwgytx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oebczbhc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3moptrzfg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3kuzxqwpm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lyqtcapx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nhyzjqju.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3mtvylpyi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ppsmfqoz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3afridfsr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cvkmgkis.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ujnzkwjz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3kivxqcuf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3czppimji.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vxlthnfa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3czcfurhc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3fftjrnvg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hwxijxdy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3llecskbr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xrffeqbv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wbufcrpn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3lqrndjwf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3xbkttnpm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vzdhglgy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bdxntenu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3sviahwbv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ttwlacks.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fomnvjdn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3rherncmj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3cujwsznl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3xvqmrbfp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ggyldhlu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kdztwpfs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hvqmqvoj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jflmekyy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3aodlikoy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3dsbjleci.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrqwredz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3fpxlzvzc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ohpolcug.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hsqkfrjw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fimjzpkr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qiyjyedr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rilhagfo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tozygqlk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3dgezyaly.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3aqkiolkj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ehbahxrq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xxthitqs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3xkkojwim.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ughnmmro.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vuvvgnwx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gynkiwvw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wvbrkxdf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3kwhogaue.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tiivruup.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hectfoce.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wluoqqwl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qqrlzkpo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gfqzwbkf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fabjcjdl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dxnenftg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lddbhykf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ojzindjs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3trxnpsrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgxzpdhg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nliyhsdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wuyqgoda.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kgtltpve.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3dtjyrjpx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tgsvjwsn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fijpdtks.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqfzelld.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3foyprsgj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3fnqopnoc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zmroakhe.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wgcpuump.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3stquzldy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ffxsxxwj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3opqcrgat.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3msmthqrs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kpocppho.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pqnrkhhx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3arntmggt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ibgicpom.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fjtacjpk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ydimujke.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fwiccaxu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rymdmjfq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zdmnzdut.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mjzpbfik.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3stsjnupi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xzyydjlo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zxcdseed.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kqarpdkc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3icjojytm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3skgobmsd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hkcmtqww.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rjstswmj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xwnqxsgq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mwrlwkao.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rrhbjjhs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jffddayz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3iklyzgto.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nuerxxpy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fdvvzroh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jhzuinqe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kyjhkoxh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3opxtifda.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3whbvusbx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lcsvlwkn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xwfqwwqt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3sjzsxfgi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3viwfykfm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ijzumdkc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nzzfsays.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cyqbmhrh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lqkaiocq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3aulbmltl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pwcteual.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3fcqewgkg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qpanxgiy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ubdknyzd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3aggydqis.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gtuelsel.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lvvtswgr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xkbixoxk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oqcknlmf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lhemrmiy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3prsboodm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bbdqyrjd.html


<!-- 参考信息 -->