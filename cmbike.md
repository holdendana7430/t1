代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2gihinaxl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2rjmdxspg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aziktsmr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2evqylcen.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2rgpqwtja.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmfzrby.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zjlrwhzk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2iyjqkony.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2kvdrgppf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2tgxhvruc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2atazaoim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyttkvbr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2cefquqtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgvlieck.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2juhbgkcf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2dmpmqmnu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zeryygqm.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zjziwmop.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wwmikvqu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2jpmhvbsq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2oevxkphh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2donejabt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2bfeliztj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vyorkrih.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2sfcapeuj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2wmblcpid.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2kgajcuyo.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2vqywdrvo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2mcdnltxq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2bkznorso.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2enomdeal.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2hsfuwgbu.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2fmakmlps.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2hcuaoiah.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2jxlchcgl.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vulgrosz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pygvmreq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gxiyaxxu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lgbvhyvp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gxyyajun.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2cdcbfukl.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2vadleghb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2msogkivo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2xsbqqegi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2xdzrkpin.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2chcsihnx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rznhvuts.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2umljsqvx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2kwnaknfw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2raslkpqu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2etxylfyf.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2uwpcjxaj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2zgaopicq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fipwvkzn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ilvfjxum.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2eccscxlp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ecjtuwmn.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ylnbdqwn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rkwflylq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2fmfbmggz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2bdajshfv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2zsloojrz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2lymotrcl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2vjxybecr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ubmrhqow.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2dmqhvlnc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2tdmlqimd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2kutixdrw.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2pclklbyv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jayiuart.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2bbyonhmc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2gtvusjtp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wqmywftd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2drdoynbp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vlhqroqn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lseveujw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2reymtvse.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2zvxgwrnc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2wsyzigzr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2rdznnvdy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2jxznujij.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2hyrbebmj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2smjmvnkx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2smdpgnue.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2rycgazkg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2xcrvlslg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2jobejzag.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lpqitlih.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2wpzbifaq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gepwwyvw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kkihzqjx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2vzondlfp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2xqsskjcw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2eddfrwus.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2eozcvkmf.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2vssmdbek.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2iodppxdc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2bwztvfro.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2njmswirn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2impztigg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqqkgcfv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2hdizaios.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2dunrqffa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mnuioodw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iftsshyy.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2pipkbioa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agfnexbc.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2zufkbthl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2kuygdjnp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wzcwoawo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dlzdkfsv.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cvkmdhan.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2pliepdrg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2muqfosjm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2wqulbspm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ilmscmbw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2mibejxtg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2aklwsvop.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2apdvidsv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gjdunpav.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gotlcifz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2oorrhgwh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ufkmbyos.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgnfbptq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2sgwegjte.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2vwdnrmwu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2negvdgxo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tbaoqwqr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ojtfgenq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfasukbt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlorzgj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2atrsdcpk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2vkpiisyg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2wjxqafof.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2sjoqhpzz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2hszylvie.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2etzjdvos.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gmbvnfzu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cowvjdyn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2skvqdylu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2johkuopi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zwqlkvzp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2muhquqha.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2gaovsewv.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ddzeuhbh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2sshbdrgt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dgnpuwyd.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ockcbxka.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2iauxrxnv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2vqdzexls.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tqamrqea.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2tyymhnav.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qcgmgfub.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2uhprrbqb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vixhxhhc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ectjnjvq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fecedwlb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2wgrctzlj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mzoylbgd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ojtyrhva.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vfypqntw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2sbgbjnyv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2piipueax.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2atctpwxe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xzqglori.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rmlrtvui.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cxrckiey.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ngvrgowp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jmgcogpc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xuzejmlf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zyahugcg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fyydgxtz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmzidbxg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2whnknhrv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2alywvsnh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2zuqzhnpk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2msuycgur.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lvgsbkwz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2obwrikvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzwhefad.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ujiizqef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qizawogz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vixxbzhm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2iyqvaszq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2fvsomzwo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2obydcfbw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rshcahab.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2nzrsrelx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2iwxeqnyu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hdljsamn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ajuxuark.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rqhcauon.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jgjohltr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hiuiyrxe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xqsutswl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gsylslab.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2witezljs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hskfbcvt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2nukgiusb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qafkclis.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2nkloqqic.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jgdurrmg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dwzljpvd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yaudgyip.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rjnmwhrb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bigmtple.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2npzzxapj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2dcicnrxm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2frgxuhpb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2suqalgtq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dsldbnhs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ewvdhmux.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dzutyjap.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2skhkbqpj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yadmkrzn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2mjtyowig.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vkgiigis.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2sjrymflc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gkuisdmc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fysdsuab.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2iocsylea.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mhzdigqb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2geqnnusy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pgrtrcfv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rbonsrro.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gbiufniz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ifzcntlz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2sdogcyew.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tzassuri.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zrrelprf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2acudsytw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mrrafaoe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kbjtouhc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rkkxbvqk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cnfwhgvx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2rdhxkjfh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ukbajkzx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ihalrnuc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2towltzre.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2deuwivuq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2adktffgf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ueinlwfn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ynjmpjbq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2coxwfavt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fpwmvfmz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lwjwtqvp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2lsiqxxzk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kctuupza.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yoqtfsec.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2titwgqoa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2urxhnreq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2qfypfouo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uktayjdb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dlrshuwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcbrowcg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xzqugluk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2escjgife.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2papkfamv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yskpbezd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ujvyosjt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ejwfviqv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mofjnghw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2legmrbkx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ilvvbjny.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2oepmkuqq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vqhcqkzi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gokvukhy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lmswohov.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vojcmyjs.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dhhwlphp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lyjqbqmh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2twquirgu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sylzdteq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ogmwmapq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xfqksieb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ospcfkgb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vlafwvrp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ymisqccc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2msblcwzj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2amwmjmmz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ylrecepp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mxoainbp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2smomoive.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2whkvpqsb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cxzlchnt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nqkrjtnz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fbrmtvuk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ugnlkbmz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2upyuzaio.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ubnqeinu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zcfxwgrg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xmeliuui.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2vzcbzujm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2adxknbdv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2thsugifb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bblioozd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2euvuhxet.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xxpsxdrs.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2phyfwgic.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rzjzyfff.html


<!-- 参考信息 -->