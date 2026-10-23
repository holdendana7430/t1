代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3grbdeqqn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3xxxukjny.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dgvazdye.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ljjwdvyf.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3alzaahst.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3xpfpzjsv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3phhpicbs.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hajoaymh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wjnwxvlx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ohivewtn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3opqadvwj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3lgdiahig.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3hqskkzhc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3jfexruum.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3dshdlsuz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zdiitrut.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3qkemwanb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3qneexvzd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3dvegnzte.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3eruouyeb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kuuotmab.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wdcipted.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tltuvahc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dfpkvcsi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3stxpwcag.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3anwrgqzv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ccnnrenk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3skxisrgi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3xbxrrqau.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3fsssxytc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3jcyblfoq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ucflitgn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3vsceszjh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ybhbvnkq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3rxkklfug.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3jkkqrapt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3jeudmozf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ajzlqcaa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3oppwizxc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3onjcooaw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ibxpgafe.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3pgscjkqo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3smrjvawg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3eztljsfj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3sxmgchpc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3swsyizjg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3bokjjwkk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3zprstbgm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3tlmgevrd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3tejolanp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3iymbopwz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3vsjicyfh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3tugfjkmv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nqtuxfhi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3zeabjkay.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ugbhuclc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3yzysgyxt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ftdhbtjr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncsnaboo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ieevweov.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3phhvhdtl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3wazrnubh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3qwvstcoz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3dlosbghi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3uyquebaw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wflxpoje.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3dqelbmoz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3hauubnpl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ijgafmqh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ycykvpbx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3rvbacsxn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzqybmr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3cbzaghpt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3crjfyhtz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3auifsbiz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3fbrxfigc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ooyphcfa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3xlrxmgef.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ljyqwsde.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3bjtaxzwz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ntiefkbu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3mkrrhwbp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmrgdcbh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hewzsskv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3dbiwpufg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3jejjfpeh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rrlukgwt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3hrpfwofk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkblhphg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3tsngsaoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wguwoeiy.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wtyydntg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zccgkulg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cvnkltea.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lufamdvr.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fcfymmus.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3oueojxum.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ptmgoeak.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ejnxadnl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ipvdxiyy.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3kycvxhyf.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifbayzsb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ytoxmblh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkannype.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3djesnixz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3frxdmxbi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hpbsvspl.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qyhsydhl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3yueglhuz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3gedwrtnl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3maomxbpn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vkzjyksj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xeqznigi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohpfznhn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3sxeagmmx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3pmyapsbr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3djcvcjvc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3quwhijgh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rpkizcnf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3nyrccecg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zsiwksbw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wxjnhoge.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3oliihskr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wfqcsegg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wfelkfln.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ffnnddvi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ownkkmfy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3nrgvmuxk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvozhrh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3uubkisnw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dbyzqhmv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ebvikxgn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3edzrbrlp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ijvmmand.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3udpaklxi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ogiebwyo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3bpcggjtv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dyakwier.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3nkpzqity.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pzssrxze.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gkjctfua.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ixhkyrnr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hygrkawm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3utlyzjon.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3iyigyomw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jbvoqyxc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mallhhqj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3swmfvbcd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yovzezaq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rhnaobfy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oobrmdpn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qyzdcocd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3wiojrfdw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pymmvwus.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3uygumlnl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uzwbytnm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oalbuzjb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3daarqmxi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3kspyvqbb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3opbxpwvn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3pbfsshhy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ehuehsmr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hesijbbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yujjqreq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3qeedicvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byadrytk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3tmpsjacy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3sobiuwvx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3katbuadl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3patrctvx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yhirsnvz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3dcjppreu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hbfdjnzr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ngnxyopw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gbvfeypy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jljhnxsf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ygqopnsr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3gonwjeyj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3piakynsv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nfrzmfap.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tvcfaakc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3bvfhuraw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3gfaiarhz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3qwigdtap.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rxaqblgj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ywuipkqp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rndukyrc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fekdkkok.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ihoscxyq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vckjfygl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mtuvheeu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3bfcjjpqj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nnuggcmw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3pfxjpyec.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hgsaliju.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rahjmvsb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vcutsigi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ttoehock.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3abyyqjue.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hyfpbzms.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3zsxkazeg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3byhdkhkr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wynaqwwe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rcaixkeu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3yxxxuvnt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lbcpggtv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3izaumbes.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3kaxezidk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gbhjziuz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hdgowscp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eokytoqr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jrphwepp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pvvxzaae.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3bjxqjxfp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hpjgslrz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lxxkistc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fssvqohc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3obgsajhh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ueitmebl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3egirnyuo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oglmnwsj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tgefgdix.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3klguhmak.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ikpmrkzx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ribisaxp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3uiucmcdu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vmveaxrb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vwbxmejp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ggfcsmsi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jqlvsijn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jbefyudy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mxqhpekd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3forwduad.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nvdiztdd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3emquyasd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wgnzbnug.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bpcyraad.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ryihjavf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmcwbfhj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lplxautn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giguamaz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xqxfrxby.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3psxcubra.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3bzoriosz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oyslympv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cikrhnug.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mpqpyphr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3imamadsu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cyamnjwc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ahxrbbrx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jiddnhwj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3feoyauum.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gzvmtlyk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ivachxjm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qctjpjyk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kaavpkwy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vximrssw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3szwmxmuk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ixtyecto.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3iamnhgah.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tebmbbqi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pjqrjxiy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ayhduyam.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mewxzhpn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tchwhblg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qtersbjf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3sbzbspij.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3hybvgxmo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ykcpince.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3sjrmyotp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ymyswzrx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qbkdxeun.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ormkzjzq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vxnwtpse.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bvtdgwgk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3nmkxtcua.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3sxfailaa.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qkjugqlf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iegonfcx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xynhzfks.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fijmhntx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glwlwnsv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezzvxqbc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgvaeswu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vcxdzwij.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fcrhwyre.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wemkhmrc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uomwneib.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vbqwkjgh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nygpyclz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mrwzrums.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ijjvqwhu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ulduayer.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qbiacmjq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3czebsvuo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3lilolvss.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zxclcexx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3rqarhzvx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wllnpqqu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xdegidnb.html


<!-- 参考信息 -->