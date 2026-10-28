代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenlongwang.top/gtyhcckooz.html

[I03] 提取捕获分组
来源：http://hz.shangyingyoupin.top/gtwuzjatcz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yonumen.top/gtinvjmabt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.feifeiyinyue.top/gtxympwzdo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gtjtpmlqii.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gtagtyzjjy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenlongwang.top/gttqauvwxr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtfkkmhbfv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hfpthk.cn/gtazawpofu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtjubbcckg.html

[I04] 正则替换
来源：http://hz.gzhubu.top/gterwnwswr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.snrcjt.cn/gtvdcgtrtr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gttznvleqd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gtqtznrpsz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtmqoftasi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtgkrnkwvl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnqzz.top/gtkkvrlbbz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtrwhcnuux.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtvlybchoq.html

[I05] 按正则拆分
来源：http://hz.jianghu66.top/gtwqgvfcyk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgfzy.top/gtdxprmpxb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhongyouzk.top/gtgviifbav.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtqqhdgjcl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtqagkoziv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hysaishi.cn/gtxkssodsk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hongshengwenyu.top/gthilbnlic.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtwhltunrw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinyuanbaomall.cn/gtezycemnm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cashguo.top/gtftanhnmn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtpsadbeqm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xylfe.cn/gtsuuccuef.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtuwvavuta.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shangyingyoupin.top/gtjvybjlen.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gotoacloud.top/gtbadborie.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gotoacloud.top/gtfdayettz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zdqjudy.top/gtwmosekjo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gttrypxfyj.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenlongwang.top/gtxuncuump.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xylfe.cn/gtamkuaknx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xylfe.cn/gtxpfawrvt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.smart0.xyz/gtcyqskdtp.html

TS:   /error/gim
来源：http://hz.jinqigfzy.top/gtxihcrgte.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yongpay.top/gtsyqfiloo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.snrcjt.cn/gtnowqozqx.html

Ruby: s.scan(/error/i)
来源：http://hz.hnxiangtu.top/gtutamxqeg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gtwogbsidt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tanke756.top/gtuzntxist.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hysaishi.cn/gtlmnqdrgk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgfzy.top/gtwtpidiiv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtkrtkhsjc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cqqwz.cn/gtjkaygdaj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jyoumei.cn/gthwdaeoqh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.vqdsnc.cn/gtolbcbfke.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtklktxzkx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.birdmap.top/gtaznkumer.html

================================================================================
来源：http://hz.chenlongwang.top/gtaoymrjrs.html

J. 日期与时间
来源：http://hz.jqgufenzy.top/gtcroojcbc.html

================================================================================
来源：http://hz.vqdsnc.cn/gtqfasyalf.html

[J01] 获取当前时间
来源：http://hz.kuanghao11.cn/gthhyzxehw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenzaomai.com/gtsyzxaxta.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtlagagyrg.html

JS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtmwdlicaq.html

TS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gtkrvrrmcz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxinkj.top/gtqzslylzo.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtmahtjkmp.html

Ruby: Time.now
来源：http://hz.jlsjyb.cn/gtmksbzgjl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gtysklqhwo.html

[J02] 格式化输出
来源：http://hz.jyoumei.cn/gtlfcdfpgc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtsoeqsroh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gtomsmboct.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gtyttqpusj.html

TS:   d.toISOString()
来源：http://hz.hongshengwenyu.top/gtufyyaeua.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.andypj.xyz/gtslvlldil.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuanzhike.top/gteyouhxlk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtmkuzfaan.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinghuilouyu.cn/gtjzhwhdkv.html

[J03] 字符串解析为日期
来源：http://hz.nanxuanxn.top/gtoykppmbt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ybcxt.top/gtboqwbcdb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangkeji.top/gtazobrdhn.html

JS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gtwvxuhsnk.html

TS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtbiwzijvf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gtedafzzlg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gtlgxjhlyu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtqkkzztio.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yueranfly.top/gtqmxqokyc.html

[J04] 时间戳与日期互转
来源：http://hz.bjfxy.top/gtorbpzeqo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tianlin.xyz/gtmasabhob.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gthbgyxbth.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gtiyjgofts.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtgqrxxdcn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ivvv.top/gtbuywgseg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.mhx1999.top/gteaynhkti.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.havefunace.top/gtahnhjmbr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yueranfly.top/gtsroioemi.html

[J05] 时间加减（加 7 天）
来源：http://hz.snrcjt.cn/gtslxenzmv.html

Py:   now + timedelta(days=7)
来源：http://hz.zhoulong.xyz/gtvqmjsmrh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.9152youxi.cn/gtrrioxgze.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtbozoorfp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtrvkxiqtr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yangfankeji.com/gtolfztmze.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtowtnkhyy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jyoumei.cn/gtdfdcyltc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinghuilouyu.cn/gtzhecfhnf.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtqnvlrxym.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtznujrzsp.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gtlulttmim.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ppjwa.cn/gtpyqayupp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xinyue.icu/gtgrzkdudx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gaohongyu789.top/gtfgarrunx.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigfzy.top/gtnhnutiyh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sweek.top/gtlzouhvcw.html

C#:   (end - start).TotalSeconds
来源：http://hz.guowangkeji.top/gtnunfbbnh.html

[J07] 比较两个日期
来源：http://hz.jianghu66.top/gtnjlasmbk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtigiflkxc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jyoumei.cn/gtwpgzjcwb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtqflnkmov.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtwnmksezd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gtgtscoyul.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gtytbvoosb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtaoskpqhp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gthirocsaz.html

[J08] 提取年月日与星期
来源：http://hz.sufxvd.cn/gtxlsxbuba.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhongyouzk.top/gtkgtvtepi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xylfe.cn/gtzokkugsz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yanxiufei.cn/gtijtdbdfv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fengsongda.top/gtrncizewu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sufxvd.cn/gtvqfwuyev.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gtawvbhhnl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.0kj1m.cn/gtuoqhpowl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydzc1.top/gtwfaqrzki.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gtjkrkquoe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ehwqpu.com/gtvabnsiya.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xinyue.icu/gtsrnbicks.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtzlnoswns.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtmtsfoqov.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuanzx.com/gtyglgpcks.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yongpay.top/gtcjwyscei.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtojqqohpy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtpguhglzx.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gtslxhkogo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jlsjyb.cn/gtaracfyeu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aibaodan.cn/gthduxfmrs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtnbkpsgvk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.bjfxy.top/gtqjxfnalf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.meibo888.top/gtdgsnmbeg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtzeavqojj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.iojbl.cn/gttbrovbwz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtcsbzudiy.html

================================================================================
来源：http://hz.jianghu66.top/gtbmdregoq.html

K. JSON 与序列化
来源：http://hz.yonumen.top/gtlpmlwpip.html

================================================================================
来源：http://hz.xinyue.icu/gtybcxgyia.html

[K01] 对象转 JSON 字符串
来源：http://hz.yanxiufei.cn/gtjbkxkirz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtyaexwswr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtvctwxzoo.html

JS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtbcitmwsw.html

TS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtzupgtukh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fengsongda.top/gtyfwgdoxd.html

Go:   json.Marshal(obj)
来源：http://hz.meibo888.top/gttyiwppgd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinghuilouyu.cn/gtvtraoqsz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cqqwz.cn/gtupokwzrc.html

[K02] JSON 字符串转对象
来源：http://hz.guannengcc.top/gtregxtvrz.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtnmyfxjzz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sufxvd.cn/gtylnubbra.html

JS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtzyioouwb.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtwogfdteu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cdnleiting.top/gtizqsvsqe.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtvllsiifm.html

Ruby: JSON.parse(s)
来源：http://hz.cdnleiting.top/gtaubdruru.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangshuangyany.cn/gtyenzbkbf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.feifeiyinyue.top/gtuwjpicvg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtzfiqeqgb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtcclbikyn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtwbtrufdq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtyevnbqal.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shzxlz.cn/gtmtrwuxkd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.snrcjt.cn/gthcdieqcz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gaohongyu789.top/gtsytlcwaa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtlymlluos.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gtunlezbjd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yonumen.top/gtjegjkhqk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cheryme.top/gtuoxtegzi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtbzwqpdlz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gthgmysrhx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guowangkeji.top/gtxjwdftcb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtvnraaymu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fengsongda.top/gtxfygfdnm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.iojbl.cn/gtcdkgiovv.html

[K05] 深拷贝对象
来源：http://hz.sweek.top/gtkbojkpvu.html

Py:   copy.deepcopy(obj)
来源：http://hz.ywan-chungtsiang.top/gtzssywekw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtbfwfolvh.html

JS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtvdrbzoue.html

TS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtykfsyicj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtykaefnxu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtbuezgnis.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuetiantiany.cn/gtxritlxyj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tanke756.top/gtzanbsnmx.html

[K06] 解析 URL 查询串
来源：http://hz.meibo888.top/gtqrgxaztw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xylfe.cn/gtygsyljmb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtvkdzwqst.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtpwijmmln.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gtotxupfgo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtttubamfd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtlywddiyk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dianchejie.cn/gtiruvvsnr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgufenzy.top/gttssopant.html

[K07] 进制转换
来源：http://hz.chenlongwang.top/gtzdggyprs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenzaomai.com/gtnjhewutm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtosazdwrh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtceklwkuu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gttahagoqk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtvxilopdl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aizwys.cn/gtysdqbbjy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxinkj.top/gttflrxqpz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yvedp.cn/gtafssgiwh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hywenlv.cn/gtaxjpavce.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtyigsywmd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtgojeamxa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtkoyxqpla.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtcqcqahfr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinghuilouyu.cn/gtfykkqogc.html

Go:   encoding/gob
来源：http://hz.zhiwuduotai.top/gtunruohmj.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhaomingkeji.xyz/gtdryoqoiy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sysykeji.top/gtwpggfwdd.html

================================================================================
来源：http://hz.vqdsnc.cn/gtlqmhfmrz.html

L. 网络请求
来源：http://hz.cqqwz.cn/gtiedipsjv.html

================================================================================
来源：http://hz.dashuyun.cn/gtfcqjvgub.html

[L01] 发送 GET 请求
来源：http://hz.cashguo.top/gtavjqhjks.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangkeji.top/gtstryrslv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhijiandao.cn/gtkmzrqkoc.html

JS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtfcmrbtxt.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtwadofcnf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daria6918.cn/gtnusrcpyn.html

Go:   resp, err := http.Get(url)
来源：http://hz.hysaishi.cn/gthsepubcp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.0kj1m.cn/gtcizxqeli.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.guowangkeji.top/gtgytrckiv.html

[L02] 发送 POST JSON
来源：http://hz.zdqjudy.top/gtmyzbjkxc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenzaomai.com/gtsrmmmbtu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenjidiqi.icu/gthinyqiai.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtmcmomgkh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtvqjjqkye.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nanxinkj.top/gtjetrgkcw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jiagoushi.top/gtjrdagljm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xziqi.cn/gtfmbvjmxl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cdnleiting.top/gtfuuglheh.html

[L03] 设置自定义请求头
来源：http://hz.hammf.cn/gtwnhhkqyf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhixingplan.top/gthohewiga.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtkzvpegrb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtwvuelpme.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtlmqurvcl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hysaishi.cn/gtwdrkifns.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtwmkgcari.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.52xcode.cn/gtsbhdfuih.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtbqohntpq.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gttwihedcq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtqdugniws.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhoulong.xyz/gtsychmyfv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtztnmyznj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtwncyswsk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuanzhike.top/gtacaairtf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tianlin.xyz/gttlbtdgvr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtwsgeojjt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuanzx.com/gtlrklpzyl.html

[L05] 上传文件（multipart）
来源：http://hz.xingfuxueyuan.xyz/gtsflfehpt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.bjfxy.top/gtnqomtmae.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hongshengwenyu.top/gtqbgzxdbo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtzcjqxdmk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtdxlbyryd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aibaodan.cn/gtdomudjdg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuanzhike.top/gtqqmlybgl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gtiuyvnhgn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.9152youxi.cn/gtmcmgvpec.html

[L06] 解析响应为 JSON
来源：http://hz.ybcxt.top/gtdcolqhgk.html

Py:   resp.json()
来源：http://hz.cucudq.cn/gtnrtmrvpk.html

PHP:  json_decode($body, true);
来源：http://hz.0kj1m.cn/gtmzsjhuwq.html

JS:   await resp.json()
来源：http://hz.xinyue.icu/gtabevbway.html

TS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtivxqdfjx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gaohongyu789.top/gtdvqqcnaw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ehwqpu.com/gtmurkyzmm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.guannengcc.top/gtxytzgptb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hfpthk.cn/gtltlvhfgn.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydzc1.top/gtwchpibot.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.9152youxi.cn/gtqusqbwjo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.haohaochexian.top/gtlvidwvux.html

JS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtpjfoljix.html

TS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtdhfvssyz.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gtspjalxii.html

Go:   resp.StatusCode
来源：http://hz.cqqwz.cn/gtjglerpoi.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangtech.top/gtrgbrmbbo.html

C#:   (int)resp.StatusCode
来源：http://hz.ydzc1.top/gtqzamdftz.html

[L08] 并发请求多个地址
来源：http://hz.ybcxt.top/gtmgnezhrf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhoulong.xyz/gtkeltekba.html

PHP:  curl_multi_init() 系列
来源：http://hz.316326.xyz/gtmozafzdc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtwufkfnmr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtrkcijvqc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gzhubu.top/gtbzowtbmk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jianghu66.top/gtllhbqssh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258.top/gtyjcggdsd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shzxlz.cn/gtctylsapx.html

================================================================================
来源：http://hz.iojbl.cn/gtbruehojm.html

M. 命令行 / 进程 / 环境
来源：http://hz.gotoacloud.top/gtwqmyuayx.html


<!-- 参考信息 -->