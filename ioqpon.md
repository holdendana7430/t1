代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wydebyuw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3eixzfggd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3adpszxeq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3qxxxdjny.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hnlosduh.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3fxaeizlt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3icsimdzo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ijsqmadu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3upxgjyvt.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3sgwctzeq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3vdwpnbyw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3oarocbnl.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3afldudyc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3pqalpebx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yqgxsaxu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3kxucygit.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3uiptzkyy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dzqzgjij.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3uzuansup.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ryonowfh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3gonockrp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3lmzkxhah.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zycmrtft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezwudpvh.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3asmepxfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgjvgkps.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tulzderl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3iupoqhdv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3zyrrbocx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3voxbysvw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3puxtzcgu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3npkwhwde.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3fqrszwmn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3mpbrplcc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3wymsrdpl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3eisrpzrw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3lmoskbzg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3cdvaxkyn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3iwwxanqm.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3gwzqmyqc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3spwluofa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ddghgoos.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3cbjqvrzd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fnycoauq.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ipzcqykz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3izbelsqi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ppsdsaqw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nrefqrpz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3plhimvoj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yupewzqm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xqmonyal.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3raqdwwfg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3qibgjjth.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3zqcyjbkz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3assyysor.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3dgbasgjh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3xxfcgpqf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3uoailejl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3tvaxdsse.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3wezzqnvl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yhtpfdrx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3imjysrvw.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3zmggmkwu.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3nwhmeyrh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3gwupjzrj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ztsgbciw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hqupzrdb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ryginqlc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3rpdvbquf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ahftlkyd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fjrlumje.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3vxsmonuw.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3xyfyledp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3cbqjogvg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3gbddqnat.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3nzzimzge.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vfxlvcqp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3nzumcrmp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3oimpswel.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3mtnnbwsd.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3uuivpziv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wnthuiof.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ugasidne.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3kptmdfgt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3svsjmkox.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3giqrjtdj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3bjpnhonf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ldlftpxa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xrnkxcuy.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3fmbqvddx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3zgyefcjo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ddzywkrb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3fzvxxdwn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3yfbkpssr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3pcdzcrxy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3iicvtiqu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3lwygsvoz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ziyljrlv.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3usvvpkbk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3dyrxrwac.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3zfxpyjkp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3cterlaxo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3dajwneum.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3rojrrwdm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3sfrzelci.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3dgpzllen.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ptjsamkm.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3hytuswqh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjfddrhm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3fpyaawmz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ilixswpr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pbhgyrtw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujoemhsl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3kgwmhbnf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3fztpezip.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ngefwbza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdtrfgbh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3abhiqgsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggtwcoyw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3gjryqiuc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3coaisomi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ocfizetd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cycrzvfv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3buotpbyl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3cdtcwbhk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3sqoxygpp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3rhqtfeyc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3mhoahrmz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3wyziqsjb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fighgpnb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3yzwfvwrt.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdccswkc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qoigxfew.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3efbntdjb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ckhvstql.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yicimeqg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bpwggsti.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3rjuhcrum.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ouvrteoj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3kzaatneo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vtdkivso.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wsavvgqh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3milkrltp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3bllnneal.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3xyackguh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3qwgwdjwx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3dohdgimo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3onhxubzj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ssscpdui.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vgsmjpkm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hxatugjm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3blwehspx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vxyaglzb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jcsvvuuo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pyntssfv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3zrgfwigy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3skidzfco.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3xkuaujxh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jbyafwbq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3eqmqleqv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ytfbxetg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3jbnnfotk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3dfloqpqj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3wtqngvwy.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3yvltcvjr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rxkxjnsd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3yqfdajiq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xezzeaho.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xsghimkw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zmyuvtpc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uqbboqwd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3piylsmpw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3atotvkyv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nzxeobuw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yatpqxww.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3clgyymqb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cqdydbwu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rpcmcbmg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kadhrymj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3lmthzuri.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xjfcrpde.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cthjhqzd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3vpmralfc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3buabussu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3trhqmfre.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3illhabsy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3amdfwfqz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xcqdduwl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3cshdgplv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oqewqudq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dipkuqgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejwpyooo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3wisdrubn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3propkrxm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3plsaepju.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xadrmwoq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3bicxmoqq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3focccjsg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3omyxbuqc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3uqvofpbw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hozhttus.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3lwopjszj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3iihvrrfx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nenxyrhd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gnppcxmf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3exibycsm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3yvhskpap.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dukodndg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ycmlzunp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3olaxoyjw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hnflrtaw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3dpfslbde.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3lxjiexvj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3dcsieoni.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3buzlkhke.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eumuvowd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3weljwjar.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3grihguhw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sshepsdt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3vinmxvqs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cykfqmwy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3nyqepygn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3sukrtlgk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ptbxqswh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nttluppy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nycdexin.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3sshlepdu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3eekrfakv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jpkctode.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3svvpjykq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qfydzpds.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3hswxztnb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ctlkkpyz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vezyvsmc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lvivwtrp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3oztkeisr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zlogwmpq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zkoehydm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3osvptlmk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rlynneju.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3scvtvspe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gtobafwp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bimfvnfd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pthfevil.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ijggcnrk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3cotemkff.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3btwcxvsx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3sjjeitlr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3clzwkfhu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3qtsornid.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3rqtkbuqu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3higmdwqa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ilqhkykz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dnvfvove.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rnjelwww.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3inkyloay.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ggggmxxy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3erzdarbg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rxjjyuyp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qxxgjvop.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fslttbvy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gwdohdrf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3polsiyqg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qekopitu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dgzsxcrl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3swfagudn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thippxik.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lkpwqdim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdbnylbr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ksfjnfra.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hwllfbxm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tbaegkmd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmcnxopn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3umdxolrx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wbfnfwcg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3suajfqau.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3eqalenpb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dafkesfn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iqkrqhbq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hhvrzfhs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lyjwlftb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wbiiwucb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kobtxyzz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pedrcrga.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kxubiplb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gtwucbnx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dtwuihvw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lthjuwql.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mapwocmt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3dzdirioy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qimbdgax.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ultrhyho.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3diyoawvo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3muhvjxmn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3sgpnpboy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rzmitzro.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3aykqduut.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dbfgtyho.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vhlhajor.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rknoklmz.html


<!-- 参考信息 -->