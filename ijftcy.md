代发 wailian999

Py:   value = d.get("k") or default
来源：http://hz.yanxiufei.cn/gtokwohgog.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zycfv.cn/gtevkpzqyk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtutwhftkh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.bjfxy.top/gtyogpaxpv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sweek.top/gtpzkixpwl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangtech.top/gtigfaxmqq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hywenlv.cn/gtxuvxhgot.html

C#:   obj?.A?.B ?? default
来源：http://hz.sysykeji.top/gtccvjmwji.html

[H07] 断言
来源：http://hz.daria6918.cn/gtmkqoxqfk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yanxiufei.cn/gtjuwftggq.html

PHP:  assert($x > 0);
来源：http://hz.jlsjyb.cn/gttazgmsaw.html

JS:   console.assert(x > 0);
来源：http://hz.jlsjyb.cn/gthtelyhqv.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtnpefsprq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pycfn.com/gtbeekoapw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangshuangyany.cn/gtehmhexry.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jianghu66.top/gtoreqjizc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gtxwbxwiit.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinghuilouyu.cn/gtfxxzgqmw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xziqi.cn/gtcyjayrfm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtcbdivcvj.html

JS:   e.message;  e.stack
来源：http://hz.birdmap.top/gthguiacae.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shangyingyoupin.top/gtpjvxjwoh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.svipenyu.cn/gtjsbcwrui.html

Go:   err.Error()
来源：http://hz.tanke756.top/gtllvjdxln.html

Ruby: e.message;  e.backtrace
来源：http://hz.guannengcc.top/gtikghitli.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xylfe.cn/gtmfdwfnyn.html

[H09] 带错误码的异常
来源：http://hz.pycfn.com/gtfaolpxew.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jyoumei.cn/gtzzujsctj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.aibaodan.cn/gtdswhlors.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtgrsceneo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tanke756.top/gteayspafv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cdnleiting.top/gtgkuvfbro.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nwbrower.top/gtpzrvchha.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cheryme.top/gtbjnjcejs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daxiang520.top/gtmgvizcso.html

[H10] 资源自动释放
来源：http://hz.zhijiandao.cn/gtwdxyhcvw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.fzhhl.top/gtryivzsbe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gttdumbpse.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtbhmnzodt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtufokpibo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxuanxn.top/gtcvsjvflp.html

Go:   defer f.Close()
来源：http://hz.yanxiufei.cn/gtdcetgenv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sweek.top/gtoudepzwy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuanzx.com/gttjohfxyf.html

================================================================================
来源：http://hz.cheryme.top/gtsjprxcvz.html

I. 正则表达式
来源：http://hz.aibaodan.cn/gtaqnrchrn.html

================================================================================
来源：http://hz.tian-w.cn/gtucnclrqp.html

[I01] 判断是否匹配
来源：http://hz.gzhubu.top/gtuzwclnwr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guowangkeji.top/gtammhiahw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yangfankeji.com/gthlttogmy.html

JS:   /\d+/.test(s)
来源：http://hz.hammf.cn/gtofmzrehg.html

TS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtzjaffhol.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jiagoushi.top/gttuqgucqq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hammf.cn/gtpjkeahei.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gtuytbwwps.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gtikxfgqqs.html

[I02] 提取所有匹配
来源：http://hz.zhengqikj.top/gtjavzlpfz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuanzx.com/gtzkgzmaun.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydzc1.top/gtbkcnnsew.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhongyouzk.top/gtwsvgefep.html

TS:   s.match(/\d+/g)
来源：http://hz.hnxiangtu.top/gtljvfravw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.c1oappe.top/gtnnzephue.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gtkaiznyjs.html

Ruby: s.scan(/\d+/)
来源：http://hz.vqdsnc.cn/gtnazxvkdi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtncfcxbyq.html

[I03] 提取捕获分组
来源：http://hz.aizwys.cn/gtpgagmflp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nwbrower.top/gtnpdijnjv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinyuanbaomall.cn/gtwblmyqdn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hfpthk.cn/gtvwwrthnd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shangyingyoupin.top/gtchyfczbs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xziqi.cn/gtjwijuezt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.9152youxi.cn/gtumwgmjdo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenlongwang.top/gtfccsqubb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhaomingkeji.xyz/gtejujkwrp.html

[I04] 正则替换
来源：http://hz.wangdashe.top/gtmdrfqkqf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.52xcode.cn/gtfgouohlb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.smart0.xyz/gtmndzowyu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtwnyoaiav.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtyyugsiqv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hfpthk.cn/gtpuxfemac.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tian-w.cn/gttdbvdvze.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tanke756.top/gtzhxzesjz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sysykeji.top/gtmqercemz.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtnobyyxvx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jiagoushi.top/gtwmpjrbyv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenjidiqi.icu/gtjfkfhhcg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtbemwnxju.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinghuilouyu.cn/gtbjvclfrs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zycfv.cn/gtxxsnicjd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj20258.top/gtmztvyuye.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtyjrjdtqz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangdashe.top/gtrbjzkaiw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.haohaochexian.top/gtesyjybiz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtcujcngyn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hfpthk.cn/gtljhdyjpy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtaftdyuey.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtcvifyhua.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.birdmap.top/gtcuxxkvoo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtbaxfctaq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cdnleiting.top/gtanzbgrfi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtarqfdpbe.html

[I07] 忽略大小写与多行模式
来源：http://hz.guannengcc.top/gtiybprlyy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hfpthk.cn/gtmcgqzzmo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gthwtjyxno.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gotoacloud.top/gtxvnvfick.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gtbwagfwrh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.smart0.xyz/gtaxdicnlh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.redwolf501.top/gtircddrrz.html

Ruby: s.scan(/error/i)
来源：http://hz.redwolf501.top/gtytimfqse.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.0kj1m.cn/gtnqpizxsh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.havefunace.top/gthzhyaguc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.0kj1m.cn/gtwanhbsrt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gzhubu.top/gtttexyevc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtrynksxic.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtuthgqcgh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtjuwkbdcq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtqcsnbaco.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinghuilouyu.cn/gtblyaldvk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtdvaajcvh.html

================================================================================
来源：http://hz.haohaochexian.top/gtngbmstcj.html

J. 日期与时间
来源：http://hz.9152youxi.cn/gtlgtlmwfq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkynncfcv.html

[J01] 获取当前时间
来源：http://hz.yvedp.cn/gtlkvgjcjt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtwnvhafzb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtqmjnqjfa.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtdaifzzex.html

TS:   new Date();  Date.now()
来源：http://hz.jiagoushi.top/gtajzbbazf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gaohongyu789.top/gtbksdpbfc.html

Go:   time.Now()
来源：http://hz.tian-w.cn/gtbzxlfmuo.html

Ruby: Time.now
来源：http://hz.zhijiandao.cn/gtzijulylr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ehwqpu.com/gtegisojbn.html

[J02] 格式化输出
来源：http://hz.jianghu66.top/gtuzjpcqso.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hysaishi.cn/gtgjdhvblz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtawrepboh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yanxiufei.cn/gtlrnayyjn.html

TS:   d.toISOString()
来源：http://hz.daxiang520.top/gtzrznpvdc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.0kj1m.cn/gthutexdmv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtmbfnbqsb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtxlnfwdkt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xziqi.cn/gtzzflbnpr.html

[J03] 字符串解析为日期
来源：http://hz.xziqi.cn/gtvlfqgzyt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guannengcc.top/gtkpbdwybz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.birdmap.top/gttfjvmauw.html

JS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtizofbcxn.html

TS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtclrmioxe.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258.top/gtsnnnxzhn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtfspwlnoy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtdtdawjqs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangkeji.top/gtbpohkpnb.html

[J04] 时间戳与日期互转
来源：http://hz.haohaochexian.top/gtozobvgak.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pycfn.com/gtjidggcqf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258.top/gtrvhkzino.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gteakuhmmb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guannengcc.top/gtfrcglerp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.redwolf501.top/gtgzlwmqjn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258.top/gtlbpnxsvq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhaomingkeji.xyz/gtvztlllua.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtzeqwoefx.html

[J05] 时间加减（加 7 天）
来源：http://hz.gzhubu.top/gtqanvqahw.html

Py:   now + timedelta(days=7)
来源：http://hz.meibo888.top/gtszrymtqu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xziqi.cn/gtezkgowzh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtrrtcyxrv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ybcxt.top/gtbdnbluuv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aizwys.cn/gtujcifpbi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxinkj.top/gtcrpmtsro.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gtparackbg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jyoumei.cn/gtyhebjvqr.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtsnflggxj.html

Py:   (end - start).total_seconds()
来源：http://hz.ybcxt.top/gtcqbfeocw.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gtgefyjkbg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangdashe.top/gtpxrqiyho.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258.top/gtasnsimey.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.mhx1999.top/gtgypsuxzx.html

Go:   end.Sub(start).Hours()
来源：http://hz.hysaishi.cn/gtolzunujs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sysykeji.top/gtygkxaxdy.html

C#:   (end - start).TotalSeconds
来源：http://hz.jlsjyb.cn/gtivbwnlxv.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtpwovmuyf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtthgxbdma.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.feifeiyinyue.top/gtehbmgdig.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhixingplan.top/gtkvtuqymh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtonxhqlln.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yuxming.cn/gtvbktvqik.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tian-w.cn/gtgwxvfgsx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtoesplvmq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtmpjxmwyu.html

[J08] 提取年月日与星期
来源：http://hz.316326.xyz/gtnwgvsxhx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daxiang520.top/gtwstghnhm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhijiandao.cn/gtycuzoelg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hammf.cn/gtvafbhzcs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xziqi.cn/gtephjvyhc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gtxkliqsht.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtbhkkweyk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigufen.top/gtyozrswjw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.wangshuangyany.cn/gtqnvjxjks.html

[J09] 时区处理
来源：http://hz.nanxuanxn.top/gtrvbvgona.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuanzx.com/gthpltowha.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tian-w.cn/gtsxpimuuj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtkkxppxjv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtqadfkcdj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shanyushiyangtech.top/gttqtjchjo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pengpengdd.cyou/gtgaeeoxpw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yangfankeji.com/gtaszmvjgj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sxryk.cn/gtdoolfpoc.html

[J10] 取今天 / 本月第一天
来源：http://hz.xinyue.icu/gtsxmlodsh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yanxiufei.cn/gtypypqfnt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtakojfqiu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fengsongda.top/gtmffltbdj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dianchejie.cn/gtakhlgpgp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangtech.top/gtsrysmlks.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gthpklzxdb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.c1oappe.top/gtnqwmjzyy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258.top/gtwzexlrle.html

================================================================================
来源：http://hz.hywenlv.cn/gtimbkxakz.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtrcsvnoae.html

================================================================================
来源：http://hz.ydjk.org.cn/gtosnkfncd.html

[K01] 对象转 JSON 字符串
来源：http://hz.yanxiufei.cn/gtiycrahtk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gteayqfwzb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.guannengcc.top/gtutvhlwlb.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtlxfvyljj.html

TS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gthbamosvg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sufxvd.cn/gtbxthhtom.html

Go:   json.Marshal(obj)
来源：http://hz.jyoumei.cn/gtvdzvawwr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtpcjeszwn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yonumen.top/gtdxgvciaf.html

[K02] JSON 字符串转对象
来源：http://hz.xinyue.icu/gtdpnxpjxw.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtxsnuyxlt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtxjgxujay.html

JS:   JSON.parse(s)
来源：http://hz.hysaishi.cn/gtdsbdqhee.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtezrpckmw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtxrywapey.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtrtsieanx.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtwtfhyiqw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuxming.cn/gtricdmdbi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daxiang520.top/gtebqlvhgr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtllqtllyd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gteojvqrqp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtrkqdqbyh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtzhmspwlb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shangyingyoupin.top/gtcsoajoui.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tian-w.cn/gtkvjnjpnf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.feifeiyinyue.top/gtvywoyrug.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daxiang520.top/gttdpcspxl.html

[K04] 读取 JSON 文件
来源：http://hz.yongpay.top/gtrzqvczel.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtuqdcpxaw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigufen.top/gtilliiwef.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtfwyvprrl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtlqlubmuh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hongshengwenyu.top/gtbnhuskxm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtnagarqlg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pycfn.com/gtnbhuibym.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hywenlv.cn/gtlfefyepf.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gtqjrothrk.html

Py:   copy.deepcopy(obj)
来源：http://hz.gaohongyu789.top/gtqpuhpqgh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.mhx1999.top/gtbhsdaisu.html

JS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtsqnxhxpb.html

TS:   structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtziuzqokm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xziqi.cn/gtasyhmovd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gtyobvagtp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jyoumei.cn/gttqbeynhr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pengpengdd.cyou/gtdktzhdfi.html

[K06] 解析 URL 查询串
来源：http://hz.yj20258888.top/gtcmqqfofc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shzxlz.cn/gtkjccgrjs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zycfv.cn/gtlysbhuun.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtehtxvcnj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtobagnfwh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jlsjyb.cn/gtulwezhim.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.pengpengdd.cyou/gtlxvcfszk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gtpcgyscuy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jianghu66.top/gtrlapskxx.html

[K07] 进制转换
来源：http://hz.xinyue.icu/gtbazrqhzg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuanzhike.top/gtzejruqjx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenzaomai.com/gteqadeiem.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtofmvpdde.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtgtyeihfv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj202588.top/gtldjllmnk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuxming.cn/gthfahwhfv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dianchejie.cn/gtyrsizpzk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.birdmap.top/gtrhhzarcv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xylfe.cn/gtkqgzuwed.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtcilwekni.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.kuanghao11.cn/gtnqmeqzjx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtphytrbnx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtpmlokgrc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.316326.xyz/gthovvjhfi.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtkjiaejmd.html

Ruby: Marshal.dump(obj)
来源：http://hz.yongpay.top/gtnidjfpte.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fzhhl.top/gtpbyihaln.html

================================================================================
来源：http://hz.quarkkingdee.top/gtzmzblwhs.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtiqcfvhwu.html

================================================================================
来源：http://hz.zdqjudy.top/gtczqbudou.html

[L01] 发送 GET 请求
来源：http://hz.jyoumei.cn/gtfxjjdskq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xuetiantiany.cn/gtvlbenwmy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ivvv.top/gtfriiplrp.html

JS:   await fetch(url)
来源：http://hz.gzhubu.top/gtnmtrjsur.html

TS:   await fetch(url)
来源：http://hz.ivvv.top/gtmcivdopi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cashguo.top/gtmvmpzpix.html

Go:   resp, err := http.Get(url)
来源：http://hz.ehwqpu.com/gtwzyjqwdq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xinyue.icu/gtdtgbjdkq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtnuvootdp.html

[L02] 发送 POST JSON
来源：http://hz.zhongyouzk.top/gttcgkaqys.html


<!-- 参考信息 -->