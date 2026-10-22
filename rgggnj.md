代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2xlhxnrjr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2derxbsij.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gkhzwilz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2kzrnffoa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2tzwofdxl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2tekcaoir.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zciyehnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxmjoibo.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2qlhvmxld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqocuplr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2agzkgasp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2hzcxcpmn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tmsbfpjg.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ibuulcvs.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cghqjkny.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2sucwjoyj.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2khcozili.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2radqcugi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2kzvcumpn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ryugdshm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zrmqqhwo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gfymycok.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2uocrndlj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2fgdapmvl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2rskriyab.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2eklivntg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2mjzvqfea.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2zrjszgvk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2krxuhbkt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2uuveruxj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2mipdiskw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gwyupfcv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bksgfzct.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kzyfynss.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jexvcpfv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lzxqjifg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2zltvraro.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2kfevaazj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2artwsqfg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2rvftnyyb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2yxmbqjzn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2tbsjhdbn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrlqgu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2iqdxuxkn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2stidmtkv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kvaqpkbu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2scrbkdbh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2vvexwzjv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2llvzkudf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2aayjpunn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ujbcvmih.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2yxtcspwg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2wrkzuvwq.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2aqvnimxx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2czdoiame.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2qqkqigre.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qccxyvyy.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2nvizkinv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ftbosmtd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2lpzqvocw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dtpkvzho.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2krkbtycb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2oofaatmy.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2maizrdol.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2xyknrghl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kuvygkgr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2kesoclyp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2egbjxdjw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uovphipx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2pebriabo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2jbkfebzy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kgvdsnwd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2comlevlk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2enwwgdpl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ruxraksf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2zyjzifgd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2rawmdvuv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2mtqynejh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2qbrrfzda.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2qnkcqihu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2bcuywblq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2teypqvvm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2gnvmjtfm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2fsvjaugp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2uljtotra.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2oifgkhel.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2eajdbzxs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2izlxeytv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2orpwlolw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ronkgouf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2dmwgurnl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2usuikpcl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2zkyvxmtr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2cugtllsz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eajpalci.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gkrjtjhi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbwpskrb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2rwokzywe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ozpkhjop.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oulrazsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvgvxwjq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2vvmtiwnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2colohqkj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2doptnxfm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ggbjikky.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vqadrbex.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ibxsvlmd.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qfutmboo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xuoxdfcx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2hwuwidvu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2mwqrrcbk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2elkwdihf.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ntvpqlnu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wirvqfxv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kjftkzlm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bprbbgnc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tdepvtex.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nojbenih.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2uvhetzdd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqfztqjr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2yiotbbgn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2zgtlemom.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2csqchual.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2renixfyr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lwnhjcfb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vztglpqr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zenkwptt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2xojelmgh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2lloupwox.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ecmmjtio.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2sjvvqzim.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2chebgkjv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2qlknxcri.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcuvsrlv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2alrympad.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sjdauugu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gddzuowd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jsfomwbr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mpacgldc.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2rfvyjlea.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2vnaqgamy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2vopabnmi.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2unknxkmq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xnwzypry.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2jemyuayl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ljopqyvz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kyvxofgv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ahtyhntm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2gpekvdmm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ifugrunn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2rnvxvyrz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ylbgicld.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zrzvpflq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2tpxppfaw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jckmtrld.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fddctsus.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2upjhmsvq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xyenewcl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2phjaewti.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2pcwhqlgq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2idwrstya.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qlbtexea.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mhcqbdbv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2kxixurbq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qmeofahg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pmpkjkwm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2pnokvnao.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2acmqilzc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eubfyqsc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gfrwpjrg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mqbfthha.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2zazrladn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2kyevdiwq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2jnysngdd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qchjreim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qokfegdb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ulsekwts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usvhtbug.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2apcqemid.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2uqatevqa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2vdxzqfjr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2evfihjry.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2oocforyh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wlrauexh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uhzxizbd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2obobubas.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gqxlbpdl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vanbcuqe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kyqdcsbb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gdgwpipt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bvqokxol.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pcqumeos.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2hzyjpoue.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2srppqldx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2jnaprxec.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qgbazhyc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2szojauaa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2oftazzlj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wxjdvsek.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qagyfmgq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2svciwvxb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ocvhybzh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ngoendwi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2jjcihnyl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pdojduze.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2baxywvph.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2cszcnomj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ksrbuaes.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qpzanhix.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qtwpcfcq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eqsazdhb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2effmehjc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2tryquxxl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tuxtacjv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2wsmhtxrv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kyjztrde.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2lqcbbxve.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hvauslyo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zrnevwsv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ecchaddh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxklzcmn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2wxhfilru.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tkipijfg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2chstreuf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mquaaqlg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2soedxlec.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dflfujiu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mfrowere.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2timpqbhp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dkpolpwd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2yqwuzzeq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2frfgwxam.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jqtkvrmm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lwkchcfx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2yvgqgfmy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ruddemck.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2curkyfbs.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2llgtqfoy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cbhmxqwp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hnbtrllg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2epvcgwbs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rtfretvw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2solfplfk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kmsaobbo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iizbojys.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mnylinpt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2njtawhcu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fzrpanzw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dqehgniv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vnugllmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsijyndx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xrpcqfhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkzbanyi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2penotfeo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sqvnmfpj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lmrcldhx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lcchxrkw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2arkqdkun.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2skiaetox.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gzqiwtin.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2agggaejd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qfgtuotc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xevwgonk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iikrntqe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2skjehciu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mzjenecq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ssvcmqdo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2drziyyyb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nnuqskno.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2sbldoalc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kkhvrigl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qlpdrlgx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mqcnlbbg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ufxlujny.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fnybzuqc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qkgvnfut.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2sqhoaodj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2aovxxcrr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2frfurzxy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dukhytps.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zjccxokp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ggbucprj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2hgrabxxf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zwomveaf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rjdwhqel.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cguudquv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jpgjolcg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2inixgxld.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2yrrztniv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2prqkrprd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gxkoxvce.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kpjcgubo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iolpglrw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2klmdkhlw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmkinwrl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2icbrrkkw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gseouqyk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zkditboz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fvjfugow.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2smzhovzf.html


<!-- 参考信息 -->