代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2hhisbwpb.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2dncolhkh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpmlypz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2cmxpwabh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2symvbjum.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2smnczycu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2settixzl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2nkxnlthl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cqxvdkme.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mxnryvjr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2trcdxamq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2pvrtrcxf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2csfrvdgs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wnwbjpjr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zzbctqha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ablukidf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ijkzsbfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyoocyrh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rpxswhfh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ajykvapv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pzwxdlbn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2lbaugyvc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gwhvytdr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2cljagskc.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2jrllxjra.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2nrjkdjjf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2geiyinvi.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2weiedgby.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kmshyqjh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2fryabqrs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2gaofaysa.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ltoiuanx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2chxmtzjb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2dsqrbvyz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fdpyrrfd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2rolbdanj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2tkmdfbbf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2wvgdrain.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ykvwdndf.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ysaysrcz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xlqetvrx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bpbxevha.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wtwhmbtj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yofkqohl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2uzwvdjga.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2xtyodder.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rxevixdq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2brvsnkbt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2dgzgpkyd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2edrgfrng.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2blswyfvw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eoftikdu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2yjcvhokx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hoclxbit.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2drxgrjza.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjelibl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2hdekrhsp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ujopkcqs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kklcxhmf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2crvnzcag.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sbciviay.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2sqmszqjv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jeutjrak.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2diuifeug.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2bescicwr.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2uxstjsqx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2nxmibvai.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2tgytciyi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2sjsbbame.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ymutrjlx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2whslundk.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2txvzzajs.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2sptyvjcz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cdpvkcfx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2piifnytp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mirldcke.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mgourzed.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fxudotxp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujpkfopc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rpfvrdto.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2evgmuywy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2rvxrxoib.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2mhccomtc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2daqzotsy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2btjaasjd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2vhqtjiic.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2yklkkqqz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2fvpmjhpk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2kobxahgp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2urnkktzg.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ykluuska.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2wdnkdwns.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2otvadmlx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2neixeomn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2hfkwdjeg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2hrpbpioy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2jytlmjmm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2szbkrsqs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2uokaejgb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ekayanwk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2balnqgrs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2inwedsgt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2wdjxkimb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ficxumth.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbgblkwq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2swhmziun.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2pphfzhvx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffnlkfkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qeijywvs.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2lrtgonez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swnqghmd.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2iqcaekaa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jmsqtwbp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2avxjfnfy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dsmgqiyc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aruomhqz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2vfzwyqaj.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2fyklsnkt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2qifbupqt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2jjrdeqjt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2sfltoehl.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2eggprktm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2cfmfrfbu.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sekicsxx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kinlodux.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2crwjqgbd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2eccihofn.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2trwppucj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ehcwbgqi.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2rflmaqcs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2hyidotpn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rcvxxacv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2avdvhfev.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tabprtuj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rqqsysky.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2noxzoudj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zdltufrs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2gzfabbwq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2icizulso.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bddguucj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2palpgvnd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mbfgwlwb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2lcqmivsx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fffchdso.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2uojopbxo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2moltuxwu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2svgwfyfi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2psqhbyjg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rtxxylnp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nwrnwdqk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ozaaqvjm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vcvbfxzf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2vvwumfdw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2candetyv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zsvabdys.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2wjhkpirh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2wddxnkpe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jpqsyvjr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2gtkukeos.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jmsfqxta.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jrtntsjo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2szgasdjo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bsvnwhux.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ezkhgtai.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nqnwmhnu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jgsdxcso.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hroopnne.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ymgbpajn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mxjblhjb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vznzbeeg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ixposjnj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2uyolgayl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qghfsool.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yzpcpwzh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dtvdvbhx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2wonbbyuv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mygrdgjg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wtsuxwpd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kxfetujr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2nlyoulbc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2kwjjejlp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bfbuubtp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jzrjrein.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knjaurkf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2slyxotcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrylksam.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jmesusjr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2whmqacre.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wwhqsefb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tgbawljj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qjunzosi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mvvlykem.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2phsubqyu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2twbidyml.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2awcmyuvc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nzrhyavr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lhrvsynj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2tjtgqtrp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mnaabyuo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rdjxxyek.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fpmnxwrw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2pgjmfjhw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2sfakeomf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2mtzvumuq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2uknbgmkt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2nejdthcd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gapaxrud.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2utkdszes.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ruflnrns.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2smwirlrz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kskqahqr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2baxepoyi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gsufftcc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2myrczdwz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xvlkqyvr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cvcdzamr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nrrxwnms.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2askuntbw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2fxnvlqhf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bxovvrlj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbiwfyd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kfhcwgfb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2eleydfxy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vwxnweon.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2eysftozq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dkfusjml.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2diaroyqy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hjnkkwwu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kjjznjas.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jmpscljl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xihvybsh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bzkgetrc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bwctodtl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yjoitwtk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lewrclpc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vdaeotdi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xdlhsztx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2xwbainvg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dzcluacb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2qoqofecl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wiazwvdn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ssfohvyj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ginfqckb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rrzeczuy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2camkphtd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kvfyogub.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yyvbazak.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fcjxmafk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2csbzkagk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pctyaifq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uvyekhnh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hfnnjrad.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gfkxkzlb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2orzakyqz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fhkcngky.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2otvrkazq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2swvicqby.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2kjfnroqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xaruqntu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2zybekbny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smnvolil.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bouacnsg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2nqcmfeeq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hdxcpegc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2iajojzfg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2liqykzxa.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fgmfokxk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uwyjfjdj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2iyzfdiif.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2enusobpu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gidwflcp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zpmhoieb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2osjciijc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ltrssxrc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hfynyise.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ahoilukb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lysaidzz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2iifozmpj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2juasdbcs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2thphjqqa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2siqhkxsc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qmndnjqh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bbldixgu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2twocxcpq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bplrftxx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2tuetoyyu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2daxhpzdc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2whoscmfw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qfhrgbhh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lnwjkuwe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2jjftadvk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sebopuec.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kldeslsa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yvcfpbnb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xsjmlgvg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dqgajoya.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xogmwffx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2uxvdadjf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cjtaegum.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jyxwekru.html


<!-- 参考信息 -->