代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3fwoyfgtp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3adoyseia.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3uleswycd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wadkyrbd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3kwyxsjwr.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3euvziylq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3kjcortnx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3oijpzvxt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3gbhwfjtn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ptdglgii.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3fajvfata.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3mkwakuty.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3mbausnpv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jsdfhdvt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rraxpekm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ckzygnce.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3llpapgpd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ggqijziq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ffpnsjve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhwfukxf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3unyzijge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txelbzwu.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ahhktqqq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3cfapnqvx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ltxszvwp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uhlyfkqq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kxennmdg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zxxwoamd.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3cepjagqz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3auakcwsa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3imuacbob.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sfljkles.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3dhywkcfv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vxtfxedj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3zqpwfkpu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3cpgtutjc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ewaxhnzs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3qeoxkxjv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3oqaefgij.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3clsloroj.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3qizbvmrd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3usoeleos.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jianrrxi.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qvzuydmb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xneoofov.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3syojngwz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ajnkqzrs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qroapilc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3arrxrmrj.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3kniaktxx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rqlmpdna.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3jdapqbuk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3udhswoxd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3btykgsem.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3ppcrdprs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3evvjpjot.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3qxxjrkyl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3xqanwbgh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3eojmbkvy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3aappkyid.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3dyzyxbsi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hyxesily.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3naoraoke.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ubovvfwc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fwclbhpn.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ytvweomq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mzxqesrs.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3lwhjcvzk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3qzkzabfw.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3taignhtw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3poecomgx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3twowxssc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3iwvrunrb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3lebccunq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3qaipkapr.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3urqqmdkd.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3gqqgexyx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3npfzkpvh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3cujvkwnx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3myugenvf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3exuyetfk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3yvgmrhog.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3witjeand.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pevxmepk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nvkupgrk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3woabfzxt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3xyhcicoy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3zljwjuhh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3eqyqyham.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3dnffdutl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3pgklxpwa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ntjbcrtu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3zsmjrqfv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3tbbgltzj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3qbpvxcbd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3rvzafsdx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3voypagny.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mmimpczf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tissutmq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3nmhrseon.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3tuheqcmm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ubzleyel.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3znjlkxmd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3vgrumdct.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3puvommqo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rywijbfv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wuwtsggh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gyrhrphp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3bbdarhue.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3mbxvbxzg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ylndmgwl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3djuoofis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itnqmvia.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3gkgqtntl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpmzyxqn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rjqdltsb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xuoxqcvf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hvggfijv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tfrixxrn.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oxhtvvcd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3rhakhwxl.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wqeuhspj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3qojljkyo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3loszhpnz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jgfshwdw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3hcuvorwv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3immnnjbo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dabqnsvl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehwpchba.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xlfwsdds.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3yptskucj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tooacosq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3mvohqcne.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3gfsoilfq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3lthcuvbg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3okpymzky.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tqmdtxjv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zudihbjd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvwdjiy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3rxrsznzk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3nutbnzyo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3hbifjqik.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkojtftn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tewozgod.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3gsnzzgrl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uwlfsbkr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gzwlxkhn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kbwwamkq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3yheaftgv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uglewxjn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uwmpalop.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3wqduadoc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3tvulaapb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3gimepedm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mkpnamec.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wtsoweiy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3tydtwofr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3zekpnsfr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xdubzkpb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3earmbopt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3efqrajvy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bgdopsxp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ogqgppnh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kbmsyyxe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ubmrfphh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nafryjjv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3olkerbtl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ymomklqo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pvhidkhx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ocoozchc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zzaebbqj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3rgomugwe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oxecoyob.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jyekycbc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3creqiurh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ngggcmpd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ylmtbkrx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rceunhmj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3firvdlpw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3vsommmsf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jrkydtmo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ayvphfjy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mxnfvwod.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ojrchmoy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3wfcxganj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3zdbcvrkb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gotsliyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsxfttmb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vffuqziz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odqqcyce.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yuncxums.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xweocwuw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3udlylzrm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dluxmqcr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ctuxeqnr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3axcprozv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gswrluzq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ajojsctu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fpntyhky.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ryaozixv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hgnxokei.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3krpkwzeu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3koncknyc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gyelyoau.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3chxrumut.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3zgzhvhcl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jxczujor.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qcotspjo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3qnwobntq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fjqjheqg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3olffughh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3lzwaahml.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jfpxzsgs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wppllmqf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pgsgiice.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3mawtwqzh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hvpnrifv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3jarsqkbp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3xwpehcme.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tbflhpqt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ovtestxw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ktedtwpg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uvkukgia.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3papsprfd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qzbapxjn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qbedqywg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3grirfliu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3pnagnyyg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3akoahfsl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bpmdolod.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lzwsruzd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ihrytwgo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3swzujodj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3cbcvxopb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqkrvxli.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cqfcahcx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bljvyize.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3aeuacreq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3htofcwlz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qwenvegw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jvzsadpr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3przqkfyn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3itzmwuct.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3lnkcekij.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zzftrhyq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tllokdrh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3oadwmvnj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3atnxetou.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ifbnrejw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3rgzmebzw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nmvaawpj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3yqdmimzd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kqozfgmi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tdnijzxz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hdzxihit.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3oyxgmoqd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3efwzdvxb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fvwfryir.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3llvhkeok.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mebbwvvz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3iyezqbou.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3grilbycg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehbivekn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3iyogflwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czdvptqh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vpucewlq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mjgotuiw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3yqkmktle.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dzmsmhyd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bgeytjej.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zesgjdhw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fvidwtsg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3idwnjgfl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gzihcfat.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oieiprbv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uawgydzu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xnnmehfz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pqgxlzlk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xdkinnzt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mbbswyzo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gkytfetb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ndstdueb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cykodqfn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3uzrleapd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3botfteyx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3khlqwqkq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nllbeqjf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tcfbulnh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xxzvdcew.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3szjciych.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3tnydwqrm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3liheljed.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3aknghepb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xxodetpw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3dwhbxbba.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qpmlirie.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lcwgqfzk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zhzcaika.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3uuomuoda.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hbuaqekw.html


<!-- 参考信息 -->