代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3wqcgipvp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xryofcbt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3oktltkep.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3lglbcytq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rdkolbon.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3pwlakdkk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3dfmcihzs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3pjrkmbvt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3kcnjkbgt.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3wccuknsu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3petzjcpg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3dlkrbphi.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3cekboznt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3jcjlvzpf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3zaurghau.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jixjdxzd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3soxmsjux.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gmvzriwq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdxtzdt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3athnwxbj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3hoynnsxf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3uxjrcilg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3cvctvptr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlhzpjla.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3hkbtbzgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drmzhtwb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3mwwdfnzi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3pxoosmbs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3uidaaiit.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rcurqaiy.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ntewbizr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wvhcgzwy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3zhsitggo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3qmpadwyl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3xreuisnn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lxcaywzz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3sfvwzwkb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tqgjmyba.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3cxnphncc.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3cbvpzgwq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3tgoqwyvi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3eopetoop.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yxdujfcr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3nwcrysrs.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3wmuznlmt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3xufvuwap.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jgotuito.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3csyrwltj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3znifebsc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ihumjexy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xieijvbw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lhyozusx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3tvcykljc.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3axypmxnh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3elmcupbn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3rktbpzil.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3flaealuc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3vqbgyljb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dansocma.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ckafihbw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3oyqdmaoe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qoquszfo.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3qbzefuby.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3odpnzfbf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3dmsazcif.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bsqjvmbl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3otnhrpxc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rcziiecq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sbiyvlvb.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3xfcjsley.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qfvmjoso.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3sfpqcffy.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zxjqnsvx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ixaejvsw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3vutlwkoh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3cwmdnpfn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3luatggyd.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ymzltcgu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3oebdafcv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3dmaejygh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3xzjfygol.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wqtusljq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3anenrwyd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3alxjccdb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3sdzkwkqq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3sdrglmvm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ortdjscg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3eidljxqe.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jsussvhl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ntgxlxdq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3nqqsnmtr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3dibhfkho.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3igikcgsf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3srpwnene.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3zvdxpcxl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3spqfckpd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3kkfusocc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rnjvevqq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3lmsdcokb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3gmnoyyix.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3snamfwfh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3netsiksg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3cltghjxh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3mdijjljz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3jrndozhl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3cqlqjudf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3apkzyhsb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zccymeut.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3rnjfzobz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3mgvphfic.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qrduinyf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lxxuqwew.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3fiplltgk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3xipgmcap.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3iholycfg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzhzsaoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xidmqwgt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3bdejydpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qodlvxjh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3fpjctkes.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ffxbkzzu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3sjrknsqu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3twndeqns.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3alqtuilf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3kqebifwe.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iggnbrso.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3fidezeid.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fwsnewiu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3qkssrbhw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3qhunbhfi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3jbmpysqb.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ilnovghu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vfsmdixd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fwqoumih.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ecdybmha.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rsuiewpo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwkcbfuv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3umfjcfcs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3dyetuvfk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3auqcizcx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ceshpmbd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nfompqic.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3sijtinms.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ycjnaxgf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pvoakuas.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rbxvsjiy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdgktktf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3atnqjgbb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3txywqemp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3oeludols.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gzpqhrgd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3husgdlhr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3viyruhag.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kdwdhykq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jvfkwpgi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3xrwusxtl.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3jkakybxk.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3erdwkbsz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nppldguf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hznuziis.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3whdmjxpx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3iuehjbyr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ogaqinbf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3bkgvzfse.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3rbleixcn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qzjikpfr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3inhimcki.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jllbqfjs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3broralmk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3soehltfr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3harosmjw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zisiznog.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3azrkyzzp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3xuvpbzkf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kcqdvnbi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ohfdjhpj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3detkkdqv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rebvvoqj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3swrmncdv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3yyfvnkyh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3utkxnodj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3irljgfpq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hxeeqken.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3exobwobj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3nhjrnmgh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jtukxonw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3eyrdokwq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3hkzezrgj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ednavooi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3peykkdbe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vmbegpwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kybxzwvg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xyahhvil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjgeobln.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3orckesjp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3swkdvmpe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wpoyrdjc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfxkvpu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uuqughrd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lyriddqk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dqvegrvg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3lntxqknq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3okrpwwet.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nxtsnrib.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3plltefve.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3gdfolkig.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wbazvlzn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uyvgmdwv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wjlyyuah.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3dbpsyzfp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fpymxbor.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dsrzapxz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3yesmpmgh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3qsgkdkrc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3prcxlwft.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hjazfnwz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gdjgbupm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3cbajueto.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tqlusqib.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ilduhqlg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dyjxosqf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bqheqptp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbllpdf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vgxuxgda.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pvmraspk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xveobjwg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nlcjuqxn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ftrcvqua.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gyhintip.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pxfxqvhj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3mriiavqm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tzpolqxu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zggoxuyq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3aqazqoah.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ldjaynfs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xtjfotap.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3bddyrykx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jqvugqfg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qaxyzkqc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ytrsbxzv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ohfzciup.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3qbonpjck.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ukogiwup.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vixebmep.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qkfnysog.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wzbqfnvd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yrkjcfqe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3trkoqlil.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hpfraetz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zfzdolsl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3fvpghsud.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3aztzqaui.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3prsajlhi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wefcymfa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jinvxjze.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qctzgaej.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kindblhg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3szzfilcx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yntofxuv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ueoweqkr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rkeqngpv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yhvqntzt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gflktspy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3fnsuanhg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bwafwqtg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3joeqonst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lucqhiik.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3htgavifx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmucpknh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3moptecbk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nyafzrpk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jguvwuol.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ueravbgi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqmlnujw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3twxwgbpa.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pemgwgvd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tlcfslrx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jaqbyhwy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mdjexbas.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cdomyvmq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ujvsxmbx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mykavxpo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wdnxiyrr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jcokvmtz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kzyygfgf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3okwtjmce.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fmamlkch.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ojvgohgz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wlvyifze.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nfoptrya.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hbartpwp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rwvudkro.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3quwertye.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3iqsvwyiw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cpjtpwqz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ekizqgep.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hypobusf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gfydhjdd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vrawsvhp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xyklilrs.html


<!-- 参考信息 -->