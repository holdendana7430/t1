代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ssiodhqz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pzphgges.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3durirwld.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3vgkhhato.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3wktonlra.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3zwbmcdbs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vsxlustc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zffnmfqz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3vcliipag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zppjuepo.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3juxmtyrz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3hwjibzek.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tpxuxmiv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ugvjpdpu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tkqdnazp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3hidxdsix.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3dcfekpeg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3uaddxsrx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3hnbfmiah.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ezjayjzl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3elinxcxd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3euhkvhas.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3jbyvjyya.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ytdptgey.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ccfnruup.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3rwgatnxo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3egdlnicm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3hntafpmz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3jqqpdzas.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3cclfhkmu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3hiospbwp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jhffesxw.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ljmnvgka.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3sourikyk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qrodhrev.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3olqdpcvf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtjshkz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3lhrwutuz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3zoiqusks.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3qsenbqtr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwfljrn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3whcednny.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vcjkshhp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ixsedxne.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3tefcwiwb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3gpsqslfx.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3grrypwpf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ycpyenex.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3qmxcrztf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3oskgiqak.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bywerwbc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zxpvyfru.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rcylilsd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3dzagozja.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3agswdjdt.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3qqetiadu.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mmdfrpwv.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3hvpamdjl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3csdgomgq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3zxqljecs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3oldvhomi.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3fzszapcc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3fczfbxvc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3hefscelv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3rufrgewi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mupksdlb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3qvedxqis.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hrehknxp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3anjrighf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3yzcqfqbz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3fixzmnkh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3veppmmpx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wpaxrjvz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3mzuudkdw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3rtscqhme.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3wwgrpcsm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3vsppouhd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3oquyijwv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3sorumjuw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3yyotodwa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3rhonegbq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3maaerxlk.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3nekyqddz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3gqartuww.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3wpvgemgl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqgcaos.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3znfsygrz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3vfsytupz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ggzeveqz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3xfrwcbdh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3wifcghcb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3adawykzw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3naoeulnf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3dmaursul.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pehjokly.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3totytqwu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kaazsluy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3clthwmta.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3tvvxazkq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tyqdolkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adbtcisj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3cnbdyrba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ookujtfr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vrpncdrn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwgtqmm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3slcqefwv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nljwhrrh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3axeqmrgq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3cdiimjvg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3alomfxsp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3kfjknzmo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3emhiovsw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3whlflyvh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3hzrpatit.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3aczcogtl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3glukfbma.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ewygjxvt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ltzwbjri.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vonjerfz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xyqsppsj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3kbsqhftv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3kszloamt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zhpbiijo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vvjflmnn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouglecvn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3usmmtsod.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hbozwfgr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3rwcwpbba.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrorkfl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ravgjqls.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3xojghmcz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3eplauquc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3cbvcqxjk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xljxhicr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bvtbjrxt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fpokxghv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hggpukmd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3svctjhuq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zkrnhtct.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3vvwxfgoq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dteqwnom.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3olnubjcr.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dcqtywnl.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qqeuqpfq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ecdxbnfp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xwsgflxc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xuhshoix.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3frtxgnxh.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3uueomwwo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3trnvqlkz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3gswmoujt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3htncxlba.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ncmzsgvu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ikfhfkhu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hhfchtem.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ujqhjvfs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bczotgux.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wigmfaaq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pwmlyolm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3xdllwtdb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3abjaxgrd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pvnvxncp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3evqstjrg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3erzhfqcj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wtmvbohb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cpukrcgm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ydwlxdvn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3inpnielg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3yghkmeyx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ptmsbqrx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3adsfihea.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3vvmomcdc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3tipqyymu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3vgegkspd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gaacckih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iswckllc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3rcrcedde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivisqckw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3srzsaxih.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3cqmdzjlu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3hcqreloe.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sqywfpfs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rwojyick.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mrjcadwb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dpydexyh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3slbbdamb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hvgznxky.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wpoydgee.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xuwtizxq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mkrlqrho.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3efrlgqnq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lcghmnap.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3spsfidkc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3irjsajyk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3sgqmbdek.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijumifnj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fpokpzba.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3zjqeqymm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvaljcvq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3agudzhog.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nkzrybzw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3uecngodw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3odpkjtpc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xzhemjdg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lahrlewq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3tniczwtv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3wrkkugvv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uvdkrllg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3itntbsec.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ebkmrawq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3brkuysap.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bimtvzgw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xmoczwkh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tvvewids.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qansptkx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3jrinfkrg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3fxkpoosa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jmlusnov.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rfmxmzrw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ouanbhwq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3arsgkrsw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3aujelzba.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rcrildnf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3gkxancew.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3smtgzxut.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3yudpzsgn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kdmefhcj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fdnyqyrm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wqggsqhd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3abwhkpku.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gjdnxjir.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3krjsxpne.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vttkdovo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jtgxzrfm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3omfbawoo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yvdkacdy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ekapqjkd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cqpfuvgm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cmylbzes.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bhckffbb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qlxdvtgp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3fxfhkqdg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3nrtbhxpq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wsbttmdc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3smksnqyd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ooptcaya.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3jyagmxbr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ombyzhda.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3prqmdkdh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3dlorxjam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lstayhxb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zbedjlod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppjrnecj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3aguiqajj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pbzlgbbe.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3zoadcvvj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fqznrhqi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lisvyqwu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kscfanni.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3efbxjuma.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gwhnuwgf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uiprmuvw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bgetcphq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bfuymmji.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3osofgorn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pwilghdq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wnesucja.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tqulexur.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cidzxbyx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mbinddnh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lzjolxio.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hdjknlew.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wnavhwuf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ijayvlzm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qvjlwuvz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gqpulvlv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jnlpavps.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ikdeueeq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hujelqmi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qauzcnbx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3amymnsbd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3msffusqz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uicjqggj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gzkdqtuw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lxdwrmqi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nlgrjuzy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sxunnhas.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hgbdggye.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3pyfpvqsp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3nvzeozdc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zqyurhit.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fnyrmtyt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ixwwaakm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qhwtcobq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lmncnkil.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lfxqfhue.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3daedtkxe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3olpbvkio.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3czhliecb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vkysfswm.html


<!-- 参考信息 -->