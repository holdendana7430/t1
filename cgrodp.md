代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3qgxubymg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hvukhcuu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ontfkyzn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3gzwcexnr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lmmhvtje.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3fliyrsvv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3mlxjvejb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3aotbwthy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ljovmzvd.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3tjjupuuo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ydfqdgeu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3cjnrgman.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3mozriveg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3brnvglky.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3wevqksgm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3trbvpzdb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3easnxrdc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rhrskecv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3yfwnyssd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3yroiwpny.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3rmyeuapz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3yfvikcaf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qhofhpev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyfxbwux.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ccoqltku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcymzxhz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3wuijvdee.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3xlkumkpu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3aurpeqtv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3sucykyzn.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3pfdbcxdf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3bgstuwxc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3pdaurmrb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3bsvhuvsf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3lkcpagyw.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3csmphayw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zxobdsus.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3shqxxtxv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3plkawreh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3odmxuxkl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3wgxrsoyd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3qyegdwsd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mlxppaln.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3bzfjuhjw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3etbkmxax.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3johgkdus.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ezvfurnq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jjvjcdqz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zwbflckw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lcldfyik.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3joseopyt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lulnhunr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ckiwtsue.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3wiqzrrbo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3sxduhazh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3gautwrhj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3pddxrqmd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jofoteer.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3izplhtpw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3gpfbclgi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vqaebbvg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ouyjvczt.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3sillltpg.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3mbgpxfjs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3tfdwaurh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3stprxxnk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrhntpm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hbrplgve.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fccyjyni.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3uitufwhs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hcvqrnsy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3zvbbypge.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3wqhtrlog.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3wijztutq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3scgjyzko.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3myafeeir.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dsnfxnxn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3hmdmeokf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3mzqhftvk.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3wkrvlvny.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ajxarxpy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qhkpvtic.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3gdsvwang.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fiajatau.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3gefjkcaq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ruebczdv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3iyhfgram.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ausxvjya.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3otcdwost.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3zdgaomel.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3foyockbm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3nzstgleu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xfklysok.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3cdhcsxff.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3fwdauspw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3kdcmflkv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3gfhlyzpn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3omlqqyqy.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3kzskbgjo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3eizsvjfo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3hllmixba.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3jntzmyis.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hckhzidr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3xjfuvmei.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3perovfuy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ltmbvrwj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3csbabsce.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3slcbjlkz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3uphmvecf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3rbreespy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ftfwbycr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3koqannxe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cmlmtwfu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3yndbqjbs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3pptwdvae.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ywxlblkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsgrvumm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ezccwwwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apohyzod.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3komsvzar.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tpofeykl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uirvomks.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xbhyamin.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajvbxfsf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3zoxucdoa.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3dqsldszl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3itligrvc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3umgpwtzr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3zjhyilen.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3hsvquuei.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3cijmmyaj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3adwfzszm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vaxihsbv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kjsowuda.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3snifzfxl.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ysbrzayr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3aihedmkq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3lfeyfaxw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tybdsxtj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3twazrnee.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jmkepuzz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fzftvzfu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3lirvjdps.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ihbqzwcu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nlbgkrrb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3hvwijgtb.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3uykhjczd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jjcrnlqt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3vmtodzmi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wwquubiy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qdcdpymw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ketkwzlz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3adtmpimd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hwvculqq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iyruujij.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3eitwyxga.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jsxidwmp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3mjdpidhm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dpywbfnk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3isjfgnfm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3yzsmpdrw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3leflbzdf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jltqbxmq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3axjdslby.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3mapzblyq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xbknjltp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3duiqvwxt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3idwedyyw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kelqjowf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ltcmhksu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ogfojlma.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ikbzmohh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bakogvck.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bfomiiqq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cjhfimlq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3oqmyndvi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3naoxxmsz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3btarnvpe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3djhtlnff.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ktwbxklo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhwzoso.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uoingpnu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3yukdcxjh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3lqhmimtj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3igqtispo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gtvoeoqm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3etcoldgr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bwmdgnij.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3yarqtsju.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3jihmbtqg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3psvvgden.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igifaaud.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3umgaxkrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxuxaork.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ucyeoauw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3zhutaluy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3masqpsjw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cbckccku.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ghorwjqe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wpcysxhq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vdgvlzuf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3lhuqurvx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3mijioeyz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qtbfzeqk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3skxiftta.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3anczwyic.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xmgqjqvj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zrrxtigg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hdzwmnqd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ipmgjbal.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3elivrunh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3jefaffci.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vxpidepk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3eodsnxkv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3odesyggj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oqafqkoy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cupmxooc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zybhnpst.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jlfdhhfr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3rfnuggob.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hzravnqp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qjadhlzq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3yanhyecq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nsaxxerx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3trdhllad.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cfgcubwt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3gihpmdle.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3oinonjyw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3fcvdmjav.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3sytaupdk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zfeaqnyf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3nsstmorv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3arfxvkws.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rdacqdvd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ejbdwjxl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xemnqhdj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vfeqyvze.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3plelznwu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iabpnigj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fpfpbjxi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zchhwpgw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hqcdkqtw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hbtwtnvo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3prdvyaqj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wrawbcba.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wetlencf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3czmaziwn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cygikcui.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qjtmsfeo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hnoczmxp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ujavygtf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vnciaatd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hxcpcwuu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3smwnhnhj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mnbsputo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3agcoobio.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gibottwp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3geahmqoo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3oeqlflgb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3pyuoowyg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ekipwyva.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3komknvwa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3svsfhzwi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mxqgtuna.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ififoulf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vlviwjve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eniiwpgo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zgkqdpho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euggltvj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wdmrhvoj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vqqwsttw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3cxcbitao.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsucfqmk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zstfrckp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ksnemlry.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ggxbwqcn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3yzavzqpi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nlkvsxjk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gjndzpgs.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ctodqtme.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jcuywvhj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dzahyuqm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3negdfutg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xhlklfvl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hnqraiwd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wccwuius.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jbfcaysy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hrjsrwrj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3epbpfcek.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qbauwype.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cdlcfcux.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mkneelex.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wzzysyjk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3gpgbkfvh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vbwwmujh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3riizthwm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3inbetcjb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sojorcwg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ewujwbso.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ywrxmegj.html


<!-- 参考信息 -->