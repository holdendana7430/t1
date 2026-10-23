代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3jajgjsrz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ghccwxfi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fbtwntlm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3kaizesnu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3yeufonsb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3inyaekqa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3duflnorm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vptjjtxz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3mlvkdqkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqozpufa.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3fuzacubk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ybbwemwn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3bspxaxqg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qotkilxf.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3cwabhdtx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bftxueid.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3zljsvqak.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ybplqlua.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ykbfpxek.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xweordfs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ssmuryeo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jnkvnytj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3rfjmeslv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3cusjhebe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3hxvpfpmd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3kfhglnld.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3stpjgbos.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3pmpmjhnk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3oorpkkuj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3fkavezpn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3vqtojhim.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3udimsecl.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uslowzzw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lvkpyplx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wpdwxvib.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pkjotzgm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3tmrfvosh.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3dwvpospu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3hrihooix.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ihzouokf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3irmlpgsd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ooogwsyg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hracuwdi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ltoberwa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3igtvwlmd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mobtjklx.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3lujipcnr.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3tajbfzii.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3eqgsnmay.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gacfvyfm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wukeffbv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3vpddluia.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3btfbaacc.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3avkmrpkb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3aeoisqks.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3synavqbf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tcruixki.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3kvemjbit.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3elyzjafp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3yjqzpleq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3houqrfet.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3hignozsp.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3iesakuoi.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3wotaxqja.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3yixgtdks.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tvqhrpbb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ctpsxqqv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yyobkosi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bbnmfjto.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lmiztsbk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3doggmxbm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sibyieil.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3scblzjsy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3wlqdcugd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3qqcvgvng.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3frdtzfcc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3swukfbpc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3kaxjhele.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3zkjmttcq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3xoposhzx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3wsyvlwzg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3yrnipqlj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3jsgdmvwh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3qqlbmdpv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3byqpjddt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3breqaecg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkqtlwj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3iwsezusf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kqfbiduq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bbzqrfgh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3azdzgctz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3eqhtfgxm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3rnvipfic.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3llsdufht.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gcjzkxtb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mglzzpyq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ptorkvxk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3tyoofxby.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3jqlcihjg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqsjmgoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ccbdaypt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3qegjsagk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umnryvdt.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dkkdydqn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zpterysn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3robbxpnd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgzbqst.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ywydwgzd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3myozbmov.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzpchnys.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3llddlhbq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iajjkttb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3tqmxlndm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ijqpmjlj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3utsodlzo.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cehkidxh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmrggdsy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jqhsyfyz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kiawooim.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xyczbthc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3dzxcnmzn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rjtmmkoa.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ombzlflp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3uwexvclw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpcmkogx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bigvnhjj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3kxdbfbtc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3mbjibfsh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3urnkgino.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3donkljrg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3nagvvggt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ixxibmls.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3rwuohzvj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mccxolve.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bvmmnejs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jlilirmm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3spwogqsz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dtakowch.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gwofysbf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3tauaxstq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dmzklgnn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ofumisvm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lftousaj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3btlylpfu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3sgsbaiyh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3buzjrjox.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3udjtnqhr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3lfhiqtvb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3kjfnqbii.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tlywidzb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3wcnugsjn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dwrwiluk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3alogwfhh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3cmtwsyra.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3akezyhlo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ioqorpat.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3okkotsft.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3tjfiycdf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qrjzsqks.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3whkzqwij.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xvdviyoz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uewhsslf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dbbrampf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3snwgxgiu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3pvplixkf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ytvhzkbz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3aojjhuth.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dvgtcjva.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3uoqkwrdl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ltstzdrs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3azxefuse.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3rzdlsfug.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xjiwefrf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3usyhkzcp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fdgdpwes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbhalngi.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bztohcuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eczpkudz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3dufacbhw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ceafzmor.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3mzpeemwf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sehbiles.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ovcvpkwz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wqkhenep.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3wwmrqwif.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3imdpysdb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rvtzffvq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sdmfxtmz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kwjufrod.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3xcavhkgm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cbyzjtsl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nnpxpqdb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3bdgdatiw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3filmnfoc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fyjblzjf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mhaueykx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fscapavo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3opezmiwj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3hxcxfepa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yrwgagyc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kknnqibd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3cxemcrgo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fvxaktia.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3dffpyynn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3spxpsosu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3hriahjgx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3iotcwbar.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3idmbmkyb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3umchoerw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ginodpvs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zavcyqbw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3wkxsbgsu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmhbgsy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qyewsirp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3acnaqaay.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3qxfoxwwb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3bmpcqxpg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cluqtzmt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3asdcxbxb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3gebgzlqk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zgwmnxxp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3oveoavjr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3udzqbdsr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ajexukew.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bqxbkjwi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3jfjwemiz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nkyvavzv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vtnvbkkz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vrkfxxwo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ezlgwvjn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ekffxymp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hrgoyzzt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xgtxpqhy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3uoupthfd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3afkdnsts.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kjgbeujw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nwxvqxfo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3viythslx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jbwfxjmr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3celkaujh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3csjgyfks.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3oqmnpywd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3orfvkqiy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3utxzztci.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wywhfwhk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rzviskjw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vxbvveja.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3cubawsnj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nlizoquv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iqenkkfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyycqxrt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zzsnqssr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufpyplrc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yfblruqm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tyvwigwk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3adcwkzas.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xwfnyzaw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vpneoapr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zqdklbsd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bxwxdwpu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jawydetf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cpagosss.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mkkddjlg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hroetffd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cbjcavet.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ddnjagkr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3efakncje.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3szwcboae.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qdvvkzxc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ckgqqfok.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lxiqofdi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rjvzgrix.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3nccmduuo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3tjclcwpm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rmrwloal.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qweyzrfs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qqqcamtl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3intsfpus.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hgdgexem.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wmjkgqsj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xmvvdbuo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cmvzjxdx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hflslnrx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ywfqebdc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qsciunwd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3drjcjyrj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qmrpfrfu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tiwenfol.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bgzhpyus.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rlekrixk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdjuefay.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bhlnuwbg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hebbuhzz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ylemlrcm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pdpkvqjh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppspisrk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ppfukngp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xvbeahfu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xbxupefx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tmuzqctd.html


<!-- 参考信息 -->