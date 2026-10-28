代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtltwsisnq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenlongwang.top/gtbhpkvuso.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.52xcode.cn/gtndrvixua.html

Ruby: s.scan(/\d+/)
来源：http://hz.quarkkingdee.top/gtaowplsfl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtlxhgxljh.html

[I03] 提取捕获分组
来源：http://hz.jqgfzy.top/gtpinwesli.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gtinlesybq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.0kj1m.cn/gtvnlkjwmw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.andypj.xyz/gtgbkohlmz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fzhhl.top/gtfrzudlni.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shuidangran.top/gtgwrwwqtr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.9152youxi.cn/gtvmuwrinr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.smart0.xyz/gttsgttiun.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydzc1.top/gtbnsufzyr.html

[I04] 正则替换
来源：http://hz.hammf.cn/gtwwprzhtb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yueranfly.top/gtwlbfrsex.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zycfv.cn/gtnleqnrgq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tianlin.xyz/gtnwwpulek.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtjzylisuh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.52xcode.cn/gtmmviugdo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuanzx.com/gtqykjtukt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sysykeji.top/gtkhvhvpop.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ywan-chungtsiang.top/gtxyzxnlti.html

[I05] 按正则拆分
来源：http://hz.smart0.xyz/gtxdbmxqwc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tian-w.cn/gtbjhrpczw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxuanxn.top/gtantbewvc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtmdgeondl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtnfoslvmr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yonumen.top/gtsjzkuzma.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dashuyun.cn/gtvgldxszm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtkwneqnij.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangtech.top/gtfrfyagqv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuetiantiany.cn/gtdqkejdrt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtsylmatbe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangshuangyany.cn/gtgnihrlay.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtuiblsguv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtaslnmyuk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sxryk.cn/gtkujmjffo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigfzy.top/gtbbneypxq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gtvrksejmw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gtfhhvvqjr.html

[I07] 忽略大小写与多行模式
来源：http://hz.zycfv.cn/gtmalyqfov.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhaomingkeji.xyz/gtaqofpplg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258888.top/gtortyjvmh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhongyouzk.top/gturfrliqw.html

TS:   /error/gim
来源：http://hz.jqgfzy.top/gtkraitnbh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jqgfzy.top/gtxrbmzsxo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ivvv.top/gtnidigwsb.html

Ruby: s.scan(/error/i)
来源：http://hz.ehwqpu.com/gtgorsjzkq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ehwqpu.com/gtuvxgcvts.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.iojbl.cn/gtbqdlmzgs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuetiantiany.cn/gtgiqoxads.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgufenzy.top/gtdbydntfz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtdkmbiqec.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtebbxaxjw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtymhbctdm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xylfe.cn/gtrxooxkxh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.pycfn.com/gtnaruowjt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gtgwwjbfwc.html

================================================================================
来源：http://hz.jlsjyb.cn/gtyqrnkgni.html

J. 日期与时间
来源：http://hz.iojbl.cn/gtfobeybnd.html

================================================================================
来源：http://hz.hammf.cn/gtncglguco.html

[J01] 获取当前时间
来源：http://hz.cdnleiting.top/gtrvgjkhmz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guowangkeji.top/gtslrztfke.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtraxmufwb.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtibeuexcm.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtwryspjio.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yanxiufei.cn/gtsrkgdrnt.html

Go:   time.Now()
来源：http://hz.ywan-chungtsiang.top/gtlcjinspg.html

Ruby: Time.now
来源：http://hz.jinqigfzy.top/gtycuwakoy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gzhubu.top/gtveonseho.html

[J02] 格式化输出
来源：http://hz.quarkkingdee.top/gteogdpill.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtrrlqhdsh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gtbizbdtza.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuanzhike.top/gtzpnbwari.html

TS:   d.toISOString()
来源：http://hz.chenlongwang.top/gturhklpuk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tanke756.top/gtxyurfzsh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gttajgfiwj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtbqhcbfey.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ydjk.org.cn/gtjlmamfyt.html

[J03] 字符串解析为日期
来源：http://hz.feifeiyinyue.top/gtkljisxgw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guannengcc.top/gtwooribot.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258888.top/gtaupmtowt.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtnvdkvkhc.html

TS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtsjziewhe.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtiqwvrjvu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhijiandao.cn/gtysdqswah.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtyrqqvygb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigfzy.top/gtjmzgzglw.html

[J04] 时间戳与日期互转
来源：http://hz.pycfn.com/gtzobsnoah.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xingfuxueyuan.xyz/gtmmkciskx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinqigfzy.top/gtdezbgxlk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xinyue.icu/gtqfzjicrb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigufen.top/gtadlhcvaa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guannengcc.top/gtpljxtdqi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jlsjyb.cn/gtrubwoqzs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtzrjredca.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnxiangtu.top/gtmsvcsgyk.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhongyouzk.top/gtbomleooz.html

Py:   now + timedelta(days=7)
来源：http://hz.tianlin.xyz/gtkebcmtfa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daxiang520.top/gtzxvushgo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gttkzuqurd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yonumen.top/gtqxdjldti.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yongpay.top/gtcidrqpnv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhongyouzk.top/gtnhogyxou.html

Ruby: Time.now + 7 * 86400
来源：http://hz.redwolf501.top/gttezyjsuv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtlrcrlzul.html

[J06] 计算两时间之差
来源：http://hz.hfpthk.cn/gtffhvifkf.html

Py:   (end - start).total_seconds()
来源：http://hz.xuanzx.com/gtpyzzembq.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhengqikj.top/gtpjkamify.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtppfofqsj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gaohongyu789.top/gtwygcbkgx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258888.top/gtbhiggrlw.html

Go:   end.Sub(start).Hours()
来源：http://hz.birdmap.top/gtvyumrsbn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnqzz.top/gtzruecwsa.html

C#:   (end - start).TotalSeconds
来源：http://hz.ppjwa.cn/gtyfmbwphi.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangtech.top/gtslpbched.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtamyotstf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pengpengdd.cyou/gtdzhrmaii.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtiohmkzqh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtuddsxiex.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tanke756.top/gtyhnbxxci.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.mhx1999.top/gtjsabawcq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtijefxgpx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtrnbthfcu.html

[J08] 提取年月日与星期
来源：http://hz.wangdashe.top/gtligogawz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gzhubu.top/gtqsqgbsxp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.mhx1999.top/gtiwbqfegg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenzaomai.com/gtiqxafluw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ivvv.top/gtfrwasdlo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ywan-chungtsiang.top/gtjicuokzy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtztkzozfa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigfzy.top/gtmlkwuwdx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinghuilouyu.cn/gtoxyrckzv.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtchdmqkhj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.smart0.xyz/gtnppxutmo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhixingplan.top/gtxoxweicd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtdjrkdfph.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtumcuczpg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.kuanghao11.cn/gtxxxbjcoj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhaomingkeji.xyz/gtenffchwg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jyoumei.cn/gtluqjxhse.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nwbrower.top/gtqzcjdzdi.html

[J10] 取今天 / 本月第一天
来源：http://hz.zdqjudy.top/gtzyhhmrsw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gteddvtwri.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gtotiypgir.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shzxlz.cn/gtxiuyhclq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtttbmlwss.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gttxtjtast.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj202588.top/gtghythqwm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ppjwa.cn/gtxggntozp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cashguo.top/gtpicbbjvh.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtqpxjfohr.html

K. JSON 与序列化
来源：http://hz.shanyushiyangkeji.top/gtrkazesdx.html

================================================================================
来源：http://hz.hnxiangtu.top/gtstxwywpe.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnxiangtu.top/gtwyhtwjza.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tanke756.top/gtacvlrfxq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sufxvd.cn/gtclrbosrx.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtqrykrfhb.html

TS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtlsfotscb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aibaodan.cn/gtcyfjcixy.html

Go:   json.Marshal(obj)
来源：http://hz.yonumen.top/gtkpigfktw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhongyouzk.top/gtqlqwueyj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jianghu66.top/gtpyetiflm.html

[K02] JSON 字符串转对象
来源：http://hz.yongpay.top/gtednopdva.html

Py:   json.loads(s)
来源：http://hz.wangshuangyany.cn/gtjuopwmjt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jianghu66.top/gttphuxted.html

JS:   JSON.parse(s)
来源：http://hz.yj20258.top/gtqllufrtq.html

TS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtnztaefek.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigfzy.top/gtelzyxezv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtvpjdwpok.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gtbemfhxkb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yanxiufei.cn/gtkbeyhkug.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gtweyizgzh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtzgrbfdrp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtucfdynut.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtrzanqert.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtatkxfcgq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtvfahwitt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gtppnyecjx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yongpay.top/gtxborqtwz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daria6918.cn/gtswdwtjus.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtgqraskvm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ppjwa.cn/gtrhohqqtj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigufen.top/gtqclxehqg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtcwmewtgi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtygefdgza.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhongyouzk.top/gtuoqapssn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtafboaped.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtflqrpdom.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.kuanghao11.cn/gtjvcgcwlh.html

[K05] 深拷贝对象
来源：http://hz.jinqigufen.top/gthniuhuzp.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gtfudayxwy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yvedp.cn/gtxnsjrtmk.html

JS:   structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gthiapadug.html

TS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtvzuiaqhe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.smart0.xyz/gtyefujqgs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gtqarexpch.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gthskugrro.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.birdmap.top/gtftawbzwj.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gtctjgttnz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sxryk.cn/gtwcmpkmez.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.havefunace.top/gtlafbhbdd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtdqlymcgw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gtojexthzc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daxiang520.top/gtpxrlpctf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtrecimtwb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shzxlz.cn/gttvwkihgh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.andypj.xyz/gtnxzawdrx.html

[K07] 进制转换
来源：http://hz.aibaodan.cn/gtyttaimdy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtvwocilmz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.9152youxi.cn/gthchvakml.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtsntzyzmn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yongpay.top/gtibsqayup.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtcvlbnmpz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenlongwang.top/gtudlgjdpg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgufenzy.top/gtzbvppedq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gtkmonqoey.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gzhubu.top/gtjwilgock.html

Py:   pickle.dumps(obj)
来源：http://hz.zhaomingkeji.xyz/gtrjvvytmp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuanzhike.top/gtyhdvkcwj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtiftratza.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtfrcdlsjj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtohrvrxkh.html

Go:   encoding/gob
来源：http://hz.sweek.top/gtydvztmcv.html

Ruby: Marshal.dump(obj)
来源：http://hz.hammf.cn/gtrutsrudj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtaveynjzj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtyfauhshc.html

L. 网络请求
来源：http://hz.cdnleiting.top/gtijlwfvuy.html

================================================================================
来源：http://hz.tian-w.cn/gtlyqkrxtq.html

[L01] 发送 GET 请求
来源：http://hz.sweek.top/gtsuaweoiv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gtqljqojrv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenzaomai.com/gtmerjnmno.html

JS:   await fetch(url)
来源：http://hz.snrcjt.cn/gtmokoujzy.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gthxnwwokb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.0kj1m.cn/gtvhvxtcwx.html

Go:   resp, err := http.Get(url)
来源：http://hz.gzhubu.top/gthglcvhij.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sysykeji.top/gtyxsdecvb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.vqdsnc.cn/gtfhdjaqhl.html

[L02] 发送 POST JSON
来源：http://hz.daxiang520.top/gtxvihkvhw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangshuangyany.cn/gtgbzjvaio.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gteztwzgpx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtsycfbhda.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtatecywgn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yongpay.top/gtckdmeijf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fengsongda.top/gtbbquqbvc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.smart0.xyz/gtwwfamrji.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.aizwys.cn/gtodldfpjd.html

[L03] 设置自定义请求头
来源：http://hz.snrcjt.cn/gtgkdhdhhm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.havefunace.top/gttzdyxkrd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nanxinkj.top/gtewwtzlaf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtudlqeolp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtmduhlrxg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtjmdeynwg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sxryk.cn/gtangxchlo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinghuilouyu.cn/gtkoqcdarh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.aibaodan.cn/gtpuuriuxg.html

[L04] 设置超时
来源：http://hz.ivvv.top/gtjwsydcpd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangdashe.top/gtdygrlgmv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xylfe.cn/gtimzzdvor.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtihafqxyh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gaohongyu789.top/gthjllgcnf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gtracaaemj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydjk.org.cn/gtpthpjwhz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.iojbl.cn/gtqwsnlllo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhijiandao.cn/gtjtlsweyw.html

[L05] 上传文件（multipart）
来源：http://hz.jianghu66.top/gtizqvccif.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtkpzazdvd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.c1oappe.top/gthkrjkppu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtaykqytky.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gttafqbvgl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtwygdjhkw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigufen.top/gtenzokndu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinyuanbaomall.cn/gtlrosdxxk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258888.top/gtkqfznctv.html

[L06] 解析响应为 JSON
来源：http://hz.feifeiyinyue.top/gtkfkrhtyu.html

Py:   resp.json()
来源：http://hz.c1oappe.top/gthsoqajqj.html

PHP:  json_decode($body, true);
来源：http://hz.yangfankeji.com/gtzwujbmbd.html

JS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtaejokaue.html

TS:   await resp.json()
来源：http://hz.bjfxy.top/gtjvamqtga.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gzhubu.top/gtevbifncl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigfzy.top/gtwlslcwbp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tianlin.xyz/gtvaqrpdew.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cheryme.top/gtkhyiijcl.html

[L07] 处理 HTTP 状态码
来源：http://hz.jiagoushi.top/gtwnumzkmd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tanke756.top/gttuulvlrj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhongyouzk.top/gtpfvjpsft.html

JS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtvslchexn.html

TS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtpzqkudwy.html

Java: resp.statusCode()
来源：http://hz.cheryme.top/gtbsiebrxt.html

Go:   resp.StatusCode
来源：http://hz.aibaodan.cn/gtspnxfnwe.html

Ruby: resp.code.to_i
来源：http://hz.bjfxy.top/gtfasfrkbr.html

C#:   (int)resp.StatusCode
来源：http://hz.cqqwz.cn/gtoccdskof.html

[L08] 并发请求多个地址
来源：http://hz.wangshuangyany.cn/gthpmcyffq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtdlopnbjn.html

PHP:  curl_multi_init() 系列
来源：http://hz.xziqi.cn/gtoufphkmc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtxqfshpfx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtbmyfzrqj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gotoacloud.top/gtejfekzes.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yvedp.cn/gtngisoeqa.html


<!-- 参考信息 -->