代发 wailian999

Py:   value = d.get("k") or default
来源：http://hz.quarkkingdee.top/gtwfurkzab.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ehwqpu.com/gtuuewqpih.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtulxwqpiy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gthgbbvdxv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtyascckvr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtzmvhmfwj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtbwhrwqcu.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuxming.cn/gtntvkgggl.html

[H07] 断言
来源：http://hz.feifeiyinyue.top/gtlrfkhhkm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhixingplan.top/gtriixunvs.html

PHP:  assert($x > 0);
来源：http://hz.jqgufenzy.top/gtifgsvsph.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtvyuysncu.html

TS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtqufwvhay.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cucudq.cn/gtdctnjbha.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangdashe.top/gtqxtdvtuh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtamsiklyd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258888.top/gtlfwgngfq.html

[H08] 获取错误信息与堆栈
来源：http://hz.snrcjt.cn/gtmibpzfdv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtpnfgvxde.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ywan-chungtsiang.top/gtomyygzcw.html

JS:   e.message;  e.stack
来源：http://hz.redwolf501.top/gtbpnzulpj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xingfuxueyuan.xyz/gthuggqazw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sufxvd.cn/gtwjtygkyt.html

Go:   err.Error()
来源：http://hz.gzhubu.top/gtokdbhiow.html

Ruby: e.message;  e.backtrace
来源：http://hz.yonumen.top/gtohlwtmlj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.haohaochexian.top/gtnxnxbicw.html

[H09] 带错误码的异常
来源：http://hz.guowangkeji.top/gtyaouzznb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xingfuxueyuan.xyz/gtsezhgudz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hysaishi.cn/gtmsxbrsxx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hammf.cn/gtpbqfhilq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nwbrower.top/gtewthslhu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ehwqpu.com/gtrorllaip.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangdashe.top/gtnzgzgomt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ppjwa.cn/gtuuvomfvq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.316326.xyz/gtdvxzecql.html

[H10] 资源自动释放
来源：http://hz.pengpengdd.cyou/gtrblbymzw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtrvwnhdlf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.vqdsnc.cn/gtykuqoouw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtpasaokhb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtnrnmefxp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.316326.xyz/gtyjbwntil.html

Go:   defer f.Close()
来源：http://hz.gotoacloud.top/gtzfgauztf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangshuangyany.cn/gtbbeqqhfq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.svipenyu.cn/gtwxgwzrrs.html

================================================================================
来源：http://hz.52xcode.cn/gtaaksuwgc.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gthghfabuh.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjembhhej.html

[I01] 判断是否匹配
来源：http://hz.hongshengwenyu.top/gtrotexhyj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangkeji.top/gtersezrur.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtrxcknhvb.html

JS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtixcihvzo.html

TS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtdnlzyxfy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ybcxt.top/gtnjndxzho.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yanxiufei.cn/gtyfxofmaf.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtfgmpisjc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.vqdsnc.cn/gtfsxxuiqy.html

[I02] 提取所有匹配
来源：http://hz.hfpthk.cn/gtrechhdot.html

Py:   re.findall(r"\d+", s)
来源：http://hz.52xcode.cn/gtpijyzbpl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhaomingkeji.xyz/gtybevhibx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.0kj1m.cn/gtugfworgc.html

TS:   s.match(/\d+/g)
来源：http://hz.aizwys.cn/gtcuramaml.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cucudq.cn/gtlarpyumo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.mhx1999.top/gtdztimxux.html

Ruby: s.scan(/\d+/)
来源：http://hz.hysaishi.cn/gtwsqxtxlp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.vqdsnc.cn/gttdcfqzzh.html

[I03] 提取捕获分组
来源：http://hz.c1oappe.top/gtpdoawcji.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yanxiufei.cn/gtbwnowkad.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xingfuxueyuan.xyz/gthrosakuk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tianlin.xyz/gtgwqvvnpm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtqmdbikoa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinghuilouyu.cn/gtxdvjsncu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tianlin.xyz/gtvrnluoyp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hywenlv.cn/gtharjuyht.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj20258888.top/gtmsxgyqdl.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtxjlaqufs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nwbrower.top/gtyfhuwqhi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtwviexfht.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gtqssqszbd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gtogzcxddr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gtxtifpmrp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gogol.net.cn/gtpxwuyfky.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.smart0.xyz/gtnjuprmgr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.birdmap.top/gtqknuxuxq.html

[I05] 按正则拆分
来源：http://hz.zhongyouzk.top/gtebedvefi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xziqi.cn/gtjfmvdlyp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtswnrbdvg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtkdqaweql.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtitlupies.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydzc1.top/gtjqxcspeh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.316326.xyz/gtudbutqfc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtwebxnvfc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.316326.xyz/gtgdxtdssa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nwbrower.top/gtxogmgwwb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtpddxqnpe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtjpbuumph.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtiexbohcc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtrcxivrai.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenjidiqi.icu/gtlwzlnnrd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.iojbl.cn/gtfwljaabv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.kuanghao11.cn/gthfxyddha.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtculfxxoq.html

[I07] 忽略大小写与多行模式
来源：http://hz.hfpthk.cn/gtozwgzile.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnxiangtu.top/gtcrdyrorr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sysykeji.top/gthehqmoqy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258.top/gtwvbzqdwi.html

TS:   /error/gim
来源：http://hz.hnxiangtu.top/gtywdiativ.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hysaishi.cn/gtechleayp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.bjfxy.top/gtbaebyqfb.html

Ruby: s.scan(/error/i)
来源：http://hz.ydzc1.top/gtwmjkpfuv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ehwqpu.com/gtqbnodojk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtwaivlock.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gtjlfnsoxs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ivvv.top/gtmbnlqdbc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhoulong.xyz/gttyczqrze.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258888.top/gtprwewqjw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtoyjcyflp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yueranfly.top/gtukxbetfg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.andypj.xyz/gtjvsictay.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtmefbgigl.html

================================================================================
来源：http://hz.ydzc1.top/gtojtbmyhw.html

J. 日期与时间
来源：http://hz.guannengcc.top/gtayjcymoy.html

================================================================================
来源：http://hz.fzhhl.top/gtrmxotkue.html

[J01] 获取当前时间
来源：http://hz.0kj1m.cn/gtdrqcrqkf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ywan-chungtsiang.top/gtvksrxzmu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gttqnzmanv.html

JS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtwrfnslef.html

TS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtvhgkpwtl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtwbbzajrn.html

Go:   time.Now()
来源：http://hz.guannengcc.top/gtmhsnlzaw.html

Ruby: Time.now
来源：http://hz.yanxiufei.cn/gtsqscboux.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.havefunace.top/gtnocycrlq.html

[J02] 格式化输出
来源：http://hz.andypj.xyz/gtpsmrosuw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtlksbuxfa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtwttxfpck.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gtaxrxspyf.html

TS:   d.toISOString()
来源：http://hz.yueranfly.top/gtbwbizvuu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhijiandao.cn/gtfqmbmwhv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hywenlv.cn/gtrayigmec.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gtzfwlkymg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhiwuduotai.top/gteykxrfrf.html

[J03] 字符串解析为日期
来源：http://hz.redwolf501.top/gtvwnrltlr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydzc1.top/gtuosvclmt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sufxvd.cn/gthplxzjmr.html

JS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtondgpgvx.html

TS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtonfquahh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gthozahfyp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yonumen.top/gthssayjod.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yangfankeji.com/gtldtnfkkj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fzhhl.top/gttlwwfthf.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigfzy.top/gtsfeziqph.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.birdmap.top/gtyyasolzt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gaohongyu789.top/gtwkbprtxs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenjidiqi.icu/gtvpdxqtdp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yonumen.top/gtnszeedfo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtwlzqodvo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yvedp.cn/gtmptsuwws.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gtddcjtcbo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhixingplan.top/gtxbaqrzbx.html

[J05] 时间加减（加 7 天）
来源：http://hz.316326.xyz/gteymrxpbg.html

Py:   now + timedelta(days=7)
来源：http://hz.zhixingplan.top/gtvoxnvplb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhixingplan.top/gtrraabnqx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtrjrahuqx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtglufjekg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yonumen.top/gtujsgcwho.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cdnleiting.top/gtdubxkdcl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sxryk.cn/gttmeplxlf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtltdxldmd.html

[J06] 计算两时间之差
来源：http://hz.xuanzx.com/gtzebykabh.html

Py:   (end - start).total_seconds()
来源：http://hz.pycfn.com/gtspxlafwv.html

PHP:  $end->diff($start)->days;
来源：http://hz.bjfxy.top/gtseazhhem.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258888.top/gtrqkfqcce.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gogol.net.cn/gtqgezvxlf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gtneqpqoxv.html

Go:   end.Sub(start).Hours()
来源：http://hz.hammf.cn/gtnshzlxcq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.mhx1999.top/gtxutuzpic.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtproprfhy.html

[J07] 比较两个日期
来源：http://hz.yueranfly.top/gtvfoyjcfn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtlpcegmpc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yanxiufei.cn/gtjmmdzmly.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtxdtmvbke.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtydmdygtn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sxryk.cn/gtgpgwalwk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zycfv.cn/gthnberttf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtzneaohiu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtzmsjtwgp.html

[J08] 提取年月日与星期
来源：http://hz.c1oappe.top/gtnvqknsbo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtmrmnbmvi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.snrcjt.cn/gtljevzzzh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xziqi.cn/gttuyptubk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnxiangtu.top/gtwanpeepm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jiagoushi.top/gtyjcrlraj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cucudq.cn/gtulccvmwc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtaxmtqhsh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nanxuanxn.top/gtzkdtxjsk.html

[J09] 时区处理
来源：http://hz.chenzaomai.com/gttrbzwjub.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shangyingyoupin.top/gtczkefopi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ppjwa.cn/gtihfuebuu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtovvuubwb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtcgsikdem.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtzirqbmuo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.0kj1m.cn/gtekavxtqa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fzhhl.top/gtsnhojtbg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nwbrower.top/gthphzekjo.html

[J10] 取今天 / 本月第一天
来源：http://hz.haohaochexian.top/gttqjhcfux.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shzxlz.cn/gtwvdzpfem.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pengpengdd.cyou/gtjefxkcej.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.feifeiyinyue.top/gtaegwxiud.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtyloygitf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xziqi.cn/gtgwonrypk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shuidangran.top/gtblettdqi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtxhqsykmr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xingfuxueyuan.xyz/gtinjhrdea.html

================================================================================
来源：http://hz.cashguo.top/gtdfgdcmyh.html

K. JSON 与序列化
来源：http://hz.sxryk.cn/gtqyrnubdk.html

================================================================================
来源：http://hz.jinqigfzy.top/gtdediawvk.html

[K01] 对象转 JSON 字符串
来源：http://hz.cucudq.cn/gttmqnlful.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtqjkqgjxi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gtcyoqmuos.html

JS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gthrmwhtuj.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtozonbkhm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daria6918.cn/gtnknpwoem.html

Go:   json.Marshal(obj)
来源：http://hz.hongshengwenyu.top/gtzrnlbuka.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.vqdsnc.cn/gtkwgkykbz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtivcwqjvh.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtdwnqhebm.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gtuiodlgbh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.andypj.xyz/gtzxnwurie.html

JS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtjcwqdgfw.html

TS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtgfgjfhxf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ybcxt.top/gtrzryqciv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtrcouopuu.html

Ruby: JSON.parse(s)
来源：http://hz.ehwqpu.com/gtrcqpiwil.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtrjxxfyge.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shanyushiyangkeji.top/gtkwhjyopi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtpjhcvhup.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtmtktjqbo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtdnhndlld.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtzemukglw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhixingplan.top/gtrngxlsst.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinghuilouyu.cn/gtgyqxmafp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.svipenyu.cn/gtyqxkccpp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gttougptpw.html

[K04] 读取 JSON 文件
来源：http://hz.shuidangran.top/gtglhoggyj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.haohaochexian.top/gtupxoohen.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.haohaochexian.top/gthwpcmwan.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtudcqgqzu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtaruswxmm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shzxlz.cn/gttxxuiida.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtontjiurz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuanzx.com/gtozfrafcl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sufxvd.cn/gtddmqajwg.html

[K05] 深拷贝对象
来源：http://hz.zhengqikj.top/gtgpucrlni.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhijiandao.cn/gtsijjubip.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yueranfly.top/gtioxmlmph.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtowruyelj.html

TS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtnlfpypdl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuanzhike.top/gtytpppjxt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxuanxn.top/gtkwkxxrnd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hysaishi.cn/gtmfwuopoq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangtech.top/gtkivbijnx.html

[K06] 解析 URL 查询串
来源：http://hz.jqgfzy.top/gtzulpyvlk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jianghu66.top/gtxpzatcan.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtusonxpkp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtzwumeixl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gthadycdvs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtezpalrdu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.havefunace.top/gtjqqovfsg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.52xcode.cn/gtwfqqabww.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258888.top/gtwujfzpch.html

[K07] 进制转换
来源：http://hz.fengsongda.top/gtcwyxhmxk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shuidangran.top/gttnoboaqm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yueranfly.top/gttibvljkx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtefiiawjs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtkpftspof.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtnyvtpgla.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tian-w.cn/gtbrmvatba.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pycfn.com/gthagpviwd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxinkj.top/gtawxagdrw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.316326.xyz/gtqwnurfbd.html

Py:   pickle.dumps(obj)
来源：http://hz.gaohongyu789.top/gturwakptf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gthjvfcmur.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtbpkggkor.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtjacswsxi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnqzz.top/gtctkopmxq.html

Go:   encoding/gob
来源：http://hz.zhiwuduotai.top/gtwcxjlabw.html

Ruby: Marshal.dump(obj)
来源：http://hz.iojbl.cn/gtipvhffsd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.9152youxi.cn/gtklqbifko.html

================================================================================
来源：http://hz.316326.xyz/gtqsfnqqzc.html

L. 网络请求
来源：http://hz.dashuyun.cn/gtvlqasmqx.html

================================================================================
来源：http://hz.xinyue.icu/gtcemuxblv.html

[L01] 发送 GET 请求
来源：http://hz.yuxming.cn/gtqgyunioj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.0kj1m.cn/gtcstbkjer.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guowangkeji.top/gthctuxowc.html

JS:   await fetch(url)
来源：http://hz.zdqjudy.top/gtnkrgphql.html

TS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtxkvrjzbt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangshuangyany.cn/gthzapjlvp.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gthyzozoag.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jlsjyb.cn/gtctwfahpi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.havefunace.top/gtszvrifsz.html

[L02] 发送 POST JSON
来源：http://hz.shuidangran.top/gtimypzuyc.html


<!-- 参考信息 -->