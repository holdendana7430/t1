代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3kqscadyk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zhxglxzh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3oytoeobu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3amrdkqfy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ovyoqccx.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3qfifmqsq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3cigbvwwt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3aoadbtzo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3awbxifat.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3gxliiwob.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3mylelxqb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3rfzopkhf.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3mekgfojd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ypmdfdyz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3bpkotrky.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3trtaqhhu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3fdhhvcwb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ptkzomjg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ypwlsbcj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3kwduvijf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3giyhuqdt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3tmoyrqiz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3cjtuxejp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svpxajfe.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3cqylinsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txmzzomx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jkltvnoe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3beurpsjz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nxxthivw.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3isttxejg.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mqxhgjeg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qlojzlhv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3jbcsyjmj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3oqutsxuj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3cdcvxbha.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pfdervgx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3hehnjysb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qeknflkb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3wulcdodz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3rykowvta.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3kwoelkom.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3divdyelw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3obpllsgw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3lkvubcnw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3qybdkljw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3tznmfpiv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3wpipprpj.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3iioswisu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qmuouecl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wrgotbru.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nctbcpvx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qxcxzkmf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3vormptgo.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3dtwsoymj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3eouwjgjd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3wjvcsgwj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ydtjgafs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3knlikzmq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gvjxslxu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dopiaxbo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bmsdyhke.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rexuxzdu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3cqqoguey.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3hejruooa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3jxmpecii.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3chtpevwx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gqnzmhif.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jwgrhouv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bjmkqqth.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3sdhrdldi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nwsvomuj.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ykvweopx.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3yoponidp.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3iezoyhfc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3hxslcuel.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xpuwqmnc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mokhsnux.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3lvxjcanv.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3wddnvpyg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3otlovssb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3cvooxpmt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qxtybtwc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3tcsgonmp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ftseervc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3junoblst.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnlrqrge.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfebmmuf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fbiynyhi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wrlcnkgt.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3xofnrvvy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3elrhktlo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3goqfclit.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3lrjkykek.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3kdlgkwnp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3zcrotwpr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3apkxngbz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3rnbhloaz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3hjhrrbjy.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3lbcztfnu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3hnfbjflc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3oivutyjv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3dgivdmog.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3klapgxgk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3bphpkxfp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3lpcckxtq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ohrpcrxv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ndnxcpjs.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3pfryxbwt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3stzxjfbq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3utbgptsd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgdbwuev.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nezrryju.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gszugibf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3jycrjfux.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3vjxomaup.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxhdqdvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tirrhmxm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vgiyajwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfvnbtjs.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kujrjlhx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3kpvjnnsq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bahofzln.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ldtqudrc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xozowvhm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ekuzwrsl.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3tcmpszvj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3wisjhxop.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3epldtkyw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yhwrsaij.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytkzitpy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3vjvkdvyf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dyyvmwxw.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqbokkkg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yuebircr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ucgguzxy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3muckhpsb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcinijft.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3nkhpxqgj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bqawhsps.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3sgimsysx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3glndpymr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hhzddsmt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3nmrqchfk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3anhqxpcx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3fbkqjeqh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ujsjrsqw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3dnyhdtra.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ssipbrfz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3pfuklyqw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fwhzgock.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3urigzfbx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kqchiymv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3smwbcpop.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qkcsdfpi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hewfrphg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3uuqdeqpy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3flqrvzxy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3maklvndo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mrhpskag.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jqefolhh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3qffevnys.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zjppvjqp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fharobrb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3hesxwgci.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3odxueope.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zwniaixe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3dznnztam.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rclgpinu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nkcpidpy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3scbwxzsh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zqsncsyz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zbktzxdc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wbhkoysx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3pxvzyezf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ujawsocc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3jqjgjgbx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ojypwlwq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mpmkiehd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3byliazww.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ogjvfemi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nebqrzcl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dkdmgupf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3swgbfhii.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3olmuxlcr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kclwpyrr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rcxojane.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wocwbksv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qjrtmgoa.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3vbreqogc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3lwqvhihx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3espckphk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iychewtk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3undmclwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ultuekst.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3frtwfnvs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3savvmbjk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tzirxqjl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wlnnloac.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rxugmayj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3omsbacwr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3solsrzdo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3jbmquobs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mpkreult.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gtijkgxx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3fjjnvgmx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3wauuylsk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3edaymnxi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3olopewix.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wwbrnycd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3djoncfpy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qjzvcobk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bvgedhhs.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3axeshete.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3lnmjuosh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3kvcfdciy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yyyzhysw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qlodmtfz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vxxrbewd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lixqfhmq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tencaibt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3aqbbgjfk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ubbecqpv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qqekbhhj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zzhtlwpi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rihhoiae.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xmpyvbtc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zhubkpmw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jnldwvtc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gxlwaelh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fvekwwow.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zvcpcgrd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wxqgdzuz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kmuuzyxw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lxzmiene.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aimchxne.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hibazjzh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3lzrnhbun.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bacieeuy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ycxdaiyf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3buhcioxi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jnbppcik.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oyoeubzy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bpjwngob.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cwdtalbz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3haczuznj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3pshdozkr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3omgiurew.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3vcwwtdha.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wicqhgmj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wjlxwlik.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3csvuxcbi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sbgytcmn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hxcxyskm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zaeejqdv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lmmuijpj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nbhptaub.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3txvxqhya.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tkfdbuva.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3zzyywlxf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yifxvpmd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ldzxbart.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fveauqzf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dtzcvhil.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3zufzcujo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3skibmhpc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kshytlsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytuodqcg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tgurdlxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsqiqdkr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eqhvfzad.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ieypctyv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nryelozv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wrgfnqnm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxrezfzl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qoqtpadu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xptpmuww.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ejdajvha.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fdhzfuwj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3thobtkya.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fzjpslqo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gsfdmcgt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rbiatrlp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cqtkmjch.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uehtnydc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3deuwxjcr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zuvkndru.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hrybskbd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3babmblnw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3leoakora.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hjamdijd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rkkqoexf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3faxsjbus.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3loblhqdo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ghnsnpcm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ysxydrny.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wvhmwqmv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ojefsydm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oqujspkt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3emejuphq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gjcartoo.html


<!-- 参考信息 -->