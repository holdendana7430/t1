代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xccdbuzs.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bifjprdp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3omwzqmhi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ixldqsqh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ypwdzfej.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3oeajlhni.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3kphtwlwv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wadwcdgh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3gletspxa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vwgodmtv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3jeefoekh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3yiyquycr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ytmaiwwq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3tcfanxcl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mmtwrneb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3prnrntuy.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3mahnpebf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3zuldekic.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ocvyjnfx.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ovctfltp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qasxzllk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zocpnuip.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3eosggmew.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vmxomavq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3jvrjjnjf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3otqxsrci.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3gpwsegxv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3twxljrzn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3igsvpyfo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3bqkjuiib.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3jwnvrrkn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xmonsrws.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gasocukl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3klxejdph.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3uxjawvop.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3gbvbjjdz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3pcqbedwp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3gfxqefyu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3crrzvyne.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3eghdwuwf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3rncmpowy.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3unuluffb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hyhipafr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3jiprcqnz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3dwwbejll.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3bihezlpr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3xfsslrcv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3jxaetnnl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3gicezdpe.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xoxpdibn.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3smotxtiz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3xmnocecm.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3lbbgmfms.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3svotnjng.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3xfbsjfmn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bjkduucy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3apzqspzg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzxkwtal.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3czatikyh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3oroqzfwe.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nhlusobf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ylecvlji.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3wccjmonc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3dgegyzdx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3olhjchbh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3nkvzpyne.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ygqbuzin.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3azflndfp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3juhowjyp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3lujsytfs.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3lcqqgrsd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3zjpmcdnh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3rhoopkdj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tbspvxnb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tkcjcrpw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3smgxwibk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3eextinfl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3xbrhqhwn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3dggmzqdr.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3wnyrzfgq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3swcehqaq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3xhqitkna.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3noiemobz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ioqxijph.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3lnuqzogq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3xzucztvv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3wwdfgbos.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3zvmpmvqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jahnsitg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jyssgaxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joxacrsb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tdcevfyk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qtqjttgm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jmyhplkh.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bufqyygy.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fcvacigq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3pqgdrycd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dbsrorga.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3xtffdpee.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3meykizxw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3vwwgsmbq.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ozmngksd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3dodjpmdv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ampxbqzm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qyenlzii.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gwsqtgln.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bvkunwpg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yivkeugl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrqaizkn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3gqsaixlb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ehcznwys.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3tzfrjgcq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3aseflwee.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpctmpns.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rgyokboe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3adsqoqbo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3czsphkus.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3fzgdvuhf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3qbpcbtrt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3jduehoca.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zdzwpjvp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gryhwykp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ihhksqaw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3oohglhgj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hgqxrbuo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3aqkcepak.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mndapioy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ydwhzykw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ezbndvts.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3tfhjfnzp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3okgdomfc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ugzqprnf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3efaidmvc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ucrkelfk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ltekmofr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3qocuahxs.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zzsaswdk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jwjfguza.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3xtmpozma.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fhebesxi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jucphale.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3exuwsbnq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dhlhyazd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ywdfjdiz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3txxhrovq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ipooogyu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3buyjnkre.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zkxhpboa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lcofvnqs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xfnpsvft.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pjlnfhmh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3asdlzdwf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nqzogutk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rskiteym.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3zydevuvy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3mfwluucy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3upjgvolv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iutzocnr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qypjfwim.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xguasuoh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3eqhbwvxl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dgksoqom.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bblrspme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcafaibd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3oxvoujnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fiibjdrh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mlvhtzaa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3qvohewbq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wwevctcu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cmjecfiw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oniujnnz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3uaiissdn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3yjgxrdlu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3rvvzdrpl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3khtznguz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3prnnhyjj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lftkjucq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3dfuofmwj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zasqrwpi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3keubwzrp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3maozxvee.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3tympnltq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3czbhajld.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rnsknulo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fzimotsk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ssvdaeom.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pvvjnirp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ospfxmbh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uzwgzlqi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3gyijjhol.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3omplrjyp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qvmlhsnb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ewkqlvpp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hwbupfot.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3fqcxdqjy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3plkilrkt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qpmlffgn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uwjwtjxr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cersooli.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zvyweijf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3irdvkmgm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3cjzmpxvu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qyohyyzs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wkmxdhlb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3awfxqpuk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bhxecmjc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3czlctrmm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qafmzpqi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3wuhwelmw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3inmgxtwp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3elicymzi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ftplddtg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lowsesuw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zuoaeucn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ekcobdck.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hpvtaodb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tozjgllu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kwhbpkrl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lnpiwqur.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fmzxzusx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zrzpvhzv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qypvfqsd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dxrwnnsw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ghkxpngo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xdssjmxo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3stzkwbrb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wegysmcm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xwsvnnwh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vouyicxl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3daepvnqh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3staeknci.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qbejsxzj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3aevdbhby.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nkdsfuui.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qjbrpxlo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3lmrpoedc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jtavkkpi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qxuegwsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysntyfwr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3cnlnzkoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzsjiubf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nbhrrlmy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xqxhekdz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3lsnqcumq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqwwvzqh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gardscxr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jqsiufuf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ingcksgl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3eiqedvop.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cqwfdysq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3twwvhjnp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ktcvwvzq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xndezhyf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tixgtfsl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mbqgljsh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yljdhhni.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3heawdvit.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dpsotqgt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3klwjzqhx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qginizog.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kwqsmdwu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3gimclmtu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ozonnsjn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eyczctpw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zkmmlbhy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zlunxnjb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pongutpg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rvekuerj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wmmfcckq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fkyrlbhn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gnlfsumq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3saayzflv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sypqwuwt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3uauqjagy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ithkkcxs.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3svuaamjq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qivmybjm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kkbtszfh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ioiknlkg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tetdhquy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fkpkdybs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3opdjngsj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ysytxgfo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kkqogxqr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3stmvfqtb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3rkypkhdo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gwleivse.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3sblnrvfh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pxgyohtq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3irdefwjt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rqwzdzay.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mshjpaoa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3rjvoxwea.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rvqrklip.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ftfdzhix.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dcmordag.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nqboosxl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3opwjhbsd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jyxhkxwt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hunoidsu.html


<!-- 参考信息 -->