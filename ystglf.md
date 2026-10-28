代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.52xcode.cn/gtwzfbgisr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtlinnvgnl.html

[I04] 正则替换
来源：http://hz.gaohongyu789.top/gtwnljmagt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhixingplan.top/gtufqdjmlq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgfzy.top/gttmmfvsbg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtbagmdxri.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtmgsvqsgw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sweek.top/gtjbzlccmn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jiagoushi.top/gthlksuelj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtrmsszcbb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tian-w.cn/gtmavnkqxn.html

[I05] 按正则拆分
来源：http://hz.zdqjudy.top/gtfjhduksb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sysykeji.top/gtwwjnmxsn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dianchejie.cn/gtflwkbfyz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtxhmvqhat.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtzwcfzinv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gtqevsuyab.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtzfnwjyeu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtenihgkby.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cdnleiting.top/gtxeejthby.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhiwuduotai.top/gtrdwlfosg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtbtlyoxaz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtgfivdxfb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtbgrtkbax.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.birdmap.top/gtkzhhbhyp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nwbrower.top/gttquhbupt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gogol.net.cn/gtxnxolkrn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gtpiimcqnk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtupjsphdi.html

[I07] 忽略大小写与多行模式
来源：http://hz.xziqi.cn/gtsndlepfr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.316326.xyz/gtzgrdrvax.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.meibo888.top/gtdsjgnize.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pycfn.com/gtxkcmbmcx.html

TS:   /error/gim
来源：http://hz.snrcjt.cn/gtazzgeesl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jqgufenzy.top/gttbdhsupc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ehwqpu.com/gttijhvojt.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtivxpgtuo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gtupxfzpaf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.daria6918.cn/gtyyhkhwpz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.iojbl.cn/gthboevfgi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gtniiulsbr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtvdevrjql.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtmzjtflbj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.0kj1m.cn/gtxydfablu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.birdmap.top/gtxfxvzwia.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtkvecuvlo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xylfe.cn/gthrkyntpo.html

================================================================================
来源：http://hz.jianghu66.top/gtvccmcryp.html

J. 日期与时间
来源：http://hz.yj202588.top/gtyombaddp.html

================================================================================
来源：http://hz.9152youxi.cn/gtrgxhtcfd.html

[J01] 获取当前时间
来源：http://hz.jinyuanbaomall.cn/gtflruexek.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhijiandao.cn/gtczxxorew.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtfnatuodp.html

JS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gtflrzaxhs.html

TS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtqkwtoeaz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.feifeiyinyue.top/gtnryuzmbr.html

Go:   time.Now()
来源：http://hz.ydzc1.top/gtlhwwntbm.html

Ruby: Time.now
来源：http://hz.dashuyun.cn/gtrmwpushc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hfpthk.cn/gtsmjevgnz.html

[J02] 格式化输出
来源：http://hz.hongshengwenyu.top/gtjtummqfc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtamvsejjp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtttgxnmup.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gtzmsqnbov.html

TS:   d.toISOString()
来源：http://hz.yueranfly.top/gtohaespxu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hammf.cn/gtnxaehgqy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtcdvqitrt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtyihxbfuw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hysaishi.cn/gtxdptffuu.html

[J03] 字符串解析为日期
来源：http://hz.jqgufenzy.top/gttivciuuw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinghuilouyu.cn/gtbgfckcoe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.quarkkingdee.top/gtwzgdkwvi.html

JS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gtweacblou.html

TS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtjyfzssqj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hammf.cn/gtrhsktfqk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtliemfnio.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtskwyoadf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gtqgvrtxps.html

[J04] 时间戳与日期互转
来源：http://hz.dianchejie.cn/gtqanuxsxg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtlpwcnnwg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgfzy.top/gteyhmijpc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jianghu66.top/gtvxzerqlg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydzc1.top/gtreacmsyc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtbkcreban.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cqqwz.cn/gtjotdtoam.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtjzonviyn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shzxlz.cn/gtpcmwykmy.html

[J05] 时间加减（加 7 天）
来源：http://hz.haohaochexian.top/gtsnmbgtfi.html

Py:   now + timedelta(days=7)
来源：http://hz.cashguo.top/gtejcijawb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cheryme.top/gtryukqygh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtwofcsldo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtsteisacb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenzaomai.com/gtcymwhimj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hammf.cn/gtivsjjlnv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yangfankeji.com/gtgbcvwhky.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sxryk.cn/gtczzjhebs.html

[J06] 计算两时间之差
来源：http://hz.c1oappe.top/gtwpxzzfam.html

Py:   (end - start).total_seconds()
来源：http://hz.pengpengdd.cyou/gthznkedvw.html

PHP:  $end->diff($start)->days;
来源：http://hz.jianghu66.top/gtifnbbsuj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtnfwverty.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gtinhpqnfx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhixingplan.top/gtnihmigla.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgfzy.top/gtvzfvztrj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtxsiyjvtt.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenjidiqi.icu/gtdeyjotsp.html

[J07] 比较两个日期
来源：http://hz.c1oappe.top/gtkeqsrzjm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtkjtpshiw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenjidiqi.icu/gtydghunrx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtqgughyns.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gtblqgubed.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hfpthk.cn/gtnysgqgyo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangtech.top/gtnjtexyef.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gthgmrtued.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtwonssppz.html

[J08] 提取年月日与星期
来源：http://hz.hnxiangtu.top/gtgspnzxcm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jqgufenzy.top/gtnuiqgsan.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhiwuduotai.top/gtwxaxyifl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zycfv.cn/gticuqmxbo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daxiang520.top/gtincubfjb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangkeji.top/gtxxeyyaui.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cdnleiting.top/gterfpsoze.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cqqwz.cn/gtzoetlczc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuanzx.com/gtgsbndsfq.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gtrgogeqsk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.316326.xyz/gtsijyqapl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.haohaochexian.top/gtnjkwdivk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtwekdbgul.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtklqktwlt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangdashe.top/gtyhemkyfl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtobjoarjw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gtdckwkfvg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gtfulonjzf.html

[J10] 取今天 / 本月第一天
来源：http://hz.zycfv.cn/gtkvbenvgy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gotoacloud.top/gtyotlslhj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xziqi.cn/gtntfomrnq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gotoacloud.top/gtzqbqofba.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtygfkgnla.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gtqltdeilp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sysykeji.top/gtsksfiofw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.snrcjt.cn/gtohweisgt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jianghu66.top/gtwyomspwr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtcugiqedf.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtzqvvyaxb.html

================================================================================
来源：http://hz.nwbrower.top/gtnkjprlxs.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258888.top/gtkbllnjhe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtugeqxmnm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtbbtihxlf.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtlqqmxugq.html

TS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtbnxznrxp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenlongwang.top/gtxqvunuil.html

Go:   json.Marshal(obj)
来源：http://hz.smart0.xyz/gtjzsnhjko.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gttedsvcck.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xingfuxueyuan.xyz/gtdgblmvpr.html

[K02] JSON 字符串转对象
来源：http://hz.tian-w.cn/gtpkbapzdu.html

Py:   json.loads(s)
来源：http://hz.sysykeji.top/gttsrbcmwg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhixingplan.top/gtbyofmqdv.html

JS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtsaryzmsa.html

TS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtezghexoq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fengsongda.top/gtmbucsuxv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gtnvobqwyl.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gtgkuwmpbt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangdashe.top/gthbuwmvjz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hywenlv.cn/gtzovcsjco.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtswvfcgfa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtvwvakztx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gthrhzdhvc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtghnwjpqz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cucudq.cn/gtqoemeriv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.quarkkingdee.top/gtztdbrnwx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gtzpvgoepw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fengsongda.top/gtehrayvpz.html

[K04] 读取 JSON 文件
来源：http://hz.yj202588.top/gtfpmgzuks.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtxvkkxrqk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gotoacloud.top/gtmlsteppk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gtxzyiqwtp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pycfn.com/gtdajcmjik.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258888.top/gtqzzjjxdw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtnmabsfum.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinghuilouyu.cn/gtnixxseam.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangkeji.top/gtuguzsdrv.html

[K05] 深拷贝对象
来源：http://hz.yj202588.top/gtsjziiapq.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtqbvyiqfv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cashguo.top/gtywtikvep.html

JS:   structuredClone(obj)
来源：http://hz.redwolf501.top/gtrhnrdrjb.html

TS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtponjxdoh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtxsvfcbut.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtqhehoams.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtqoiusktl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cashguo.top/gtduubmzcl.html

[K06] 解析 URL 查询串
来源：http://hz.sxryk.cn/gtpeasmzaz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dianchejie.cn/gtbomvlbwv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtgkvmhsfl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtmmibbdyj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gtrfsnrxoa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.feifeiyinyue.top/gtjmaaggsc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigufen.top/gtiyigvdzx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtnghbjdpi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guowangkeji.top/gtelldmdrn.html

[K07] 进制转换
来源：http://hz.tianlin.xyz/gtbzclmfnp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtfthpxtam.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangshuangyany.cn/gtadqnyytd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtvofneklk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gthqevfnuo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cheryme.top/gtdfqnbeys.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtxnzxhsxe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.mhx1999.top/gtahmwwklp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.haohaochexian.top/gtobotvfrs.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenzaomai.com/gtoxlvdclv.html

Py:   pickle.dumps(obj)
来源：http://hz.iojbl.cn/gtvmzolfgw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.mhx1999.top/gtmxmkifbh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sufxvd.cn/gttzbnceeu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gtjzlezrwb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.snrcjt.cn/gtelfhtanx.html

Go:   encoding/gob
来源：http://hz.guowangkeji.top/gtlavsjdrf.html

Ruby: Marshal.dump(obj)
来源：http://hz.zdqjudy.top/gtrztadepe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtrcgvzhjn.html

================================================================================
来源：http://hz.havefunace.top/gtcyjjwchu.html

L. 网络请求
来源：http://hz.gzhubu.top/gtzuugdzir.html

================================================================================
来源：http://hz.gotoacloud.top/gtpqrksdmn.html

[L01] 发送 GET 请求
来源：http://hz.quarkkingdee.top/gttizhoyro.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gogol.net.cn/gtzrhmpkje.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtyljmfnnr.html

JS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtzuwnjdbo.html

TS:   await fetch(url)
来源：http://hz.aizwys.cn/gtpktgispm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pengpengdd.cyou/gtdofrkrym.html

Go:   resp, err := http.Get(url)
来源：http://hz.iojbl.cn/gtloovgqav.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aibaodan.cn/gtaaznncel.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.birdmap.top/gtizvsozjh.html

[L02] 发送 POST JSON
来源：http://hz.jqgfzy.top/gtgreqyfrg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gtasdvxhcq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tian-w.cn/gtjtwofugh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gtpjogritl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtvwncvkpc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hysaishi.cn/gtkfcpqqri.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhongyouzk.top/gticxseacu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangdashe.top/gtyosjehoz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jianghu66.top/gtdthqprxn.html

[L03] 设置自定义请求头
来源：http://hz.smart0.xyz/gtxsqpdlkj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.quarkkingdee.top/gtjnwbjpql.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenlongwang.top/gtksvznwla.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cashguo.top/gtxpparobq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtlvlhlyam.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.wangdashe.top/gtvtygwspg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtidnijpze.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pycfn.com/gtiimirmtp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xylfe.cn/gtorebinrt.html

[L04] 设置超时
来源：http://hz.pengpengdd.cyou/gtfniqoibq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtqbjetppv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yangfankeji.com/gteyjytnhl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtrkudvuwq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtocnpuzoo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydzc1.top/gttvdqpkqr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hongshengwenyu.top/gteiitsnoc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hfpthk.cn/gtavdtjwta.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhaomingkeji.xyz/gtcipzrddh.html

[L05] 上传文件（multipart）
来源：http://hz.xinyue.icu/gtpvafrsbb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nwbrower.top/gtlgbtelbt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhiwuduotai.top/gtcunhfvud.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtsaobinzf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtwvmjvpcc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.haohaochexian.top/gtpxixyfqy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guowangkeji.top/gtkgxkuite.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cucudq.cn/gtclgrvqvt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ywan-chungtsiang.top/gtauenwvtt.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtrwocieya.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gtigygndeq.html

PHP:  json_decode($body, true);
来源：http://hz.sweek.top/gtlptvddou.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtikcsrqvl.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtgmbswnjo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtmptdzmqp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jqgfzy.top/gtoxmdrzsu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shuidangran.top/gtgcxyjryl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gtcofhwbmz.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj202588.top/gtcwmjrmkk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtedowmbjs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jyoumei.cn/gtjjwzrtha.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtaubegdgw.html

TS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtswndilgl.html

Java: resp.statusCode()
来源：http://hz.jinqigufen.top/gticrcnqyn.html

Go:   resp.StatusCode
来源：http://hz.gaohongyu789.top/gtkmntllfu.html

Ruby: resp.code.to_i
来源：http://hz.sufxvd.cn/gtadqynctr.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtcgrysgiw.html

[L08] 并发请求多个地址
来源：http://hz.jyoumei.cn/gtyknfnexi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nwbrower.top/gtimzdszhw.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangtech.top/gtpegacore.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtkwcgpumq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtkuxvtprr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sufxvd.cn/gtibacswya.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuxming.cn/gtbqymimpx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj202588.top/gthugsxvwf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.smart0.xyz/gthswaidhi.html

================================================================================
来源：http://hz.wangdashe.top/gtakrzsaix.html

M. 命令行 / 进程 / 环境
来源：http://hz.meibo888.top/gtiagbpmjq.html

================================================================================
来源：http://hz.chenlongwang.top/gtwljsrpgz.html

[M01] 读取命令行参数
来源：http://hz.ppjwa.cn/gtjnctddrd.html

Py:   sys.argv[1:]
来源：http://hz.nanxuanxn.top/gtvpczypzo.html

PHP:  $argv;  $argc;
来源：http://hz.zhoulong.xyz/gtrtlswtfw.html

JS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtymxbibco.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtahgfyoxa.html

Java: args 数组（main 方法参数）
来源：http://hz.birdmap.top/gtrcgxsorf.html

Go:   os.Args[1:]
来源：http://hz.hongshengwenyu.top/gthabvbkyt.html


<!-- 参考信息 -->