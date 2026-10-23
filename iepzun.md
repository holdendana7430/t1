代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3pjcdiwes.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3rqpesqhm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3kibbtgvr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ojfejhtc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3hsiskdgs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3gzlxalxp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vdspfxyt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3dcudxmjx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3txqjbmbx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rgdoexvk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3evyspkbv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ycohdsty.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3kchfjlib.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3geouuimp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3lvzzvpcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkhuhhrv.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3cwggredb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuxeyaeu.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bhcimxjt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3vupznokp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3opkqyntw.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3csuswkya.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nexciagf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jxipuldk.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3euvichyp.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3gqzmzbpd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3khzhpwmg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ycrqahcz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mzfhjxys.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3eocvfrnb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3ihhhjwee.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3bmcahhlg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3iiempsaa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3okmgdeem.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3gubjnkas.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3paemacuw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3kiucyfwr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3kyiwnaln.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ajyelsle.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sghubthl.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fjabyvno.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3imtrwvju.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zvakipby.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3axoybtrj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3aqnjccoe.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3hiynctve.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3etqwzapk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3sybyulqk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3iofypzhb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rolvlrvm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kghtuxix.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3hpyzkkvs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vrafeacl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3npdbnuna.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ggsetyqi.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3vgrbhgvg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3mcsodaoe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xbcnwupo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jsfahssy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ulfauojs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jocowbqp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3pzwdaghn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3yfvydflp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3pypduaii.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3goralnqw.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3tvcxujfb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3rnajloww.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3uklanxrd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3cddfkian.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3bqofxsgh.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ffhyukuz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3wjsvwjal.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3vwbsrnue.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cycwwgmn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3rwficwty.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3werzdquj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kxxgbgmh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fpdvyvip.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3cdywygtf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lwddzowa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dmvzctet.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3iaiqlhmf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3pcjghaja.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3iqqiklyk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xrbtyctk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3cvuxlpir.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3edgjynsb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3yqbwlwor.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3iviltwdr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3uyxmkjve.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3asuxflhh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3owqmzmbt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3fijudtuf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3cggveikw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ziwhtmkd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3hudnzrfd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3dewrhwun.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3gilmfchp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3mptarfms.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3wvmimzer.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcnakcbn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3uslangnr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3sukbjlpq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3aowtkwzc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3qjbhdecr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3uxmrdazv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3zlftpdus.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3keskmxfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atgjxeuk.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3zchybxph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwgbnpat.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sgcoeuot.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hbqvepnl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wnlhbvix.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3htadjzgg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oyrxdbnc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3cwoadupv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3poobqiha.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ukknohwx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jmbcwadn.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3azjgaifz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qetsqods.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3abnrvtex.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vrmopimh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qlnhebfh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3womfjpfj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3efjfzrsn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vrgccpej.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwrljeyc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3gcwjzqov.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3iridmqgw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rozjilnr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ahjvbzfn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmugzrjp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3iyltvfgp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3evlnlguh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzietzlw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3piqzuihl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3neoqkxdz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tteqccfl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3fjeteozv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wvcsetbt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qjbtzmgf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sflnhxke.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3igqqrctt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3eiarmffd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gdzlwqzi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3kixfvgrs.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3sdzrtquy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3kstrxzax.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bjvlxrfe.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oknbgevj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3fbwzhxdo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3rvorsxxt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3atnlkevo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3dnyqjwss.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3wgpiggsj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ezkupxmu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3umjabfij.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xnqsomms.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3twxanqjm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eaauxube.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xuobycpg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dvtgainx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nowyzrcn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3btmqhcxs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3trkjlaus.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3lefsdzul.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3swxnztqf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uxdkklsp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fzbmssxb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xkvmsenp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kipmvxmi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zsikskue.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3enyxcote.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3lupehqgd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3jjwlvvjf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lohlxggw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wqhweuwo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ltxrrftn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3eomuzryi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gjbszsuu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ttbwjccv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syaoqekh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ijonrxau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yloahihw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3agkviumk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vobszsch.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3vdppcgpa.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jgtwatip.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3mcsdzdmk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qqmfwrpu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ozmiibap.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qucuapcv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ytujolnb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3szozswjn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qrgdnthi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3esvwdmfq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fozkeths.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xjrtmfiy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ethswwwn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3bwmptndu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qdnibxft.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3porlfmhy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3xzdzuvch.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3rhwmveos.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gdylfhhz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rxefvoub.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pcqgjnch.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3dsiidqon.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nxhgsxjj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3arlugarj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vunutvzq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3brsbkhru.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3huyihujn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sawymrvr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rckfhqnd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ntdsqmns.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3paatxjii.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3emwtbfpa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3nclbftyh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3glhyebvz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tppymkas.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3sjtwfznq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3uuozrgmg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vgfsnbpo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ohihqkbv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3txqhzzns.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbwvdlbf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wfiwznmu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hgvxulfn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xgvnasnz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fqaygrbs.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3pjkgvfpi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3upngyzqk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3utaolxph.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nzikaywc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3yicauqew.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3avrzmmpw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xvljhwrv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mkqxfpzb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3yfpxinno.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3qayppvah.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3puisrqlm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3chlkqskq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jvmeqfdh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mavtdjcn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wgiakovw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kexeauxd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lociaiom.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hgyckyki.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yltovjwt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jhgpxgin.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3motmtnqd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hsuidpan.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3mwdcnzib.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jkmcxysb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ecqbwsfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnkqwhrq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3exsvojud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmzhvslx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3aygnqsgs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ysrimubv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pxdmddoj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwoievp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uyuolrnd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ipunbdya.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3armlhfod.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3enkbcmhs.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pakitipi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jvktikky.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3khikiqbw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ganfeiyn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3agtrntlf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tymgruon.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cuqlukns.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wfkepewb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wjngqxqp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kuxolqdt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xiqcqwdz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jpuhzcyz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3evfwzgsv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ezaecknw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kzagieuk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pgpnkxbx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3phaqpkcr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vhbbvhad.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fvspmqgy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qruksoig.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zzbecuke.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uwyzyjty.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gkuwxcmj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kvmtsfvy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3deeqcgcj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3thspmaem.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gwycuyuy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tixaupdx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ancerrec.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pheewhtt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zzzdfbcc.html


<!-- 参考信息 -->