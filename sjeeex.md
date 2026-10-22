代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2vbxeuots.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2tncpuupl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2lepltbfr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ydnukgrf.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2vnrsrzyr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2srstsxdw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gmgsvhgj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2bxiyyjmg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ofebspqw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mnwxjntt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mwmagkkf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ofsnshxi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yjdjdhof.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2taeuarsr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zqsclaei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fubroldf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2slgtlcsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suxsncfu.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tgmjqovm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2gbyelnuk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pqnzprda.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pqlkgrtr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jgbqtjwp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2yzqibpzb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2drppaqhg.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2poxiozfa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2njyihalk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jkdhyrll.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ykrkdomy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gcqxvjuv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2fuvvewfw.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2nybkkkgn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2vhhsqjfr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ifnogzqw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2gxifbdvy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2xhbkfzvp.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2lotnzuii.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2osekejlr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2rykwqcco.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2isszvlry.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2evwhpjeo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iuokvpas.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2omamnvui.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rcnujsed.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ikodjtuq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2bdshjcci.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2pyrbsyvb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ajmbzxzb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2cbbknjem.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2uedrqbie.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2kovpkaut.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hkhxszbg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2esodoqed.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2oromczlb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2bztsoujm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwamvmn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2rhvwmpmg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2tmtfmhii.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ggczmxov.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fdhmdkpn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jvpdyktw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2cipddrdu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gtfbjadd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2awmqtwkm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2plhqxvug.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2wylqkstu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2eqfuldsk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2meqllbzz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ymqpmnpr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2klfmlndy.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2luhisfdg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2dcyhrtpa.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2cjooymly.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lxmlukqf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2qaaylhsl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2spqpanry.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mrnkpboo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2amzlqppy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqmpncam.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kqjsgscg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2oxtcczxb.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2wirwsfls.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ynylpwhe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2dzwjehjk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2kkdcibja.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2jtxlxfxv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2fpwqmpeg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ffakbewi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2bvhglbdv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2vpwvaaai.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ualubbiv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2gzhwdgon.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2slprnnzi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ppswghhe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pssmnqdd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2wturmbmw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2lzwinwuc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2idhlexzi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qlvfbwns.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2iiwwjvgw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2yryszane.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2pudkerls.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2znwxdwul.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hokrpadp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmfkyvj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2owjsfrnk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2cdbwhyue.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2fmdjqwiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iabrftze.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ttfkkmcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkjsbvic.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fmoanthp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2htuexlxy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ikxlsuda.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bwertkle.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dotubonq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2sbxwgckf.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vsyddseb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2pofwxpay.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rymgtgqs.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2udrhqgqi.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykkjhjuv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2koortcmf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yqokolrt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aeulxyot.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tlwsvcnc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ihcnwydy.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tkiemwux.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2sjkofbxz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2fezsiazu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2dastxkxd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lnrgftpj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fximtvec.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yeuhabiu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2xckmlmof.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2fikqhhyl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yzyixzxh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2joyxcref.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2nptljfmx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2nenrvocb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2umeilrwx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qkwgiqaj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2kxbikilm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dywhtpbz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wvadiocw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xcfxsqcb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2khbfyici.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2sduiexnl.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2zopcgoos.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ngiflvxr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wuerqhpz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vdbfwacr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2iulguexg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2rfgdwwek.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zhcinixr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ehbnfnhk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ynvsvefu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mrsixbim.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2jbalkxiv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2csvljnix.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ogrydlpa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2werqmsjz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2punifpir.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hemmkata.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mlfwpsfw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2lephwsnb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vwpymreu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2kucvdlxl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ovvbklud.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ltacqdcu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hutggyrx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ciklmzjw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tmowynwk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bevqqwjv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2rjuaxdrm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2afgjbkjh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qngmmpbo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ftgygdck.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bbvxxewd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2zjqnffrb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2npmobjig.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xwaxwrci.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xouymbqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpdumeas.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vmhnghym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fydgqzlr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2trcoqroy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2asitbcxb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2eyuiitah.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qfupgfca.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cdvbmczx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ofzyzfgq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sublfedo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ayfwrvmz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pwnutzrp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2loljvvbs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mrnqhshz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jcoegodd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tybvslds.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kbezmefq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qjfocpes.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dslqmnbz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2wpmzcdqq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fgxmdwku.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2tqzoubee.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qedlifie.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2rayoldyp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2riruawhl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2iyqckmym.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jnhavhxi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kdlekply.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2koclgbkj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ywommbhi.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2cbuvvafe.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2unzyhzzu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jwtewevw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sqkpvedz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cmilxtgm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tvkioqla.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zwgpcgll.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mtdzcgie.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2flungebi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2mxpmmhfj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fevkfkly.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2siarnflx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2odasoill.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mxmyyipu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vgtunfgk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlhaekcl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2oleooplk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwgovlue.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qcgxkkbq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fkolfjbd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2olfjnbxn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bevorxrm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mjqajniz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xhvlntxf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2wqtdviyz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zphrzojg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tpszmkhh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qjoudjwa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ypyyriwn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ffnecrmg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zdleldoe.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2oianzefs.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2hxbhddlf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jaddzolk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vjtgajbz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wssokkjw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2duzrqrus.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vuhcxvqf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2xjutzhld.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wzkeienm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mjdoebrl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wygsiaih.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2prcvdchg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dcibpluq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ukdblgsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lltowktr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gzrionwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvumnxbw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bhknzlcc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ojclwjxj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2uzwoysdg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hqbzpekq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xqpmtjal.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nuifohyb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2txkurwmn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ykmvldca.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ydcagvkg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jouhljph.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kesnzcuz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2myynxgzp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jmydvsbg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2roxpksuv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hnxgmpeg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bnkayuav.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2nidyzljk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jsihsqng.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fbjppnin.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2uljwnwmo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2dvnkwgsu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wgezqqjv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2whmelyhf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kopqiume.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ttiseqfi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dadknycc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ituhfmmj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dvuyxjjy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2snecjtnk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2eazxufvo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hhxjoodj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2czmlrclq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uvzyqeuq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eoofxjro.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mdfvgqvm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2nxzflnqc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2thajtitt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xevtesaf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ewnpcjjf.html


<!-- 参考信息 -->