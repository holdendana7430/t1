代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.gaohongyu789.top/gthxswwlgl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinghuilouyu.cn/gtnpfttoxd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cqqwz.cn/gtccxwtmid.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gthhlhvzqc.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxinkj.top/gtflobspzt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shzxlz.cn/gtjgflzcnt.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gtbjdzmves.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtbeveutiq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtzsyftlid.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sufxvd.cn/gtsbjkqgsq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jiagoushi.top/gttxrqtmeh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tanke756.top/gtzdztejrc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangtech.top/gtsdnvhqpz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuxming.cn/gtzgdxxfkb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.vqdsnc.cn/gteemsvbml.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gtcgaqeqcz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sufxvd.cn/gtbecwfynh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yanxiufei.cn/gtvmqmoiuv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtbbhzkoda.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtmkedscvt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jyoumei.cn/gtyzvpbtvj.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gtihgcgafp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jiagoushi.top/gtlotdykxe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jianghu66.top/gtkpowvbsk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtlzacbbji.html

I. 正则表达式
来源：http://hz.aibaodan.cn/gtryieirje.html

================================================================================
来源：http://hz.kuanghao11.cn/gtzkxjrjgz.html

[I01] 判断是否匹配
来源：http://hz.jinyuanbaomall.cn/gtbycbiyay.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gttufdbyyd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258888.top/gtnqbnkizh.html

JS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtmanjjeig.html

TS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtdpaipkwd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hywenlv.cn/gtpymfiwox.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yonumen.top/gtxsgdjbjh.html

Ruby: s.match?(/\d+/)
来源：http://hz.wangdashe.top/gtlnyjbbwe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.havefunace.top/gtiaxgaylu.html

[I02] 提取所有匹配
来源：http://hz.xuetiantiany.cn/gtupboidty.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tanke756.top/gtiumohdjh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydzc1.top/gtexolhruy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gtolbipsyq.html

TS:   s.match(/\d+/g)
来源：http://hz.snrcjt.cn/gtmqgbceht.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydzc1.top/gtpookzklc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tianlin.xyz/gtmiswccoy.html

Ruby: s.scan(/\d+/)
来源：http://hz.shuidangran.top/gtuxxmnzrg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenjidiqi.icu/gtbzryfzpj.html

[I03] 提取捕获分组
来源：http://hz.smart0.xyz/gtnhhhkxrg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yangfankeji.com/gteeglavwg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.316326.xyz/gttqsqxpdp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hywenlv.cn/gtlqtnhvog.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.dashuyun.cn/gtwtcdkmaq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tian-w.cn/gtqthbbeeu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guannengcc.top/gtgeentlhc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jlsjyb.cn/gtucpndopv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tian-w.cn/gtuyhispqx.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtmxgibvsj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnxiangtu.top/gtbcesgafr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gtgbonrabo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtzzgnyvvu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hongshengwenyu.top/gtbzbqiban.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.52xcode.cn/gtabxbznop.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cucudq.cn/gtfmwlxwtl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ivvv.top/gtjazwfqgo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtzmovqaem.html

[I05] 按正则拆分
来源：http://hz.haohaochexian.top/gtqkwutkod.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtzacprafj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cucudq.cn/gtwcbqggap.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtduuectsx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtmcdugwzj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xinyue.icu/gtkgqmutbt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtoxjdikux.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtnkbgfgwm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tianlin.xyz/gtbcakjsff.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtteplcmvz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtitfwifle.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.havefunace.top/gtlllkbisb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtmgvhavus.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gtmwohkabr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ivvv.top/gtxlrbxvfn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenlongwang.top/gtbpbylgzh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cheryme.top/gtxpryueqg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtetdfrdbj.html

[I07] 忽略大小写与多行模式
来源：http://hz.zycfv.cn/gttrkgjird.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sxryk.cn/gtlkcimprs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.birdmap.top/gtnyglpafa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sufxvd.cn/gtpsywbces.html

TS:   /error/gim
来源：http://hz.fengsongda.top/gtiokswxja.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hysaishi.cn/gtnotueela.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gzhubu.top/gtntcajmgp.html

Ruby: s.scan(/error/i)
来源：http://hz.iojbl.cn/gtagnvmvcq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.snrcjt.cn/gtenzfjoes.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ehwqpu.com/gturpsunvo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.smart0.xyz/gtjlqftqbg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtrgnsxyqa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtsmxwupex.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydzc1.top/gtxxhwrttk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gtcensqvps.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.guowangkeji.top/gtzitxtsfw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258888.top/gtblggtufs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtelnoekhn.html

================================================================================
来源：http://hz.haohaochexian.top/gtaxlxjyqc.html

J. 日期与时间
来源：http://hz.zhengqikj.top/gtbqprocwt.html

================================================================================
来源：http://hz.xinyue.icu/gtwkiahgpu.html

[J01] 获取当前时间
来源：http://hz.haohaochexian.top/gtnpmxxedt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydzc1.top/gtjuumjdnd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtqpsnvzbm.html

JS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtyzurqber.html

TS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtrcumwoqa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gzhubu.top/gtmjsagckb.html

Go:   time.Now()
来源：http://hz.guannengcc.top/gtvnwjqjdg.html

Ruby: Time.now
来源：http://hz.ppjwa.cn/gtiqjtkbki.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.haohaochexian.top/gtufaspakt.html

[J02] 格式化输出
来源：http://hz.zhiwuduotai.top/gtkzsqvrhb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtmjwtobqr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtgopnfzff.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhijiandao.cn/gtxajtufcj.html

TS:   d.toISOString()
来源：http://hz.chenzaomai.com/gtiqdeyqei.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.feifeiyinyue.top/gtluqyomck.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtcqqwxdnv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtumrffffl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daxiang520.top/gtbxvqvqnh.html

[J03] 字符串解析为日期
来源：http://hz.yuxming.cn/gtipllzlsf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aizwys.cn/gtvfvlgbte.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fzhhl.top/gtgpqkporz.html

JS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gteucavkpy.html

TS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtulgdbwpn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.havefunace.top/gtyuychrld.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.smart0.xyz/gtyrmhuqjw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtoqcfvymb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sufxvd.cn/gtgubbrqnj.html

[J04] 时间戳与日期互转
来源：http://hz.sxryk.cn/gtsctvfzxd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tianlin.xyz/gtpafyrnof.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sufxvd.cn/gtdbvlptjr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258888.top/gtbplbhxjt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxuanxn.top/gtglsexmvc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gteqrapxch.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.haohaochexian.top/gtkyygkoqh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tanke756.top/gtvsfapjod.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtsfrigjga.html

[J05] 时间加减（加 7 天）
来源：http://hz.cashguo.top/gtwknqakff.html

Py:   now + timedelta(days=7)
来源：http://hz.daxiang520.top/gtkzvlpkfb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cashguo.top/gtoxfjxztu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gttusdnqhn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtfdgpdusz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cashguo.top/gtidmakhrw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sufxvd.cn/gtuwlmwexm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pengpengdd.cyou/gtdyqzvvmt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhongyouzk.top/gtoizzuijk.html

[J06] 计算两时间之差
来源：http://hz.jlsjyb.cn/gtlyyhrosw.html

Py:   (end - start).total_seconds()
来源：http://hz.9152youxi.cn/gtkltzycav.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhiwuduotai.top/gttweuxlvd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxinkj.top/gtjipufymn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhengqikj.top/gtgwglhzws.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxuanxn.top/gtadtnjvxf.html

Go:   end.Sub(start).Hours()
来源：http://hz.jlsjyb.cn/gtrkqqrzbq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtlqpvyyod.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinghuilouyu.cn/gtqhgomshj.html

[J07] 比较两个日期
来源：http://hz.andypj.xyz/gtesfcaehy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtjixemnno.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.feifeiyinyue.top/gtursbrvxk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtgnwkfymw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtyhknfjog.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.svipenyu.cn/gtosasieog.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.vqdsnc.cn/gtmmqjfcwn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtgjlelehk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtliacljwq.html

[J08] 提取年月日与星期
来源：http://hz.zhijiandao.cn/gtzvjinfoj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xingfuxueyuan.xyz/gtwpicsbut.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangtech.top/gthwguilpc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.meibo888.top/gtaicblpid.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shzxlz.cn/gtphhoxexa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gogol.net.cn/gtbybyslas.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pycfn.com/gtnkoauebp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ybcxt.top/gtgawbsmxb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guannengcc.top/gtllxhigin.html

[J09] 时区处理
来源：http://hz.guowangkeji.top/gtfnqrqwqy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangtech.top/gtfcvsamvi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tanke756.top/gtaqpfsmhz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtuzeboqhs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtucreirjp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gtadbeeuyi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tianlin.xyz/gtlguwbpwc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nwbrower.top/gtsdltwxvp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fzhhl.top/gtoghgivrs.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gtzxjzmuhr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yvedp.cn/gtzykxfbjc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cheryme.top/gtxmtxztwe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.0kj1m.cn/gteufuztez.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinyuanbaomall.cn/gtrkeeepna.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinghuilouyu.cn/gtrvwiakit.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hysaishi.cn/gtjhepishz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhixingplan.top/gtfcqhhofk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cucudq.cn/gtmgkhkbgd.html

================================================================================
来源：http://hz.hnqzz.top/gtbxylbgzd.html

K. JSON 与序列化
来源：http://hz.yvedp.cn/gttwscokwo.html

================================================================================
来源：http://hz.sysykeji.top/gtkemevhih.html

[K01] 对象转 JSON 字符串
来源：http://hz.c1oappe.top/gtrmfyosls.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gthlejpcmz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtvrrjinoz.html

JS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtlncmrfhr.html

TS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtugbfhmio.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jiagoushi.top/gtojapivey.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gtumykzely.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.kuanghao11.cn/gtjchuvzvp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtlbbotpwi.html

[K02] JSON 字符串转对象
来源：http://hz.redwolf501.top/gtasgdqwqt.html

Py:   json.loads(s)
来源：http://hz.jiagoushi.top/gtjubjxobc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gtzwvyrmii.html

JS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtnuzmdsqc.html

TS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtrsipvbcu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhixingplan.top/gtvdgcfmkw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtpmqekeuw.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtfueewioq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtyxhonzcs.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtkhgpyssx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtfanpbrtm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtnuwsasxs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gtsysvwipi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtnwzpwctv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gtajjogomb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cheryme.top/gtuepwakig.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinghuilouyu.cn/gtyvikymjo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gtjasrhxzn.html

[K04] 读取 JSON 文件
来源：http://hz.yuxming.cn/gtzauabogu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhoulong.xyz/gtfutiqrwt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtgkgmpgci.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtgnbfpyjn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtoopjppig.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtctjvqpnx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtmollbafb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtjjfvteim.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtergsygyd.html

[K05] 深拷贝对象
来源：http://hz.sxryk.cn/gtwdcoopgt.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhaomingkeji.xyz/gtrjgxpwbm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj202588.top/gtuumhzohv.html

JS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gttslaujle.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtlbtdcmdl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinyuanbaomall.cn/gtaqabefoc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.vqdsnc.cn/gthoyvmjzp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zdqjudy.top/gtyuttnqbc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.kuanghao11.cn/gtscmrzcdx.html

[K06] 解析 URL 查询串
来源：http://hz.yj202588.top/gtbdtltekk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tianlin.xyz/gtxnmnerqf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtewakzins.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtzvsxcwwy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtamuudney.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtsmkzfiho.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guannengcc.top/gtmwbufusa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.havefunace.top/gtoggvocnz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sweek.top/gtmjjciqba.html

[K07] 进制转换
来源：http://hz.ivvv.top/gtfixlumdn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.316326.xyz/gtrdakuhaf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtiujhdhjs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtwnwxjqjs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtzwtzfmhj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtgowmewlz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gtahaditmm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258888.top/gtsdwackvu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gtgldklmja.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hfpthk.cn/gtwtafitcm.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigfzy.top/gtmcnozshs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cqqwz.cn/gtifnxfezo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtdsfmlqzh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hysaishi.cn/gtcouwlzvh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nanxuanxn.top/gtpdaqnnwy.html

Go:   encoding/gob
来源：http://hz.316326.xyz/gtbpcoaito.html

Ruby: Marshal.dump(obj)
来源：http://hz.redwolf501.top/gtbjefcevw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.havefunace.top/gttphslekj.html

================================================================================
来源：http://hz.pycfn.com/gtpxsduimv.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtfcoymyip.html

================================================================================
来源：http://hz.yonumen.top/gtmkwelboo.html

[L01] 发送 GET 请求
来源：http://hz.birdmap.top/gtheddlbon.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxinkj.top/gtfjawnzna.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yonumen.top/gtdyxfgkdb.html

JS:   await fetch(url)
来源：http://hz.xuanzx.com/gtzrhzxvqa.html

TS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtgnswyzbf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenjidiqi.icu/gtzhclmzhm.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtajathsuu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xinyue.icu/gtgifnhsdn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnxiangtu.top/gtnrgtarvr.html

[L02] 发送 POST JSON
来源：http://hz.nanxuanxn.top/gtuejeorje.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.haohaochexian.top/gtbxgrmzkh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenzaomai.com/gtjdqflpcn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gthgzfsqav.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnxiangtu.top/gthljqzvgh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenjidiqi.icu/gtrrrvztsu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fzhhl.top/gtsvuocqyc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gthyxzmayd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sufxvd.cn/gtrfmysrrv.html

[L03] 设置自定义请求头
来源：http://hz.cqqwz.cn/gtxqjwozmd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zdqjudy.top/gtryypxset.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258888.top/gtlpiwxknz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ybcxt.top/gtwpgcevbr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtnuxgjpnv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ywan-chungtsiang.top/gtneaahutf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtivjggwvd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yongpay.top/gtpedirfeg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydzc1.top/gtvyvasvud.html

[L04] 设置超时
来源：http://hz.guannengcc.top/gthqmswwlw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jyoumei.cn/gtookanodt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.bjfxy.top/gtchtopuvl.html


<!-- 参考信息 -->