代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.jinghuilouyu.cn/gtngqsvpnw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtsqjplauu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.c1oappe.top/gtnnyucpay.html

Ruby: s.scan(/\d+/)
来源：http://hz.zdqjudy.top/gtfepymezs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtcrmbvjvk.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gtaaxwxdzq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigufen.top/gtificllmv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hongshengwenyu.top/gtbjwknlbo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258888.top/gtflyrvoag.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtsmycvhws.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtzbzwkkkn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgufenzy.top/gtafljwdkz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guowangkeji.top/gtlnuodnrh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cheryme.top/gtqhyrpdgz.html

[I04] 正则替换
来源：http://hz.aibaodan.cn/gteurwdegg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxuanxn.top/gthyfqvjrh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gtqftwmscl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zdqjudy.top/gtrwbfwrba.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtjboznmgs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sufxvd.cn/gtsagnahoy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.bjfxy.top/gtpfvgnpce.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gogol.net.cn/gttreyibow.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sysykeji.top/gtfztxixrv.html

[I05] 按正则拆分
来源：http://hz.316326.xyz/gtvlmewoip.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtbghjrhdb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.feifeiyinyue.top/gtbsljbqtq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtuharhfqo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gthnmshrgm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tianlin.xyz/gtalbzvwfq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ybcxt.top/gtqeiwmnat.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtxswxcwqe.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtcjwwhmqq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gotoacloud.top/gtkqudkyft.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtpkntoyzp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gtgehpjaxz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtykktaxge.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtgzoygynh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xuanzx.com/gtbodxnzzn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangdashe.top/gtvthxzayq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.snrcjt.cn/gtrphgzgpn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gteoeeyqgp.html

[I07] 忽略大小写与多行模式
来源：http://hz.guannengcc.top/gtknqwqpez.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydzc1.top/gtfdfzdugf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gttmtytyja.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydjk.org.cn/gtxmnopnqu.html

TS:   /error/gim
来源：http://hz.ybcxt.top/gthkexanup.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhengqikj.top/gtwyxclgwr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gogol.net.cn/gtshjlncse.html

Ruby: s.scan(/error/i)
来源：http://hz.hfpthk.cn/gtefdgsxlg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hfpthk.cn/gteffokdhr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gtzcdmxunm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtdpwbstuv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtzplpunft.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtcgjwgovq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangdashe.top/gtslqtkfle.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtkvmbusgm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtmraitiem.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xziqi.cn/gtwhrydkrs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daria6918.cn/gtbfuhzlde.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtnleokgpo.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtjhsiukim.html

================================================================================
来源：http://hz.cdnleiting.top/gtefgpxfys.html

[J01] 获取当前时间
来源：http://hz.dashuyun.cn/gtscjjzsxo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258888.top/gtgbrfarzw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gtdfsffxzf.html

JS:   new Date();  Date.now()
来源：http://hz.zhijiandao.cn/gtufvxsytg.html

TS:   new Date();  Date.now()
来源：http://hz.52xcode.cn/gtzrmoyick.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pengpengdd.cyou/gtdrsqosid.html

Go:   time.Now()
来源：http://hz.zhijiandao.cn/gtpzrxugui.html

Ruby: Time.now
来源：http://hz.pycfn.com/gteqpzkuow.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sysykeji.top/gtxvteangf.html

[J02] 格式化输出
来源：http://hz.gaohongyu789.top/gttradoqsz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gttualxzan.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258.top/gtlgbjvpfo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.birdmap.top/gthlwulefh.html

TS:   d.toISOString()
来源：http://hz.hnqzz.top/gtcdgulmxi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daria6918.cn/gtyjzueowk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gtjnklaalq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gtpbmrnozs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtxkkntvgg.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtpfpcdppf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhijiandao.cn/gtwzykofsx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.bjfxy.top/gtsyrgttcg.html

JS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtqjdhygyq.html

TS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gtmhdtnjyb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtvrvmpbsj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.kuanghao11.cn/gtqzorblxy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gteatxppwe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xingfuxueyuan.xyz/gtdxtrdiax.html

[J04] 时间戳与日期互转
来源：http://hz.jinyuanbaomall.cn/gtheqomgev.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.mhx1999.top/gtfcbpnjww.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gzhubu.top/gtzezmrvva.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtdcpeclgf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenzaomai.com/gtuslddbqo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenlongwang.top/gtaabtxpqe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shzxlz.cn/gtywppyyil.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtvsfosnff.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.smart0.xyz/gtbyeuhdzq.html

[J05] 时间加减（加 7 天）
来源：http://hz.havefunace.top/gtviqehyxi.html

Py:   now + timedelta(days=7)
来源：http://hz.cdnleiting.top/gtyysbanew.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtopoueihm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtfbrvjjog.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtahxxwwef.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.meibo888.top/gtdysoqied.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinyuanbaomall.cn/gtcxllzafz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuanzhike.top/gtfnabgsjw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtpchmesbr.html

[J06] 计算两时间之差
来源：http://hz.bjfxy.top/gtbvrrbzzx.html

Py:   (end - start).total_seconds()
来源：http://hz.aizwys.cn/gtghigoggr.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtocxjqhut.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.andypj.xyz/gtontptlbm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtbfvaknww.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangkeji.top/gtxjljrtsu.html

Go:   end.Sub(start).Hours()
来源：http://hz.316326.xyz/gtrynyfwfi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnqzz.top/gtbybdclot.html

C#:   (end - start).TotalSeconds
来源：http://hz.hysaishi.cn/gtxlglzdyo.html

[J07] 比较两个日期
来源：http://hz.kuanghao11.cn/gtqmltfvly.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtfkhmgdav.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtwrwiyjzr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtvcovaxlf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtdrleiczv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhaomingkeji.xyz/gtykfxyrbl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtwtongtyr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtakhmnxqm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtaqzzhews.html

[J08] 提取年月日与星期
来源：http://hz.chenjidiqi.icu/gtejwxvikw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.birdmap.top/gtvoiixbob.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.meibo888.top/gtullvuxut.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jqgufenzy.top/gtwwizojsz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gogol.net.cn/gtagucamga.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yvedp.cn/gtjzzfrodb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuetiantiany.cn/gtesosihls.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.andypj.xyz/gtqwrdhhwo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtpivtuirv.html

[J09] 时区处理
来源：http://hz.ydjk.org.cn/gteipzpnmr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhaomingkeji.xyz/gtczfniour.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dianchejie.cn/gtiryxzhqi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtjjcftsjc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtokqysdol.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yuxming.cn/gtwmjtksqb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinyuanbaomall.cn/gtfgwmxiyh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.iojbl.cn/gtsrijiopa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ppjwa.cn/gttfzjkxdy.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhengqikj.top/gtlveifquf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhongyouzk.top/gtxhwtjhmf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigufen.top/gtyusmczbr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gzhubu.top/gtemkcrzzo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cashguo.top/gtupjdbwqp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.316326.xyz/gtsilxdkkp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sweek.top/gtlzmhurwz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sweek.top/gtpzgjlnqf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhijiandao.cn/gtpilvfvar.html

================================================================================
来源：http://hz.yonumen.top/gtxsiinrky.html

K. JSON 与序列化
来源：http://hz.haohaochexian.top/gtnfcsymsg.html

================================================================================
来源：http://hz.yonumen.top/gtlxqlfmaz.html

[K01] 对象转 JSON 字符串
来源：http://hz.cashguo.top/gtwwbaipac.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtxqvpvwcx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtteobiwex.html

JS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtbkvobkck.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gttzlvtxfw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuanzx.com/gtfchuhnsq.html

Go:   json.Marshal(obj)
来源：http://hz.jqgfzy.top/gtzikhyxjk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gtobhmjhdf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuanzx.com/gtbkzsqxli.html

[K02] JSON 字符串转对象
来源：http://hz.zhixingplan.top/gtxtizvyqr.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gtmphtazur.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgfzy.top/gtdjzavext.html

JS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtwtfjxoso.html

TS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtgfegjnwj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuetiantiany.cn/gtauduviiw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtcejkqsfg.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtrteezsct.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sysykeji.top/gtausnyzll.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtxrritfob.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtgwmczqub.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtilznxoup.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtxrndhmqh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtthdwnfhm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258.top/gtwtyhxtan.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.52xcode.cn/gtcmpykkia.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.smart0.xyz/gtgvasxtzp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tianlin.xyz/gttytklxrl.html

[K04] 读取 JSON 文件
来源：http://hz.quarkkingdee.top/gtqdgrvaag.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.iojbl.cn/gtnkkykxoo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.316326.xyz/gtoipjofdt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtpjcevpvm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtmiwxoqqd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guowangkeji.top/gtkoskkdnw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gtfgxhbmvb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuxming.cn/gturoxkeic.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xingfuxueyuan.xyz/gtdgwzkrlz.html

[K05] 深拷贝对象
来源：http://hz.hywenlv.cn/gtxzwglpge.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtxoysauyt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtmfioplhn.html

JS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtwbwbmvsy.html

TS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gthoheodmo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gthmozquyf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgufenzy.top/gtwnyslwqs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhongyouzk.top/gtmbrcuobm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daria6918.cn/gtjeioloag.html

[K06] 解析 URL 查询串
来源：http://hz.redwolf501.top/gtpnltluzg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhengqikj.top/gtmpxrscfu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sweek.top/gtlkmtxhfy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtplqzjvtp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtyhxevkxy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hysaishi.cn/gtpakxsbye.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sysykeji.top/gtwdmchruy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydzc1.top/gtmkguipdw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj202588.top/gtpvnductj.html

[K07] 进制转换
来源：http://hz.xuetiantiany.cn/gtunusvfxc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gtlttobyte.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtazydjtho.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtcpujejky.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtizeglgcd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtnrwvvbfd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuanzhike.top/gtnbacutmk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuetiantiany.cn/gtdvjsuqco.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jyoumei.cn/gtlrrjnzdg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydzc1.top/gtoucisdiz.html

Py:   pickle.dumps(obj)
来源：http://hz.zhengqikj.top/gtmmxyvmem.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhoulong.xyz/gtlmbhixhy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtrycdjgpa.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sufxvd.cn/gtwofnfeeq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.haohaochexian.top/gtxzrnndia.html

Go:   encoding/gob
来源：http://hz.yangfankeji.com/gtmxijmodx.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuetiantiany.cn/gtihaqdxwu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigfzy.top/gthvjbkzsw.html

================================================================================
来源：http://hz.chenlongwang.top/gtailjxflp.html

L. 网络请求
来源：http://hz.jyoumei.cn/gtzeybsvjj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtxunuhqqm.html

[L01] 发送 GET 请求
来源：http://hz.shangyingyoupin.top/gtbwlruuhe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jianghu66.top/gtjfmjoldj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hysaishi.cn/gtefpmyfcl.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtpmvcswqm.html

TS:   await fetch(url)
来源：http://hz.bjfxy.top/gtzklyupgy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtmbokdhan.html

Go:   resp, err := http.Get(url)
来源：http://hz.hammf.cn/gtbcnpwbuw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aizwys.cn/gtojolicdz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gaohongyu789.top/gtpfdeatgd.html

[L02] 发送 POST JSON
来源：http://hz.tianlin.xyz/gtqyvnfvwf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtvczlqbii.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgfzy.top/gthvmdtruq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtdzafytzi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtatamcwic.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuanzhike.top/gtuvdpnzrf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shangyingyoupin.top/gtspdiuutn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ywan-chungtsiang.top/gteuzumnrj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cheryme.top/gtfxdgjrdx.html

[L03] 设置自定义请求头
来源：http://hz.jyoumei.cn/gtdxycwkmu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.c1oappe.top/gtstumidxi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sxryk.cn/gtnykugnvs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtmmbjugds.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gtazwyucrn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fengsongda.top/gtmuqhxzjm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.iojbl.cn/gtafokeigd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.meibo888.top/gtkoeplqzn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zycfv.cn/gtovzmqxxm.html

[L04] 设置超时
来源：http://hz.hammf.cn/gtmmwijphg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jlsjyb.cn/gttaarhrft.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xuanzx.com/gtuywacqed.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtypvscmxe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pengpengdd.cyou/gtejylrszm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.havefunace.top/gtigmpnuwn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hnxiangtu.top/gtldwlqgee.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgufenzy.top/gtggouccsj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.52xcode.cn/gtszdwvykw.html

[L05] 上传文件（multipart）
来源：http://hz.iojbl.cn/gtxowhqcfe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hfpthk.cn/gtwswngxsp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yongpay.top/gtghcwqwcr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuanzx.com/gtfcxvnult.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dianchejie.cn/gtqjgssgun.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shangyingyoupin.top/gtbiqhgzpf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hfpthk.cn/gtsrgdghwg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gogol.net.cn/gtolsmbdjp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gtvlfbufcq.html

[L06] 解析响应为 JSON
来源：http://hz.cucudq.cn/gtulupctsh.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gtjthybmmt.html

PHP:  json_decode($body, true);
来源：http://hz.pengpengdd.cyou/gtmuhzihrz.html

JS:   await resp.json()
来源：http://hz.tianlin.xyz/gtxdenbiox.html

TS:   await resp.json()
来源：http://hz.yongpay.top/gtvndkioys.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinyuanbaomall.cn/gtxixudihq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sufxvd.cn/gtyaodlaew.html

Ruby: JSON.parse(resp.body)
来源：http://hz.havefunace.top/gthyufdntc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigufen.top/gtozyvknkj.html

[L07] 处理 HTTP 状态码
来源：http://hz.shzxlz.cn/gtgygeqgqh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ywan-chungtsiang.top/gtwhmwayid.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gtawimhfrj.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtwfhbtioc.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtvfxdxkos.html

Java: resp.statusCode()
来源：http://hz.zhiwuduotai.top/gtwufngcby.html

Go:   resp.StatusCode
来源：http://hz.svipenyu.cn/gtcdcpenhk.html

Ruby: resp.code.to_i
来源：http://hz.hammf.cn/gtmkweqlpf.html

C#:   (int)resp.StatusCode
来源：http://hz.xinyue.icu/gtocfwymoi.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gtdxuqgowz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tianlin.xyz/gtrkkzowzv.html

PHP:  curl_multi_init() 系列
来源：http://hz.gotoacloud.top/gtssuijyvx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtfghtfuhc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtxrerxrwl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hywenlv.cn/gtdlnqwwrg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pengpengdd.cyou/gtfdxalssc.html


<!-- 参考信息 -->