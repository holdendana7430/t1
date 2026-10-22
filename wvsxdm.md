代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ixqxvzof.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2hnmzgbmq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bgnaplne.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2inyuirfk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ccrbtljw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fnbrxeih.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gmkyncye.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2qxvatapb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2sxziswlu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2cgpafxgl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tykkdmkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjngirvy.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2bpsctail.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iiddqndw.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tvjmhxri.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2pyxrcxod.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hjhgsdcj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ketyvvzv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wlrnhkpy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cyglfqqj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2fuodfrut.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2zskhajjq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2uofeswyk.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2usivbgpm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wroddfww.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2vvdcyxil.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2bjqgvtdg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2drvhtysl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2kgmwmjpv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2xzysjxqy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qcjmyhqi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2mworrlfo.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2tnzhyxby.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ojqaqzbr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2eakwwztw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ssdzjxvz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2frpoyniy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rrhrukde.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kjgydjko.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2raxuvkot.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2vyyarkbd.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2jwfahnuz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2thvvylna.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2oehnvjrk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2aauvozud.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2pqbuioou.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2pvapxwpf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wwvhombh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2phqoywup.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2nhsmmmjh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2obybfold.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2pwivpvog.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2vbbmcaew.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2arrliagg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2xlqucnxl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ciwtnkkc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jjsmdgow.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2saqmxoca.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbagbor.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2dajxkcrb.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2bbiolpvf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ymbpljye.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2jxachcld.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2jqrijwjj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2srcnhwrp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2otlmpnkf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2pygybzzp.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2uaqeskwo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ebzioxoy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2aaxzpcan.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2luhlhoji.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2tlivybgh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vnicitwu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2jxpbwpwx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2yujecqkg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2sinzxtpv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ubufdaua.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2joftcanr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2aatzabzc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2sztrofkc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2kohwzuya.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2sksgfljz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2aefvvoju.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2welgsdzr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2alppxhpq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2xtqnuqkl.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2oraexvfz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2woavkgsa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2jkhuqycq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2soetgzdx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fupwgmlw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2vbdknfer.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2eudvuuiv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2arhijqld.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2agutstbl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2mpmunqye.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2snrmlmho.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2hzcizjsc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbecjcnn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bqnytkyc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ldpxcbqq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2zgtsyaln.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2omdaaoxs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hbvirena.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzcbimje.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2lkbhylpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzfphbxd.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2tanleprd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2kaqvcgps.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2nmnzgbet.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zjrljexc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2asacsbaj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2uetfmnho.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ztoewsvs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2vfmsalwa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gtosdjlk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2vkztapwv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rmessumf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2pshzqgmm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ukqehknm.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sgidllmm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uiatsuvh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bvumhetj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqtzmhrh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sanbgklg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2irpmqhwc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lswbhyas.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xeazqdeh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2cdvgysgf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gofdmvwp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ghjlbuon.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2amplridm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ruymsokn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2hisrlvjm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2khxfbjrm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dsjkauqh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ykslmwio.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2novpkjma.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lfepcpse.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gzzlynla.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gcifcaaw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pbiepdpi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwfkasnb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ncesqrvi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mxcfrzzp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2gypfbpyb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zvzveveo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rkfjkaul.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2tfxeagvl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2hlncxyzc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2rksdntkw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2dvcbrcsq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wndnvxzy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hqeluycn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2trmxoefy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yelplckh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2avxiwpie.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hrommrup.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2joyjyfij.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2euusdgic.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2naaexdzn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ofpiabeb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jvjtczmd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2gmpvjdhu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vguorwso.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2boxyeszv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yybtzhbk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2selbskco.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ilspcokc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2harkqtso.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2qwcucjlo.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aiaiiuyy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2fxtwxkqu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mzvujpiq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xuthyedd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2aegjfzta.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ngwqafyx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xdofatyi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dibupcer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydtqonka.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2qhhyqvgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twavtghg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2lrklquak.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2yacezfxq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2rmizohar.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qanbjecz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lyasofjj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ajqtskqe.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2igqdsqet.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lpaqdblt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eflrmxoe.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2crxnroft.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2yrnamvco.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2tkpehkaq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2teuryhao.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2twllqxqp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yoqojzgm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2cdtrpdob.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2axyvvswa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vwysmdme.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wnjthpxj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rzkfzedi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ftroabqd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ixdyzwem.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2putzulke.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2gbcegbpb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gusvpncn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tyrketyq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ucgqwphh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2scsaovqz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wjaqpcho.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wakrsrmz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fuoiqrrv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ngeupubo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2avxyngid.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ripbqjja.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vsscywhx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2udgkvoig.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2tcirksvd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tcsddaqv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2mzimkeyo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qwfsrkea.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lfygbbsn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2lnvyszxk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqvdsqlh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wkwarlqz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vsfssxnn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2eliaozsn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zmiictqh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pdgkunxj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cvggkwcl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2epnyviiu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oejgcrpg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2eaewpdtv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2nbbfnfcq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2sqqvczcq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2szcnkitn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xkcerxfm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ruzglyzz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2magfgkuq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bswmldha.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vcycpurt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fcasbwel.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wxzjwsis.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bssrdooz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fqfyciul.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dxnwncqk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2eybjfabj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hrqtxgkw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yseecjto.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2qjhttfok.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mcrxzeiq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2egdmpqiz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2khqlvpuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnppdamh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xkhwbzpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxplahxu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2teutspkz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bnrerdsi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2yvzufkvt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gbunwymk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vcnxkzru.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kxgpxtze.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2abyjsnev.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2pyhoidur.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qvgjgtwq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2eekchfgo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uxdxomto.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yftyewlk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2evfykcqr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dmdixwxd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bmlavqxo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bmqfwldm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jmycjlfg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ssajamcu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2blyeblhc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2fruljtst.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ffgmjrav.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ztoxihsf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nemqueru.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xbatzsoc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2sputqsgm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fgfeazox.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ksfwxlhx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2kpyksjeq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2esvswcrc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lviftmkx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oforydle.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xzhzcaov.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2snukxeos.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ylktkwhw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2javzclbn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gavypxyl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vfzzsmpg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2joyrybro.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2eqsnuewx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kkalnvpr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qwpluvme.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnawjgno.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ajtuamgz.html


<!-- 参考信息 -->