代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ueeecvwm.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3jnepdldx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3oysrattc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3egerapjl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3segkjskk.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3qhemyccn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3afqkhwzw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ifsyjhqo.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3nigaqszn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3xntwcumx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3qbaxcdig.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3fuufzzwj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bcxwcfxc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3flolljcy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3prrpixlr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3bdlqqias.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3pctwrnsc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3mpihxjfd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3vmlieyjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3teugftpc.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3uqlsdrrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkxzwbwi.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ydcpfnti.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3tjfbynxt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3mnpheneq.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rflenosh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uokipypt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3vnticzkg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3leelwoer.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3nixrwumt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3wvaujxgn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cizkxzys.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zgbsdebd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vijxsviy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3szfinqef.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3smpgazjj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ypiwuvzp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3flqgrggm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ihhjgjrw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3kcitqzaa.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3vorczwnx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3bkqmpuki.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3yagfzhwo.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ptcwsbiv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kamyitqo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ahtlkkks.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dyyavape.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zjwvnjrv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3hlsysdhc.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3fragdcvh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3enhwhshd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3dixskola.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lqpqfzik.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3mhzkupdj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vczlticl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3dswptkhq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3usrnxorz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ektcaaoo.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3slexmjez.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3wvnpxssf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3rjbrctmn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3waylltyp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xhcbilva.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qrmmogzc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3iduskter.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3pewqdjge.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3bvturofi.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3tshrtaap.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3evmqqdxu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3aeqrieqj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ejayitmv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3azgsgrbi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3saasgwdl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3uwwmqpam.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3rwopphuu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3tgeeiobw.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3mudvosci.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ixvnnkkn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3amcbppgi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3laycpcjs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3nxkcszww.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3oihwgieq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtrlmfnx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3odhcwune.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vamfjcou.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3curttaaj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3tcztgxuz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3wccsdxmq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ldlcutzi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ssbpyslk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3srfniqas.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ccwojktu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3mchqfxqu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mmiuqprg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3pboojipc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3wavokmel.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3cvefdagb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bxkzfxkj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3fuxiewxq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3bbdjzjvd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3femmqbkm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3nmxfhtsp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3kuzjznwp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3wxxoudlx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ogmetdgn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3jedfuskg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3evsdzwiq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tjrrtfpv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpnfxnqd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3biscyndr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3fbqjvjhz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3slxgtwwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkwgodys.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3hivjbjgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgqzsmhx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cclhuugd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3tmvlspml.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zwbovhzh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bzsoqqmy.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wytoslgb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3gosgndpl.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ockttodz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3bbfxurfs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3cefdafmx.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3zgkwqtnh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3qiaxycqg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3rzkiosbv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evmlqrjv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vzdwxckw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rmsmxxaf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3etrotspq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qclxbzej.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfpvdtbj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ktjfxkez.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3njcpofij.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wyzfybwr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jxrsqrwa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rlghjhxz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3dvfdczio.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qlpdxots.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3shluatfd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xgyzeerw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozyfxnsk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3qgiuqdoo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3shwsysod.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3lxxdlbaj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ymrpmful.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pbyrcfga.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nzdhmwrm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tkcxvcgg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ldjprwos.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3tquuddak.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3torydumo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3abszzdyw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tyhrzavr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tjjqmmql.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ajuzyhih.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3fronowky.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3hjrzpcss.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3oywsylwp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xxcxpztr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gocahweq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3scvkuzmn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hmuzclvj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3buraoreo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xookygig.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ofvwztff.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xbepjbez.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ynuwwhiu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3azivusnc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dgqimdpt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3rihwffvb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lbfrwvuo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tsqfwgcg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wfitgsxq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3gkitstda.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3sahjyvrt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tsulnuoc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3shvgxoif.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tlreaxpt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubeizeat.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3edlbuckt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iqqzgmrd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3yhjfyerc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wqrlsajj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uytaupru.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zoglpnwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jckaxaad.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3hxqmzxpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpqxzafq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3wzgzleiy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3dsepfjhc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3kkhfraxc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hjolamut.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xjmxkdqa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3uweumjuu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3itlvufdv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dftctilb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xyfgmrvn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3yfglxton.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mkiktvhx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3dyssiohp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pknithkq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fvnyftmj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hwbqefwz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3pbcmyami.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3nzoyetfw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3msgphckz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3esotfapb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3kqwsbfhz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3imyeupla.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ektcgfmm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xcjckjsy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3kxmjamez.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wgoniihi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3vvubmlrs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gwdaooxg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3whhpeeig.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ipyskrww.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3nybgasnu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3efqkwtzx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gdmssvyd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uspqujic.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3sqpbltnn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xequqtxn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3byvhrnor.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3oubvhbdo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fjjrsreu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3glzsuros.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vgemnsbk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wunfdsni.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3calrnlok.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gpmpyxwa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mlbdycvm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gxxakaxl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tmwyeylf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ggymnwuq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lrfmzgel.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uthtunro.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qrgqxrxo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hvsnrryc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lwwpvvmm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3vwajkeyv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3pwsyxysi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3obyylpzy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ajxegonl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nzurlird.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nvaehuvw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lijlglgc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tyfnlxpc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jiyjkzzf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vuoiirrh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pxegamct.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ewhbvdvq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kmnjrqmf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wgvynmrt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ihfqnncl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nkvmmwxk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3znqnhlfx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3jztcdyed.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3orurwrns.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ifdtahcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcomfgry.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3fohewfax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsdueugg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xqfdupsz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ertzgqvy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mihzrcar.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oijguwpe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gxujpqco.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jejvqmiq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3orzsmnoa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3stxfyuqm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nkogcfig.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xvjevpqi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3khafngah.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jiduriok.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3djxyzxfx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wrpwayxb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nhfqwoke.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bqiuiutq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fwfyydlo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mbzamgdz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3tkdkrank.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rrxuachr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3dksawksc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3djpbxwyc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3phamhznm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ofhqwdbc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gcbdbkbj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cmuuvdoe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ytochuxo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3lhmzthml.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yoklusme.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ckxbihqu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fttsxvdx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dnosugww.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mcrrxvyb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3denyczcq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pqbyspvp.html


<!-- 参考信息 -->