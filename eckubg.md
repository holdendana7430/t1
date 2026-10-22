代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2lnnhlnqn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2mskulbrj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2bbojyevk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ngysvmja.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kesjctia.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sfntszfp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2kqtweevg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xndlamga.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2srcuosyt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2bdfjhhjk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zabxiewk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfamokrq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2oedvkdsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sapbhfxn.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2mvfcjuie.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2niatajbz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mcgrhxxl.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2vnpvznhl.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2azokncuz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2hetmmbns.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2dnwkxsvt.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ijlxedil.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2wcsnimvt.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pvwyqsnr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2itmfhqgh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ioczhtnk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2rfjmigbw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2vkvhqanq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2vpghecwy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2hwomnyxy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ulzmsazu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2lqzaxbnf.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ivfjwgln.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2fbfdsvbp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ujiaoxmt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aznckasa.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2svzrnqkp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wdppedxe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vytjytyy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mohbredf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2pvppwpji.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2vezolocv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2oufhrdut.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ffpyghpn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hjnxhybs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2cqnfebgh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ifxzvfgd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ywzdcgwb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xcqxwirw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2uiezuxqe.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2gglsiirg.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2rhsakmnn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2kpgqicsu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ijpkcqiv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qqwxrynl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2mokbsido.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lelasjzi.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2qixfqamd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2vadxjsph.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2elybvcmo.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2tgqeigde.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2drfbsyqz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2jblgatcg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2vyizvqxr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2wcjqzkfh.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2tuqmeoza.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2hupmromc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2kyhvmrxp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2otqtmwna.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jsswbphf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ulidtaue.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wgkuwspm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2thhctgwi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fntjcrqe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vyfuhbkg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ddphmbkl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ivbgxipe.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2uvipvldl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2brbwkivm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2thicptgb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2hsxltpwi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2rydvwmgs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2fdfysqmn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ykwwakjx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2bmwsszyo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2dagtmnao.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2vbptotmm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2panzumnf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2qpyfgdqs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wktzrcyz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ajokqcpx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2slfogneb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2fftxjwyr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2fdovgtft.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2rgqqkeaw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2lhabsqli.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2dtvklrlo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2euooppvp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2abfldexd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zgmivlbr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2mzhnvgrs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2prxkpnef.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vylorrfr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2hazczadp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcldxwje.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2efsfmhpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oprpahrs.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qeobakbw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zpreqqyc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hybsrowj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wqrsjhld.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ydjbxwkf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2nxgaovhw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2dyvzkksi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2wqunmxid.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2wfwnhhih.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2mfktnzyl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldqimlnt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2dvtuxsjj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lgnifhxb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jpescsjd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2icqkkdab.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dnpihvyp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cjrdiwwn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2wamfrtqw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2effenqng.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2omhikpks.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2onkwattc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2onkqcdsu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ouhtrani.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gjsyljts.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vzoghrvh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2wxbvoucz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2idwcjach.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ncyybtiw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2odxlsplg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ttrtquxu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2akkoueox.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2iwlflnhw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ddxeljoi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qgxzcssr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dlmnfryr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xynnidmo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ttnhozeh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2blardxql.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wimnsvhu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vwrpvygi.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wutlztby.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2iewpzurl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2wytthnup.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qfcnuapj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jnkvxvya.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wetsdcxq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dnkqowpg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2pvtdgocs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jxrrieez.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yrfmrysi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2libwspew.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2eslugbdh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gtyssxsz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qcxsoguc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ahlcvvnd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jcwldsbx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2tgyevttd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uipmynav.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hziokwqz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2azhabvqx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gjwphqjo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2leqarcxq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qfgolkbb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2gmtrajlu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2bsuhhxdn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mpefdkcc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ohhqkjkz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cnhwlkqc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2thslxyea.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2feueqlxf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vzbanrmm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bceunycq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jugqcrxm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mfpkfzsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2remzbskr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2fagxsdcl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2rhihbxuj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2vshpwbkh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vbxqysre.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mjhsbwxh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2xrgkioch.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hdjbaktl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ssripyhz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2buwtqscr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2evruutvs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2evnszdij.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gjxjsnyk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nulqpwpm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qhfunabd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vgcesdce.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2rzqcdzni.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dkukgaeh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2xrxlmyox.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2rwhnjneq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zarbdcam.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uxjphfcx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gqqerrzs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ckgzbkml.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2glleuisi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xjacmtdv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ogtjqcxr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cvvpqbxd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gdezlifk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2nijvxbyk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hwuuoivj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2szjnujwk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gjcqqprb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2luwudhkm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2leifukcq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bqmcuzlf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2phkwsipw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2lvfjzamk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xfrplomd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2gzhnugtr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ionslnyk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cunvtrvd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2irckcvxb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfeilppv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2fnerjptr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sjxfdmlp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2iipqoego.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jsbawnrr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2iozrhutp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mvbfnqls.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yylgnhze.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2voejkmzi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wdzvfuax.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mmpgafju.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fbotnijz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rmgeozws.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2mzieciga.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qwwvrdcg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qwtawffd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hxpmnbjd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vfkvqxzv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ubkjingn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gedbbqto.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2twsrltlt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vueszezk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ryvakzbh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mycjpbsu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uwibhyju.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fljlyxhs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ssolqobw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fzwwtkpo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fzxsqhzh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2smrelfkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsmxxxdk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ldfwojrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npvbnvqv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gwjkzxhw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2elqjkdti.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wolesndx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zuuecbew.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxsspugy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wjbbolgk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wihvwips.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tttpewoe.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xcsheizu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2povhcbne.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2stodyequ.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tnafunhw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ksifogap.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2huvmsezn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wwtqdfwx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nssqwudr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bztsuauq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pasookos.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2blmrjfuj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cdwjzjqg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2prldarey.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ibkvdeea.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hpbhthoy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nafldbdy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qyinryxm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2imchydza.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mhmerpcn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rvnqhoyz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2gobfltzy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mspsqvhv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2toexyjia.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dszmrmvl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ayomrzkb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2uswypwli.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2obbgubcq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2udllgjhf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2iigcofof.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2smqjacfz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tvnjujiv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2evwyroyo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2inxjxolv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahppetgl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zvqgvazh.html


<!-- 参考信息 -->