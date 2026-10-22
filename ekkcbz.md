代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cafkvuio.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2igeqqety.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2oicutfcb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2gfwasfpz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2gxsusnmv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2htchscwk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2pbgqsopn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vserbnmw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2mmlpwhqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcqpowah.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2mgkadtjy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2epmkekfg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ockphnlw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2awxxgytt.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2spftpiwy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2pruyrpji.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2rcywfgqd.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ssmfnare.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2vmnamfyp.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2glhadwdv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2merrgfmx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jxjiwojd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2kafqxmez.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2folosvsc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2exdivtok.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2cwtnygss.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2lkxujrnz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2iyxgcpux.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2noqancya.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2clqyuhez.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2weutqlnp.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pudfrzte.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2prlfyicp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xexixlos.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bkleplhm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2slqfwrjv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2rvhlphgl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2wuvnaqol.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mtiswspf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2aooaumbg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxruaqv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hnovdebl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ytijhzwt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2dxmnsfkh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2bcdsgsne.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bumhiyrn.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2kirfugfh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2seyefblf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2zxvbcrsl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jfmawpsj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2urochntc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lmwycvwn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rxkwjdvn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2kmcqorxe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tyzmktap.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2aedcwoqg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vcdvvesi.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2flywucuz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ghfpkpoq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2wsbkxgek.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2tuogeikx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2mniemias.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ibzoxdpm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wzlvgiud.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2tmmtsrhn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2sezypmok.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ikdwdwpw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2cregagfb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ftifquie.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2govyvhtt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2dqihgodc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2mtgqrilf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lmyhrmuo.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2lyfmqpom.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2xbdckjed.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2bfwihzsm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2hkafjnyy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2tuoratde.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mcuhobws.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2aajhddfm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2oxjopjft.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2eylvglxg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2hhbaspjn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rccuwymm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2dyxkxwvo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ldnwbide.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2nqrjraua.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2fldlrdss.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2pdauilos.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2hxkpxfja.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2okolsxds.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2xdakehzp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2cdkkoerx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2vphfkrck.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2xzjjxguv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ovsqxzix.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgernvd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2wltmnekd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2qwavryub.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dirofhur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kynmqdsa.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2lszgkkgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aygowdmn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ctjfqfhj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2dtzsrtvv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nneiepem.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dzuoaptr.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2fdpvkiza.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2gfhqfora.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2xiskfenm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2mnblpzwr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2uchnmixq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2rokszatk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rvknxztu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2aanxwfxh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2srlygwlw.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nelvizfz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ecwipsnt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ioztnvwn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gynjcbqj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2btlhlyby.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2blbopxic.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xabyivpu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2yagqauku.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eminibfx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mazlbpzh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2aqvfqtvh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2pheiqzmk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xmovzfvi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qorctauj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2djccyjor.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jbnsxuci.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2gwoqoicx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wtzlbkht.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ultynrrk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hqkwkxwm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ejztwspo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cwutmovx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ivzolrvs.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ndivryre.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2nngapupv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wpecmmkj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tfalkvyo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hjwvswxk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2fywegzxl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2hwjjyiaa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bqqrufpn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2krkgdlzp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2upzypfrx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mqqcarox.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2espagkaj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fazsnlba.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qhudinaq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2csvgqfls.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uqyhgjdh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2swgobvni.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wpmkgbrb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2rcsyqtee.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fabqupln.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2fewxvkpr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cvccinpd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dflvbmbl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dpshqtfa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2exgemrom.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pbogmiwt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zusdwosq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2spwnwmnk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2onvbezbm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2frngpyax.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2njkccwmb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gguuzumd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2cyttoobe.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dpkkywsy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2peixlbhn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nvbewtwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcoqqlxy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2lynhsrai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxlqjbwx.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2npizgqje.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bljhdgwi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2pcnmmvoq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bbhrabpn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yrorbozc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2cskfcxkw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zhqclgxz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2haypajni.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jcyvphoq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zxcdoqqx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zzmgemxc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2nfzljjkz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bvfzpgjx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ciufjufe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2guulkduu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2lwnxsgxj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2szmdhkee.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2demiyyne.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ilzaowci.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jnktkdoa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ivkldhge.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cyqbxbit.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nshvzbfg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pdagbsmt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yhrrskon.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2trlavnkj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zdiroked.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2swgkbjon.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2loewrnmp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xaqjwqud.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2psddfocj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nbvbiyvv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bcmemtuy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hujumqqm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2berukxib.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2oovgccdr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2nofiehxr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vopupueg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wzehqnaz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hitposzh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ifutxkus.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2pixnmldx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2erpspegu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xlkflusj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uyklsbzn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2amzlqfeo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jrmrfidt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ebgkilcy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wzudvzdj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qqephpaf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gxzjdcky.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2kwvfzwcy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2uiroxsez.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zhabfhwp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jpabujbh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fcmmwxlb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mesijtcl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yzjhiyxp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bemckqlo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2pjsbhqkx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vulufgco.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2spduvmtl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kxngtfrn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2bzlfkdnn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2tduiqbut.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mplwxemn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fztnvbqg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2orezpgik.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2jbocasav.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2emuhyrkv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wmqxefpu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2emrcgtvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcmbkxng.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rjadygan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuzlkpjc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sdmrttzq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2nnfqbxgl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pqyfveie.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2odpwmecc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fivkjbix.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2agdfkzsb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yvqjbgda.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2sqobavfz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zkzxnzmh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jkieipyq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uaqkglgr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cusydnmd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2miawwtjn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hsngtykx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tengahzc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ckxufkql.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rqwdhcru.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ghtdrjyb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qoqbojkz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pjxknpau.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2yqfgsxau.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2biijghzd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2schltizr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dkyhveab.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2iipxuqzi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nqfiyynn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hnsmcymd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xjwwsayp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rvotvyms.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ugmrsvqe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ihiraqwm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yunhsjjb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zosvpytp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bdvsxkqs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nwuarydh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2dibhwlye.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yyfruxew.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekesgwpn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2baznzkyt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tqizxfob.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dqmnpuqr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujivovrg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmsbpmuk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2sghpdslp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mropsszz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2durivapk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2weowqcil.html


<!-- 参考信息 -->