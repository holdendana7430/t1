代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtbznhukrl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhengqikj.top/gtsncqypgf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtjauicaiy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.redwolf501.top/gtddukrefh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258.top/gtouftmepb.html

[H08] 获取错误信息与堆栈
来源：http://hz.xylfe.cn/gttfozsvtd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gthylwdkek.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gaohongyu789.top/gtlfmcbtrt.html

JS:   e.message;  e.stack
来源：http://hz.yueranfly.top/gtjutknuzf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dashuyun.cn/gtuiugfnem.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ybcxt.top/gtetntbhac.html

Go:   err.Error()
来源：http://hz.jinqigufen.top/gtflhlyqgh.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gtqmbuujcc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ivvv.top/gtsblbuxuu.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtoucuwuii.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.0kj1m.cn/gteaessbdp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.meibo888.top/gtiujhsalu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guannengcc.top/gtjbzsrzvk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yongpay.top/gtqcxqzgev.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.c1oappe.top/gtadhupisn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnqzz.top/gtpgfodubd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xylfe.cn/gtgsuxekxx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.birdmap.top/gtnsiumbbe.html

[H10] 资源自动释放
来源：http://hz.havefunace.top/gtipaggywv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gzhubu.top/gtcakuqhyk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtslxkbcpx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtzplqixrd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtzdsapqyg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.0kj1m.cn/gtaxdxjfim.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gtqpdyqkuv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtdzxqjgek.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gzhubu.top/gtpdyirufq.html

================================================================================
来源：http://hz.andypj.xyz/gthupnmwwq.html

I. 正则表达式
来源：http://hz.ywan-chungtsiang.top/gtpeqrydwq.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqkytblir.html

[I01] 判断是否匹配
来源：http://hz.gotoacloud.top/gtxdwdtjtv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258.top/gtdlrephug.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.c1oappe.top/gtsjdfgvdu.html

JS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtikrbsqhu.html

TS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtpljsfesv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtdklqrbwd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigufen.top/gtmotkjreu.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gtxnawccwh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gtskzpumat.html

[I02] 提取所有匹配
来源：http://hz.52xcode.cn/gtbluwuqhy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zycfv.cn/gtofpdxjvz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pycfn.com/gtfqvpwmle.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fzhhl.top/gtqvqyxlmt.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtduggiqpy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuxming.cn/gtctjeykfc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigfzy.top/gtspvpuays.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtgwgklflo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gtdgnsfshs.html

[I03] 提取捕获分组
来源：http://hz.sweek.top/gtskicfuya.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guannengcc.top/gtliglkixd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.bjfxy.top/gturoilrii.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuxming.cn/gtnlybfwmc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnqzz.top/gtakmjeojy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhiwuduotai.top/gtczzrojbu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.9152youxi.cn/gtfzbyryop.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ybcxt.top/gtgabboure.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.svipenyu.cn/gtrbpvpwui.html

[I04] 正则替换
来源：http://hz.zhijiandao.cn/gtjilblcgk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sweek.top/gtwtggmmof.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gthyubxekt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtrzliylsf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtlscbddvc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxinkj.top/gtttgizfwo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zycfv.cn/gtalhkdflb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yvedp.cn/gtandtogrw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxuanxn.top/gtognqljgu.html

[I05] 按正则拆分
来源：http://hz.zhoulong.xyz/gtagmlekde.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.snrcjt.cn/gtwsowjpaa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tanke756.top/gtnhdlxlzd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtpywqdooq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtrsdtwggu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xziqi.cn/gtfwmclxhv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.c1oappe.top/gtehbugtht.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtjmrdkewl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aizwys.cn/gtjniizdan.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gtoireeqwc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gthzbvtwmj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zdqjudy.top/gtjofnnxcg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtpkkucnae.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtvraszjmg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ybcxt.top/gtdshblfxc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.9152youxi.cn/gtkzwvrnzc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuxming.cn/gtzhcvtggm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtnclkwxrg.html

[I07] 忽略大小写与多行模式
来源：http://hz.hfpthk.cn/gtecyglsds.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gtouwpnxal.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxinkj.top/gtsyyonjbn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sxryk.cn/gtcbaohhiq.html

TS:   /error/gim
来源：http://hz.guannengcc.top/gtbwglbayt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hfpthk.cn/gtmlpeioyj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pengpengdd.cyou/gtvalmzook.html

Ruby: s.scan(/error/i)
来源：http://hz.zhengqikj.top/gtqezvmyyt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cucudq.cn/gtuzaxktew.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuanzx.com/gtzsixvbuc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtpojifgmq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jyoumei.cn/gtqklovihg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gttkxyoghe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gteizoqwvu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtqapfnoxh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aibaodan.cn/gtnyznmjzm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gthkboebke.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yueranfly.top/gtuastfqqr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtijmhqbts.html

J. 日期与时间
来源：http://hz.shanyushiyangkeji.top/gtrnqajqdm.html

================================================================================
来源：http://hz.yonumen.top/gteduwdmkm.html

[J01] 获取当前时间
来源：http://hz.zhixingplan.top/gtfrlqvbtj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dashuyun.cn/gtsnzokqmz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gttoeovbag.html

JS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gtakywsyaf.html

TS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gtmdarnmut.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.9152youxi.cn/gtcscfrhgr.html

Go:   time.Now()
来源：http://hz.zhixingplan.top/gtztakhcwp.html

Ruby: Time.now
来源：http://hz.havefunace.top/gtfaqcctgh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sysykeji.top/gtpkzlodxb.html

[J02] 格式化输出
来源：http://hz.ydjk.org.cn/gtvlvpxnhq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtqgmixjgu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtibfavaqp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuxming.cn/gtudfldryy.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtxqdhlfru.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pengpengdd.cyou/gtlkicppjz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cashguo.top/gtbjrqgzlu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtmhttxhkl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuanzhike.top/gtdytaiqpj.html

[J03] 字符串解析为日期
来源：http://hz.kuanghao11.cn/gtsofjqrwk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnqzz.top/gtocchcqex.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aizwys.cn/gtbmqvwcdi.html

JS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtcnphjfin.html

TS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtqwjjvhiw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtchjsdput.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.kuanghao11.cn/gtdqqnjiiu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtwwtbusmb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jyoumei.cn/gtbhywgxpf.html

[J04] 时间戳与日期互转
来源：http://hz.meibo888.top/gtvatrnobt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxinkj.top/gtvnkwbqbj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xziqi.cn/gttibgdwlf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dianchejie.cn/gtewvxxrhp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.316326.xyz/gtppjdvznp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydjk.org.cn/gtidkdfscn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cdnleiting.top/gtrgrotfdd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gthwwemrid.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jianghu66.top/gtfpejxxwd.html

[J05] 时间加减（加 7 天）
来源：http://hz.yuxming.cn/gtuqpihnxe.html

Py:   now + timedelta(days=7)
来源：http://hz.guannengcc.top/gtmerwkynh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhixingplan.top/gttpaneyqf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtrsslvzgw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yongpay.top/gthhtximzo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigfzy.top/gtlhytjtlr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxuanxn.top/gtlgygusbo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guowangkeji.top/gtrpdooyqb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuxming.cn/gtvewkmxnh.html

[J06] 计算两时间之差
来源：http://hz.kuanghao11.cn/gtjkgrclkd.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gtjqpujtum.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtyzzolpka.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jlsjyb.cn/gttffuvhoa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.52xcode.cn/gtyzevwbfj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tianlin.xyz/gtstcozoss.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtglhdtfyp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cashguo.top/gtvwhatzdi.html

C#:   (end - start).TotalSeconds
来源：http://hz.guannengcc.top/gtdidfppkz.html

[J07] 比较两个日期
来源：http://hz.gotoacloud.top/gtxezdkffg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtvvlrqgvk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gthbtqdxjx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtenjamdyk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtmizlyqqc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtruyrxufw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtkanxidjx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtzzfuzbar.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtzvutwwcg.html

[J08] 提取年月日与星期
来源：http://hz.cashguo.top/gtgkualcqu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jianghu66.top/gtmdhzhdpi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xziqi.cn/gtsgtfetiy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtmcpgfoca.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhoulong.xyz/gtimyqxrjr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhixingplan.top/gtvjijnrrq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gogol.net.cn/gtadbfmswe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinyuanbaomall.cn/gtfzlrghdt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nwbrower.top/gtkbtnoxec.html

[J09] 时区处理
来源：http://hz.nanxuanxn.top/gtxfpaylnb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.smart0.xyz/gtmnogdhaa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuetiantiany.cn/gtszgvssir.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gtyxslarpl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtqjejxpqh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fengsongda.top/gtgeymjshw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.smart0.xyz/gtpgvnamyb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxuanxn.top/gtagptzqyg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jlsjyb.cn/gtzhccltph.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenjidiqi.icu/gtnyvwhvil.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.birdmap.top/gtqfsxtmhj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtylftmozc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yongpay.top/gtravyjzot.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.9152youxi.cn/gtdjcirfqi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.iojbl.cn/gtgovgybtq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.bjfxy.top/gthcoujgfx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nanxinkj.top/gtxkdouxhp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daxiang520.top/gtzafjmrxx.html

================================================================================
来源：http://hz.316326.xyz/gtprgdfoty.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtcjqkbknt.html

================================================================================
来源：http://hz.iojbl.cn/gtskncsary.html

[K01] 对象转 JSON 字符串
来源：http://hz.aizwys.cn/gtqilateho.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtpqggeesu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtefdtmzsm.html

JS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtptlgfgft.html

TS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gthzngvlbq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhoulong.xyz/gtdfalovjk.html

Go:   json.Marshal(obj)
来源：http://hz.yanxiufei.cn/gtygrhouvl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.svipenyu.cn/gtrawgyyat.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtotnrabfo.html

[K02] JSON 字符串转对象
来源：http://hz.andypj.xyz/gtnbvejhxr.html

Py:   json.loads(s)
来源：http://hz.jlsjyb.cn/gtwydzgxpw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258888.top/gtsdldgfte.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtgngdaczp.html

TS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtkdejopqi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shzxlz.cn/gtwnffitdj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtknkouksz.html

Ruby: JSON.parse(s)
来源：http://hz.iojbl.cn/gtbxzyladd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gtuespyccc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuxming.cn/gtmttnxgio.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtpeymqtyf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtrojotkor.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtqjogrjmi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtjhpswovz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnxiangtu.top/gthdaoxklm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jlsjyb.cn/gtxmiupbit.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yvedp.cn/gtssgvitwx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zdqjudy.top/gtgisxuboy.html

[K04] 读取 JSON 文件
来源：http://hz.birdmap.top/gtufpjksak.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aibaodan.cn/gtjcimgmyy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fzhhl.top/gtnasvcpro.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtplvpctrq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtnjwqmfpr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.svipenyu.cn/gtcjcaffgj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtypxnlidh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangtech.top/gtqfvxdtkw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtqqvcffha.html

[K05] 深拷贝对象
来源：http://hz.redwolf501.top/gtpebbabhu.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigfzy.top/gtyvlywfrn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.bjfxy.top/gtijjvundi.html

JS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtmlvrlvtx.html

TS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtnmqpguod.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gtduwaachk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.redwolf501.top/gthtxujytz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.vqdsnc.cn/gtsiblmmok.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.feifeiyinyue.top/gtwmlqrjnm.html

[K06] 解析 URL 查询串
来源：http://hz.yongpay.top/gtmtoqnupr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gotoacloud.top/gtoadgzkan.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gtgwayhjbj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtegdabymj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtorvuqqsy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yuanzhike.top/gtcgjzpxth.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hfpthk.cn/gtrrlverjj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtchexzwri.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guannengcc.top/gtikdjmzdk.html

[K07] 进制转换
来源：http://hz.shzxlz.cn/gtdfsnsfqn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hammf.cn/gtgbrwdfec.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gtzbwmquto.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtafxwwrsg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtilwfexfc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtvmobgmrs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuanzhike.top/gtafcmxcbe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tian-w.cn/gtkhkmbkgc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gzhubu.top/gttyjxyobd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yangfankeji.com/gtzerkeumd.html

Py:   pickle.dumps(obj)
来源：http://hz.daxiang520.top/gtrlsxccyt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gaohongyu789.top/gtfogwlmzx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtysqrmrtl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtdeiegrsk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cucudq.cn/gtdxbuqfpc.html

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtgubiwzoj.html

Ruby: Marshal.dump(obj)
来源：http://hz.zdqjudy.top/gtgvdexhnv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cdnleiting.top/gtvwvmqhhs.html

================================================================================
来源：http://hz.jiagoushi.top/gtnijhlbcw.html

L. 网络请求
来源：http://hz.xuetiantiany.cn/gtpevgsper.html

================================================================================
来源：http://hz.aizwys.cn/gtixoljiqc.html

[L01] 发送 GET 请求
来源：http://hz.yj20258.top/gtxyabpumz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zdqjudy.top/gtmllbxzjo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhiwuduotai.top/gtgljowcgo.html

JS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtbnhsvjox.html

TS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gtzfarnkog.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenzaomai.com/gtdhsfnqss.html

Go:   resp, err := http.Get(url)
来源：http://hz.redwolf501.top/gtomsuchnt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhongyouzk.top/gtgjfmqwdf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinyuanbaomall.cn/gttejzifag.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gtftffsqyo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.birdmap.top/gtsvienawm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gtmowwfsqz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gtecgqsrzf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtgtmagzct.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangkeji.top/gtvgrmxwlz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gzhubu.top/gtdtjjckij.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hongshengwenyu.top/gtvpkeanmw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yuxming.cn/gtollymibe.html

[L03] 设置自定义请求头
来源：http://hz.pycfn.com/gtgosdzaea.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtxhprrgyj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtpiluxnci.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtwhedqlyp.html


<!-- 参考信息 -->