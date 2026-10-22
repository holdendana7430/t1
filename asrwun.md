代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tfgwpsgt.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hhnrwzip.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bjbmoceb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2edjkvuey.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2fwgyefoj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2gpnftqdj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2hsmculck.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lyfddmxl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2jwqtxpdt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xhwpvmmh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2qobtabkj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2nzfspmdr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2fmqckkar.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ubhsnpjy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2yftkognp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2xpsgczrm.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2lfsqkrow.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2mnoavuaj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ifbuvhpk.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2icfwraoi.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bfewaopa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2szxczxno.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xlodztmj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rgolszrz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2wnvhjjqw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2hzljldlb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2mjxfxszz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2tgvkrsuh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ptqpyhjf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yaubnilc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2xturvxep.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ewlyvsiq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2hxtlhiot.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2owrkuymm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ctcdtlxf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2blswrkyl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2udqxcprz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjupwav.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ajlogoij.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tbrjjyvg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2vmdusmjk.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2qhrheupy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2kgrsefck.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ommnvoxn.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2znyrggmx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2nayeumqd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2cuodynop.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2jriyayql.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2nxtipqca.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2rnvfbxuq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2wgzwegma.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2utjqtcxq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2olfgfxjl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2sheaqjaw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2vloyxnko.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2dcgoqmes.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2coubnfie.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2cssykrrx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2rqjnlmjm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2fscruugy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2apziptms.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2mujqddlp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2kltmcauc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2myfpivlh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2sxryxcyl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2oyfksaby.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2twezimtf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2sjhzigjj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2hixbggiu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2lbjieitn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ccouvapp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2exdkbrdq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2uwxunsjy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jxuhgrxx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mzjbqvet.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2lxvwxaxu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ingspysw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2bfudywjr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2nbxntuvs.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2rprdcwlf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2dqmntnpd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2wexbigff.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fglvytbb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fnszjkcj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezhndmsp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2lwveqsvy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2yzlunyge.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2grgexrhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knbwvbyn.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2xnfffplm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fplgfqoe.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2stekkuvn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ocrelyxa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2igpcqeqy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2mfqsvchw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2grqbsics.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ipbxwknn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2kotpyqbk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2jyjxhvui.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2owbqvdjo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2aeaqlque.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vmvdedfk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2sbiojbcn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vfutrhmd.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edjhfqqb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2auojfkjx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2tnulfwhq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zvlucgyx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2vwvmieoe.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ctvdhiar.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ffoznmce.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bdevracb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2cedpxskj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sthjswqb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2gmavyvnt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2hrdawlyd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2cihpvnhd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2wpgdvwuf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhrjpbkd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tzbmskom.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vsdxukao.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2puhcpked.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2glkebkjk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ziucewpz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tlvvrvmf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qcvlkxzh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iyxovfwc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2lvvdeppq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2jimaojbn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2tudueyuw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2reeoimwx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bkvyumsg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2bpihpqpc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2knlxoqcq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wxsqrycz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2unscgyxj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2blnpjdzw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hurujjha.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2fyscuese.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fevabfzl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xjforvwk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mkegnary.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ancgpiwj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2khqykhzd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yuvkxxpr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2uomkbrdv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2matwdqnv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2djwrmtnv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2azimbtjy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ooaxyfhu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2buahulol.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hfuzaajx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2rhptuyoe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xdygpnna.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tuibanog.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qmkbpzoo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jnxfmtxf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wrogyaau.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qgzcirwt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2yxbciszz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2iygywrma.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gyavmbce.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vmhhslpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fybtekzg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bamztbzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtayilrh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2kmavusga.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ebzybpgy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2eazimtvh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lfbuicrz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fsjheoff.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2bgtigbwr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dmjaycgn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2pojhvjvm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sllnqpox.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2diqlydnp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2aajfnsfp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jzkzvibk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jzrgxczt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wtylnljz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fjbzzogc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2frympkjl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2pczcjzcb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2psafeuth.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2sopbzcik.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2kpxaxset.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xtndxsmo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pesbvxvy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2eecwkpst.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nhajizkp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hggmczto.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ebioaijj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zcwfhpyz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ppnwbrir.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ihvqnyom.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jparxjgv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fastegdj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2stbkjljh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2klxzvjdy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2vkzeptrq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qbinqiug.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vetamyng.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2gcpmqaah.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2syncbpge.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bgdjpees.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xlnfsecv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2oxogziua.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vjpxujnf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nevncfyr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2kaqpqqio.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kogqpabr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xvynwgtv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2duqkwbho.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2nthzfjno.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yiuibbcs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2chnhdrpq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wxuvdsqa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ujqnsepq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2tefkqjpr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2mpstcgmb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ekzjjplz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lnqczlfr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qwhcosdc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2buwaptke.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pkclwvng.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gqzwdfsy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bxzeyoir.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hspnimoy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kujehhpi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mipdhvof.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2grtrfqjm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2guvnjkdr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2srzmcfxg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zjlmgrrw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ntlnplld.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2szmdabbm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vjlociat.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2grpnqvzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obibqssb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2uhvkzjok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsigmlxn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hymkcylm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gvksztcf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pncunmxe.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzjcooyh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2oycojswy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yurevpcb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zqwhovia.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2irbrzudz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qfbbjrho.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bjeyyjnj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hxaafjkj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ytfbeuxq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zsavkabi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2neumelzo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fgwssscf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fsbkbsms.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2momoneco.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fnpfxusq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kmlrldyl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wuffbsvp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zmzxepjf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fuoleago.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nlehfkqg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2axnxgnwu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2lalxciup.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ggorzmgz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zizezhgz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rkpxqdyr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2azjifiop.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wlkbivgb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xtfmoqol.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fhmvlbii.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2meemsleo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hhmmxtbe.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2jvpkiqkt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2lknunbes.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2apzbhtwf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rdfxajci.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mzphunnn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2japybqaa.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ucshgbdd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzqmjepc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ldnrgzkt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jrafzchs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bjhucuck.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tvpsourh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zdbibuer.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mfdbjvqu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fzmrdvus.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lsofhzxi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2odnivben.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vivdpsga.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lpoffhcj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2kubthuwo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2piwxyscz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bgserpsj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hygerpol.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lzhjbjlu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2glfkyvcd.html


<!-- 参考信息 -->