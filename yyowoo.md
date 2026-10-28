代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtwjmyhebx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.kuanghao11.cn/gtarvcmxfs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.meibo888.top/gtulydjucx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj202588.top/gtoncvlxvo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigufen.top/gtsegajmof.html

[H08] 获取错误信息与堆栈
来源：http://hz.jianghu66.top/gtvxeewwcu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtrgnuvdfq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zycfv.cn/gtkyewellz.html

JS:   e.message;  e.stack
来源：http://hz.zhengqikj.top/gtpzvtsrmw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.9152youxi.cn/gtckpzaxba.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenlongwang.top/gtggpheoym.html

Go:   err.Error()
来源：http://hz.c1oappe.top/gtnkauddji.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gtpzpnwtml.html

C#:   e.Message;  e.StackTrace
来源：http://hz.c1oappe.top/gthjngqpqt.html

[H09] 带错误码的异常
来源：http://hz.zdqjudy.top/gtkdndzfpd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangdashe.top/gtgaknzbgi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxuanxn.top/gtvkelnhjp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258888.top/gtqqkkcyac.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenlongwang.top/gthjrlprif.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gtnonrobyg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtoyzdealc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gaohongyu789.top/gtdyrvjzhu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.9152youxi.cn/gthyhnwkmj.html

[H10] 资源自动释放
来源：http://hz.hfpthk.cn/gtyvtvcxog.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.meibo888.top/gtcblobrlc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtowtxrkoa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydzc1.top/gtjdbcbump.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtrmahnowk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.vqdsnc.cn/gttxkrplvm.html

Go:   defer f.Close()
来源：http://hz.yuxming.cn/gtgypgvrai.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.svipenyu.cn/gttbqpduud.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dashuyun.cn/gtxpohjdht.html

================================================================================
来源：http://hz.jyoumei.cn/gtatdizmnw.html

I. 正则表达式
来源：http://hz.xuanzx.com/gtwvwbfuyw.html

================================================================================
来源：http://hz.wangdashe.top/gtakvhdzvx.html

[I01] 判断是否匹配
来源：http://hz.tian-w.cn/gtpjkvvfcj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cheryme.top/gtlzzuhnje.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hysaishi.cn/gtqigmernj.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gtkpxlhwax.html

TS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtmenyzzoc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.meibo888.top/gtivgnocul.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenlongwang.top/gtbkihekxe.html

Ruby: s.match?(/\d+/)
来源：http://hz.hfpthk.cn/gtvzqyzkrr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xinyue.icu/gtcxjlsfob.html

[I02] 提取所有匹配
来源：http://hz.yj202588.top/gtvygswgaa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.c1oappe.top/gtpsyhryui.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.9152youxi.cn/gtinhpgfdu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhijiandao.cn/gtjldemnkn.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgfzy.top/gtulncclin.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hfpthk.cn/gtqtavmpru.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ydzc1.top/gtmviztfwz.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhengqikj.top/gtmencfbfd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.birdmap.top/gtooakpify.html

[I03] 提取捕获分组
来源：http://hz.xuanzx.com/gtkldqvote.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aibaodan.cn/gtmwanoxfg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hnqzz.top/gtmgqldtch.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shangyingyoupin.top/gtmbujqhkg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxuanxn.top/gtzziwpwgh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sxryk.cn/gtxyblsles.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangkeji.top/gtofbbjgof.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daria6918.cn/gtfrcntppn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxinkj.top/gtfsufbzrb.html

[I04] 正则替换
来源：http://hz.jqgfzy.top/gtnkzhoyyo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinghuilouyu.cn/gtaadqziok.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cdnleiting.top/gtkyorbwdq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtyfjsgiyt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtvcrolmvr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gtcczqbsun.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yonumen.top/gtybimbfgf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.52xcode.cn/gtvgfxemrk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenjidiqi.icu/gtminljssd.html

[I05] 按正则拆分
来源：http://hz.ydzc1.top/gtabpnyimw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtwmiwxvco.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.316326.xyz/gtunkdfwfq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtvdgugzcj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtdcljyyom.html

Java: s.split("\\s*,\\s*")
来源：http://hz.wangdashe.top/gtzlubduuh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zdqjudy.top/gtnnlqrcud.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtcufhhpak.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gtebssbies.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuetiantiany.cn/gtfmdeyzzy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtxiirjezy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.andypj.xyz/gtbscnyjgy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuetiantiany.cn/gtbmtifqiy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtytvxznjm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtvxfjftnl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxuanxn.top/gtqtobdkgz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.haohaochexian.top/gtibpxixft.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.vqdsnc.cn/gtvuklbsof.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtedksuqfl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.mhx1999.top/gtfyrhvehu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.snrcjt.cn/gtdbovxale.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.redwolf501.top/gtbkrzcowg.html

TS:   /error/gim
来源：http://hz.chenzaomai.com/gttdxqbzib.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cqqwz.cn/gteprsxvlk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cdnleiting.top/gtektqhfry.html

Ruby: s.scan(/error/i)
来源：http://hz.iojbl.cn/gtmqtiuamm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.52xcode.cn/gtnvoexwtm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj20258888.top/gttqlycipu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pengpengdd.cyou/gtdntfupmt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ppjwa.cn/gtelpsuccm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gthxhdklol.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtsbokmnar.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cucudq.cn/gtpepmnmoc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.0kj1m.cn/gtexkqjsgr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.c1oappe.top/gttpggnjwu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtqbdnrwof.html

================================================================================
来源：http://hz.jqgfzy.top/gtxkfdqrqi.html

J. 日期与时间
来源：http://hz.zhoulong.xyz/gtqsuwaemi.html

================================================================================
来源：http://hz.sysykeji.top/gtncuhvhwh.html

[J01] 获取当前时间
来源：http://hz.cheryme.top/gthmpmtxwo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtjunpzpwo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtxglmikus.html

JS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtbtdphqfs.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtjbqjggzi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtchogshsb.html

Go:   time.Now()
来源：http://hz.ydzc1.top/gtzshfohhn.html

Ruby: Time.now
来源：http://hz.jqgufenzy.top/gtkukgrvne.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nwbrower.top/gtpdtpufqm.html

[J02] 格式化输出
来源：http://hz.yuanzhike.top/gtklcetazd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pengpengdd.cyou/gtghldalwq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gteoddhfnc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hywenlv.cn/gtyazstdgv.html

TS:   d.toISOString()
来源：http://hz.ivvv.top/gtbtsemjea.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangkeji.top/gtlqejxhev.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.andypj.xyz/gtivoftkew.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtxyvzrgpg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtcknokqpw.html

[J03] 字符串解析为日期
来源：http://hz.sxryk.cn/gtmgzuynbv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jyoumei.cn/gthkqixbhg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xylfe.cn/gtchugicjw.html

JS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtmbjfavpz.html

TS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gtgzgcgzko.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtfluteakw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gotoacloud.top/gtnjczrazl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtvrupyscv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yueranfly.top/gtiospytjd.html

[J04] 时间戳与日期互转
来源：http://hz.hammf.cn/gtrdcdiqlw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.birdmap.top/gtcimkvjxt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuxming.cn/gtgbvsgzqr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258888.top/gttehqgizx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.316326.xyz/gtthxdzffx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cqqwz.cn/gtbmckmgqy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yueranfly.top/gtnmamfodu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cdnleiting.top/gttdigerry.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yvedp.cn/gtwtxozzks.html

[J05] 时间加减（加 7 天）
来源：http://hz.zycfv.cn/gtsfyiiynn.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgufenzy.top/gtdtxiuqvg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hfpthk.cn/gtpodmjent.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gttbpquyzx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtwtamhejl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gogol.net.cn/gtkgnemaca.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtjexesthm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guannengcc.top/gtogygwmob.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtqyfzocuq.html

[J06] 计算两时间之差
来源：http://hz.xuetiantiany.cn/gtsvkifunk.html

Py:   (end - start).total_seconds()
来源：http://hz.hfpthk.cn/gtaqnhaato.html

PHP:  $end->diff($start)->days;
来源：http://hz.fengsongda.top/gtxprpooam.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shangyingyoupin.top/gtzgnpzwic.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yueranfly.top/gtujkcrapa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guowangkeji.top/gtfnaqlove.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuanzhike.top/gtesmcepiy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aizwys.cn/gtgyrtltdi.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenlongwang.top/gtncckmeyi.html

[J07] 比较两个日期
来源：http://hz.hammf.cn/gtbonzehhk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtlfpznkli.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtfjyllkmb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtyclslaup.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtworudnxv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yonumen.top/gtnlvcbcqd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gtvniyiygi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtwerousnk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtctcwgmcm.html

[J08] 提取年月日与星期
来源：http://hz.tian-w.cn/gtjyiityav.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhiwuduotai.top/gtnlfrkima.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yuanzhike.top/gtwnwqkeat.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.snrcjt.cn/gtklfdwqlj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gtmwgkovix.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtwevteytj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtidrvmlgo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxinkj.top/gtfnqlepyt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtzkpyipxc.html

[J09] 时区处理
来源：http://hz.52xcode.cn/gtwzwrhupp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gogol.net.cn/gtzdrrmphb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gtztkcxvrp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtvfyuwvjq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtybjqajdc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj202588.top/gtpcpvmkck.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.wangdashe.top/gtvzizhdrj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yanxiufei.cn/gtaejfjhju.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnqzz.top/gturddarzp.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gtjsxupofd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.iojbl.cn/gtyvfjajsk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtayhxylwp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gtzcqopgwe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.daria6918.cn/gtkzqkxkol.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhaomingkeji.xyz/gtadigihxu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hammf.cn/gtcpjzackm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.redwolf501.top/gtmphurqsj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cdnleiting.top/gtzmgxymar.html

================================================================================
来源：http://hz.bjfxy.top/gthvlflaea.html

K. JSON 与序列化
来源：http://hz.gzhubu.top/gtfuskyeca.html

================================================================================
来源：http://hz.haohaochexian.top/gtnyaowqxk.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhongyouzk.top/gtptfzudgd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pycfn.com/gtxcxlyhvl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtyiojmyuz.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtfbkbdyla.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtfczlghcx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ppjwa.cn/gtnxjrzxkz.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtibroarfy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yueranfly.top/gtgmlhsomt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zdqjudy.top/gtgqhzrdaj.html

[K02] JSON 字符串转对象
来源：http://hz.hnqzz.top/gttmzulunt.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtqcxhasho.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ybcxt.top/gtcwhdmrkf.html

JS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtdeonrvel.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtjxrxzexl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cashguo.top/gteqnyzxsi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gthhphbbpt.html

Ruby: JSON.parse(s)
来源：http://hz.mhx1999.top/gtnoqkfajk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuetiantiany.cn/gtcsmgqpdl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.kuanghao11.cn/gtkccsfbdp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtxlomornj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtjzsqphmd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtrhpefado.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtojyynngg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhongyouzk.top/gtqgkxqqlf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pycfn.com/gtccdlkluj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.guannengcc.top/gtaqlyziop.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinyuanbaomall.cn/gtgfrajwcr.html

[K04] 读取 JSON 文件
来源：http://hz.birdmap.top/gtfwxflkaf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jyoumei.cn/gtofcguuzw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hammf.cn/gtwnqxwgls.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtdpiojdil.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gtvuzhnohd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aibaodan.cn/gtpujuqfli.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtgnicjwqv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.316326.xyz/gtkowotuug.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cdnleiting.top/gtxhzrofxy.html

[K05] 深拷贝对象
来源：http://hz.havefunace.top/gtmjjyqvhw.html

Py:   copy.deepcopy(obj)
来源：http://hz.andypj.xyz/gtjcowlmnz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.andypj.xyz/gtupkoseni.html

JS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtkiigezrs.html

TS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtjgmdprlc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangdashe.top/gtpsofchtq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.birdmap.top/gtnhybwcbe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.mhx1999.top/gtfcnpjatb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangdashe.top/gtktkhpgwk.html

[K06] 解析 URL 查询串
来源：http://hz.wangshuangyany.cn/gtmckhmvzz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.quarkkingdee.top/gtijpzywbd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtkqitqlxg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtaospmngf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtydynwgkz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenjidiqi.icu/gtwnxippjn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aibaodan.cn/gtidcfgvkj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gttjmtryus.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtzbfpzrla.html

[K07] 进制转换
来源：http://hz.feifeiyinyue.top/gtmmxbjtsn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhongyouzk.top/gtxoqvxfbg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sxryk.cn/gtnohlnlrh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtppanbpar.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtqhurtndy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtxnkgcpyp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fzhhl.top/gteswnepzw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtcjvmcgqt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gaohongyu789.top/gtbmwsvnpv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gaohongyu789.top/gttdwconzu.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtwhncvenu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhongyouzk.top/gtqtgrkrbt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtmoaevydz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtjyhrapnq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgfzy.top/gtfdkljmio.html

Go:   encoding/gob
来源：http://hz.quarkkingdee.top/gtoffrwebv.html

Ruby: Marshal.dump(obj)
来源：http://hz.birdmap.top/gtacepmusk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.redwolf501.top/gtxutxdrzk.html

================================================================================
来源：http://hz.guowangkeji.top/gtsdjgsgsf.html

L. 网络请求
来源：http://hz.ydzc1.top/gtqpsmcndt.html

================================================================================
来源：http://hz.hfpthk.cn/gtxwcbtnul.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gtvicnfgyr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aibaodan.cn/gtlgjgjqeh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtpqhkjeki.html

JS:   await fetch(url)
来源：http://hz.fzhhl.top/gtxgyytdmx.html

TS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtavdvkeit.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zycfv.cn/gtrutamjdq.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgufenzy.top/gthfhixagj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ybcxt.top/gtnltiacvm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnxiangtu.top/gtacaqsgip.html

[L02] 发送 POST JSON
来源：http://hz.gotoacloud.top/gtevuxmict.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhixingplan.top/gtonmzolye.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gotoacloud.top/gtqggjsgif.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtuuyxwzvt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtsirpxtol.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jiagoushi.top/gtennxyqox.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.smart0.xyz/gtvyofzgpx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tianlin.xyz/gtmohxxaxf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.quarkkingdee.top/gtypjrxyyv.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtljswuhji.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cdnleiting.top/gtskabxitq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtyfebhiwj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtbcfcntdv.html


<!-- 参考信息 -->