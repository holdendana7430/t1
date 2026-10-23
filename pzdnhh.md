代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yvxjmnur.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3oczlxuii.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3zsnfhqer.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3iojlciiu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3guwtsigh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3fabepiaf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3etoogyxr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3dtzqcdtu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3mlddmtmp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ccmxqiao.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3rumfqfaa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3crnfzmkx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3trsvpupr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3astbmfym.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fwcukour.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3annbelwo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ggoybndf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3eonhywea.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3soriucgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctyfvers.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ezbojobw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngkuzflp.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tpfdvith.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3tgyjdhry.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jymlfneu.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mzkeklfx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kxcwslsy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cehmisgv.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3oucrexaj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3vkfglkqs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ppwoiurz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ngzrzrqi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3buzvfkty.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3fcetvjrx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3qzdvuncw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3oghxbthf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3dmzhvhfm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3eonmqlpi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3axxwrmax.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3qqhovpkf.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3qnkwmztp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3qxwkczjx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ciyqnfza.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pphcxkfh.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hfcasmfg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dcydgrwb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nhezyila.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3palpmmjc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3kpxaxkfw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3avzukpzx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3xlmoerxn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3synymscl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lykxqvvq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3xamtzipd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3dtjeciil.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3vwwxldkr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3dyllozfp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3eioicirh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3tdcuhpis.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ulexntad.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3gdgxvgqn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3tmmtnwzp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ocllaiuv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ujsswakq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3ymztwspa.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3pakicwoc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ndpwvgdi.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3luegiiqt.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3yzlytjdl.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3axwoewic.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3docjcaqm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3oatnwxhm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wdcxxyba.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3nahnjugm.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3plbijden.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3reyxewvu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3vjwgbrfj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3yalmkcbs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3wskxfemz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3fmksibre.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3eztyybwd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3vbduhseu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3myndeotd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bwwoeros.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yvslwyla.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3wyqxholl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3mgctmngb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3nckyhfzo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3flqulham.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3cuxvfpmm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ubukased.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3taqdzemf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3tyjebcuh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ytpjvkhn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3yzubklxg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3igjdejrx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3wjutwnnm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3quuczgsj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3yepbpusd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qykllppi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qwhmuguk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3fmodlnwf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3hriwivot.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3jictvylx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3enrcntga.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3xaowgqev.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3fnkzwwcq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jgvaolzy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwmhgfqv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3rbiihehl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3dkmuasyy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3olwubdlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lozekwtt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3wcpwvzyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvclcyie.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3laizxqud.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gygigebj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3feauafjh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wifidqsa.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hwjypmoz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3xowhmqfe.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3akkgmlsj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3qznfgbal.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fzbgtjtp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3zcihznuk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3pwyjeofk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3hawmjqtk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckaatlfp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlvncceh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zvwynnim.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3eirnlyvk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3keoubfan.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwtrtrjr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3wqrywcnt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ikarvahi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fstottiu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cevaesae.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cicudxhj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3npapysou.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3toennmuj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3igjhdveo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3yzpoppfu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhuuyhgd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ndaootit.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3yfuamiqm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zifczbal.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3syidkcqz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pqnhdrrv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ihdimltk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vvwllsdb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3oyfjdnjh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3vbukjffz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3fwomarhk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3gfrldnra.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vzfvsbpf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ftmrukea.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3yicyyuom.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3qhxmrgen.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jgltpfmo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3csfoclkm.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3qhuuaxxk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vkuiqwfk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3djhrtici.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tuylzemy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mwhoazdy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zftgevcg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pnzvfvgq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mhchgnyn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3alzkesop.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3nnoqucha.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uefdadot.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ldwhlepn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ycavwuqs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nbwgrxuo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3knwkxhkr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ikggfcqk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mgpopbyx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ydqbdymk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3zkxrbthg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xxidklwv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngrdraas.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3smqvseab.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rbczpasy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zztdqqmm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3pnesqjey.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fxfmvrmw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ngwfiztk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afbuovrz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3hgsumrvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixhgwudb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3crfhzdix.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3rctgquep.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wuymvdfy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qvjzxfzl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yvwaudwh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3uzvfskpf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ehlalsqm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dbwyecfn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3lgjjvkdf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nlyyopum.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rwjpevle.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ftaqjlcg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bcvyldtx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lovcjpau.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3edagvakq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3iqtkyktp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3posygksj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3exewaufs.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3iwzxtrtd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3txjfwafv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zhphlubf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fifngakq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hkpruqjw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mdgrsuwi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ipytguwa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3behjckor.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qnwdfjtz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3yftlobwt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3dhdvdmtn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tqksahga.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vspvybze.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bqpanwga.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3hqwejhvp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3swmmqfwg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3heuneney.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3egjgjzpo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3himcttrm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3yocnyood.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xyjnzsnk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3oatheljb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3sventvgk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3dzvbxqew.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zdyvbbnh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3htzxtmff.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3emglojtm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jggxmscu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wdhxyzyd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ypjeewft.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qtptllhb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bxiathnu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dshlpoxh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xasjgjbz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3sbyyecsy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3idfkeiho.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3psvzefjj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qkfmazbc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3clkfmirl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ygxbutkj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dojnbxcd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3utwujpll.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zobjrdxw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kngyqedl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pmpzdmyf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lvvgnhxz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xocdanyo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3awfghspo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yerqlava.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qnpdgpgf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3imqfxuvg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wkytzpqb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cygrowrp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hckcppww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhcuvimx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3phjvdkbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umriognq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zzhfnukg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qxcxdlba.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qjymnwjh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gngmhign.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hgoabofd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kaivuctd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3twokjuyx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3yfjpzcux.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yjugqqud.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pafdebch.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ajpngjnr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cixalnrw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rberbmcl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gfodcerk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jishguvk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hluxeoer.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ezbfhqve.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ouofjinr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vvuhyzga.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aukftrgx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ynqamxbr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vuvymtrh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xabysfcf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lpghxuaa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kvjfatig.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3akgjygfx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jtrwitdz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3tlnlfclu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bectqylc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3pgjaltgu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gsxgukkh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jfhbpogq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3sjwmhngd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fxvahcnm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3uvtsesah.html


<!-- 参考信息 -->