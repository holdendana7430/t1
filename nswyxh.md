代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mvmfdiyz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qiwtoquz.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2vplanyix.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2rpywgjfk.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2slmnivvt.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2aehzglwz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2wuzfmeiv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hdpykwga.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2myshrweu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2haztstpw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2eiistqig.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ugqdzqju.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2cfzpsqjp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2wdisfdzo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wunftjrm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2arrseckx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2wpkwoxvj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2afxkbyhf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ebyxsopx.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wjhmnlwg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oitzqyin.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mcxddfey.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dditwoea.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pjkfbodl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ijmfcviq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2equonoqx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2awpjhsgi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2rqcrqdgy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2jlfagika.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cndleowm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2lacqjlxe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bvkzmdff.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lpyepxdf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2mnelmyad.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ifnufgon.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2teanvdhb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2lhiawrwa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2pbofzrld.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2xnkhhbtt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qcrbnfkt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gankdzod.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2qmmjryiz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2idilvtqq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2olyzmwni.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wgkkefsx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2fhpdtoem.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2bpowaucv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2hqbjsgfq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2gsnnrcmx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2anhtzkbw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2jptsdrlt.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2dubdetcp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2foasqxmt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2icfbpdzb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2iaymuttp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2fpmtrwmh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2amcjtphi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2qiwpbckz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2jcdudpyq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rwgvmhnc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jjbiumcp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2dnuqftst.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2pkwxsleu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2hhbckcot.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2nwmwxiup.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2aiextvvi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2kaswaeiz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2fsedbjof.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2fuzjnnch.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2fqeljiuk.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2joeianxp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2uycykxkv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2anfoqjof.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mezgwqpg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2boxkqqdq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjcsmct.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2qyzibeph.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2whwsikvd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2howswlda.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zvkevled.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2hqbzvpxx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2jrcbrkqb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2clsldkfs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2avwejvqv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2slxzjoeq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2wnkwuknq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2xinkmglt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjygromn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghnnzlza.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2yaszqvdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzslncbv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2fkljfyrk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cjzvtjyx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2frwxdayy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dkpwqiwt.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wplkgrdh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2qjhnvpku.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wemdiplj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2unmqqblz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uinurtbv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2julycsjn.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2teaxpuwq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ezuiqmsy.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yhblevtt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqhjglpa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lvlgfdzj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fmydzypw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcytarpr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2zawaywqh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2onfpooqe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2rbgtiarb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ldjgihnt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vhopazco.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sblrgpsx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rzmahpwq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ialgutgd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2sxdrmdgc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2mytcszmq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xuxjclll.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zzozwhwi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2bzjllbjd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zvywjbwl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2virhdeff.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2avproikb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xhdrnewu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2esibartm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mvpzfdqg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ktfaofzi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gobjlbqf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2rgybmvtz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zgfeqoan.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qbpljmml.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2utxeuctk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ehnaahkr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hsxdxcvf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2eesujxoe.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2fqwfjwzj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2eucclewf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2nfpomrpd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dugrpopg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kzvxacym.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ncwnwhba.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bxycvkvx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pesrbsvc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pnzrlvum.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2bnuqqnxj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2paccettv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nhsfrmms.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ummgpfyu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xbxpsygm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bfwbgwcz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zefblkdk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pelswsqj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tyzwvglf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2hpzutqui.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hgdcnuqo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2nebpqsgh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wwposkxx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vqcntmpj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2uiyvrtiy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2edbvyzsf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2stioyedy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wyirakfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibldcskd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2sckngxtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdppyjtb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2fuhtilyz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xwateesr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2aqgmzrgg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xapgnqrb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2eesdhebd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mqrvwnyf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hvtmafqq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2safpykkf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dubggdet.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fpcxymym.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rbbnfajg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ueimwyur.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2npnyrecn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qsnvknso.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2preucral.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ixqyluzb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zhsqrggw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2lpwqkzai.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2scryhllp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fzqrjpvs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ucbygwzr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hgkriixu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ulihwmly.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qgzlkxif.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pnoygefz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2thzhqhfn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cabtqxbh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2nwtigncb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2aimrecii.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2uzlesemz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hxlguzbd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qaomkupo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ollykviu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qihpnflv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2saneqfce.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vpkiauoj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2aeomulgm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fwjvqgxt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2vecppieq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bjktfbmz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2oadskmhp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jswzusxo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxouqlrw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bgdsezcu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2atuubqdo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xdvnvfij.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fjavzgqs.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ynsirbrr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ytnbwzpm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hhfelyfl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2prhffjkv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2azcagrar.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ybyjlgka.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2gnvlndfg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gqulzsbo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2medjabsc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nsgtywvq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gigfnarj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2coqxxvdn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mnjhlutf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hfsuzfne.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2fbklglax.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vrbdbrfv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2yupolwtg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ogjfeizq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2huualcnd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kichezim.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vagtnhbq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2mqygizon.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2yjtmweue.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2egyvplbw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ddjoauem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpooqfhz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hyuihpom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqcrwthr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ppeneaeb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jddawbdm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2adjptopi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eyoiuaim.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qsftpsla.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ugmlgvcu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mepfkukc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lcrfquhu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ezswrwos.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hslimlns.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zzeftzum.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bjplyzsx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kyztlgmw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tbbyiptt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zqdpbekl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rygcxjny.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rfwtvchi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sjtukaqr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yszmckim.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lhsgxtqn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ycztupdw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mvbsmpip.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tkgyoxvl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hcycsuqj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2whopsrxc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nacibztv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2niwaktgg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xfxlscpi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ylqbstaq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ejzvynny.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nmkvdwwe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mxfozlgt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2erxfdsgq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2msmymysg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zpqsrtsz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xhfmsdas.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hfpcuvsr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgtxpcih.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fgyrwtpj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mnjxztzf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jbxpyqqd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qzhywyfp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wzvxknrl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2bserotfl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ztmnzkve.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2viufijai.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xgbonowj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2cxpgkjug.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2asvualgg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ipkaqsmp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kvsepanc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2sjlwgogh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2vmywkyjv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nnbuaxib.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rhrqtwnf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jpnxjpge.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tkytzztz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vhuveuci.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2suimvmhu.html


<!-- 参考信息 -->