代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.sysykeji.top/gtetlxiwzn.html

[H08] 获取错误信息与堆栈
来源：http://hz.ywan-chungtsiang.top/gtkarfrsqv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cdnleiting.top/gtmmcanuxr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cucudq.cn/gtrsgvmtvv.html

JS:   e.message;  e.stack
来源：http://hz.wangshuangyany.cn/gtbqrflfoc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258888.top/gthnwkfdvj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daria6918.cn/gtqldyzhqt.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtxwliizef.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangshuangyany.cn/gttponkmhg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangtech.top/gtgxstremk.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gttilhzdzp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.quarkkingdee.top/gtseyfdllm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenjidiqi.icu/gteublyvxz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yvedp.cn/gtspcczgdg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daria6918.cn/gtjqzlknaw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhoulong.xyz/gtqzleldkp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shuidangran.top/gtqofyfprf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtdkmrjpux.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dashuyun.cn/gthfjszwir.html

[H10] 资源自动释放
来源：http://hz.zycfv.cn/gtghdrbyvz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guannengcc.top/gtgynzwcgq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jianghu66.top/gtgesyhvrp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtgbmfjvie.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gttspzvqbf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnxiangtu.top/gttmctksml.html

Go:   defer f.Close()
来源：http://hz.yongpay.top/gtdlqjjoty.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenzaomai.com/gtdpajamys.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ywan-chungtsiang.top/gthlgdmkqx.html

================================================================================
来源：http://hz.zhengqikj.top/gtvnjyuswb.html

I. 正则表达式
来源：http://hz.dashuyun.cn/gtmsdicmlh.html

================================================================================
来源：http://hz.jinqigfzy.top/gtrcgvskao.html

[I01] 判断是否匹配
来源：http://hz.yueranfly.top/gtbkjfvnqi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtikwxsdju.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.snrcjt.cn/gtzcrmkcpc.html

JS:   /\d+/.test(s)
来源：http://hz.dianchejie.cn/gtlctevtsf.html

TS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtlnhfplpf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hywenlv.cn/gtjvttyvne.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258.top/gtxrwejniv.html

Ruby: s.match?(/\d+/)
来源：http://hz.sweek.top/gtgznlzrbw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuanzhike.top/gtrhqxytoq.html

[I02] 提取所有匹配
来源：http://hz.nanxinkj.top/gttrcopsmu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gtlrwjtnsi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.c1oappe.top/gtzarjmhhd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zycfv.cn/gtnfnqrtec.html

TS:   s.match(/\d+/g)
来源：http://hz.yangfankeji.com/gtoksfpqah.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.0kj1m.cn/gtvgtoaqqg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gtxgojhtio.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuetiantiany.cn/gtcgjzuhin.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.havefunace.top/gtxqtaaoiz.html

[I03] 提取捕获分组
来源：http://hz.sweek.top/gtmlouggio.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gtyyicahom.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtbwbbqqbm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zdqjudy.top/gtgdzbfmsq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gttuhojlsa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.vqdsnc.cn/gtqbjjxvbj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yangfankeji.com/gtikihfkzv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sweek.top/gtygzexgrs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgfzy.top/gtzyetzhpi.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtcibsqjpz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuanzhike.top/gthdscetug.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daria6918.cn/gtkwubsimv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtojsmxwqp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtquncsnhs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.316326.xyz/gtpvoenseq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ppjwa.cn/gtwutipnkk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gtqhgzaaft.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtbnfhbslw.html

[I05] 按正则拆分
来源：http://hz.jinqigfzy.top/gtrshprbxw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nwbrower.top/gtftaipojc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxinkj.top/gtteivfuli.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtobrrfyrf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtsugrsnwf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.wangdashe.top/gtppqmgwaq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangdashe.top/gtewgwiwfk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtrhzikpxv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tianlin.xyz/gtfcyxmkyw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xinyue.icu/gtmzsbwcvw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtnnalngsc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.kuanghao11.cn/gtsekdcfyo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtxuqfqclb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gteftnzttv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258888.top/gtgtjyvmln.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yanxiufei.cn/gtfijtfspn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hammf.cn/gtuwnradjx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtppfkrxuz.html

[I07] 忽略大小写与多行模式
来源：http://hz.guannengcc.top/gtcaixljjj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yanxiufei.cn/gtkhlpvntc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.haohaochexian.top/gtrevsswux.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhongyouzk.top/gtxwlwajvl.html

TS:   /error/gim
来源：http://hz.smart0.xyz/gtnvhwfzxm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhaomingkeji.xyz/gtnsxijrcq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuanzhike.top/gthpqbwvsf.html

Ruby: s.scan(/error/i)
来源：http://hz.ywan-chungtsiang.top/gtrujdzzmx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.iojbl.cn/gtdriwarhl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhaomingkeji.xyz/gtwzlpqafa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj202588.top/gtpihzzgff.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.havefunace.top/gtawioqvyi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtyyivopgh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtursiwgcs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtmmapmjld.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtowmjxdxq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtxvmopszj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtsgxnajce.html

================================================================================
来源：http://hz.yanxiufei.cn/gtjxgeobqq.html

J. 日期与时间
来源：http://hz.smart0.xyz/gtqigtsfjr.html

================================================================================
来源：http://hz.yangfankeji.com/gtjjzjwovl.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtnplkrupf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxinkj.top/gtmltrvetx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtxzevmiyv.html

JS:   new Date();  Date.now()
来源：http://hz.52xcode.cn/gtmpotrlgp.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtwvrkixmx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ppjwa.cn/gtktsmxxqh.html

Go:   time.Now()
来源：http://hz.zhengqikj.top/gthyxqbbuk.html

Ruby: Time.now
来源：http://hz.pycfn.com/gtfmmsdyma.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xingfuxueyuan.xyz/gttzabavaq.html

[J02] 格式化输出
来源：http://hz.iojbl.cn/gtytgczqur.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtclzdqdsl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gthsqvzuru.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sxryk.cn/gtzxnapzwc.html

TS:   d.toISOString()
来源：http://hz.fengsongda.top/gtsocbcvie.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daxiang520.top/gtzclvhxqk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtncxkvlcy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtfljsldyx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangshuangyany.cn/gtktwkzxfq.html

[J03] 字符串解析为日期
来源：http://hz.zhaomingkeji.xyz/gthywvikxn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xylfe.cn/gtlxdklydi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.snrcjt.cn/gtviragviy.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtbdkllqoh.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtuxdzsdox.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtnjguqlrz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ydzc1.top/gtwpjhzfse.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtpyigtnjk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gthmzarxeh.html

[J04] 时间戳与日期互转
来源：http://hz.zhongyouzk.top/gtonajneor.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydzc1.top/gtgxrqligt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ybcxt.top/gttfqvktty.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shanyushiyangkeji.top/gttitgxysj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhixingplan.top/gtwvbjogof.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.meibo888.top/gtjogabuvt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jlsjyb.cn/gtehuhenqf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hysaishi.cn/gtdafnmise.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hysaishi.cn/gtyekcefjg.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnqzz.top/gtdgkgjwdt.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtjzbbwjsu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daxiang520.top/gtzketgnjc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtuagynyyw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gteichkyrj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yangfankeji.com/gtwolvemax.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hfpthk.cn/gttsodltbd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxinkj.top/gtnbyojmen.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtkpvtsilp.html

[J06] 计算两时间之差
来源：http://hz.ywan-chungtsiang.top/gtwzetwpwg.html

Py:   (end - start).total_seconds()
来源：http://hz.zhaomingkeji.xyz/gtspfwetcj.html

PHP:  $end->diff($start)->days;
来源：http://hz.redwolf501.top/gtzkfzyymv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtnpoqpnhn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xingfuxueyuan.xyz/gtghmcceil.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhaomingkeji.xyz/gtnhvgdfqm.html

Go:   end.Sub(start).Hours()
来源：http://hz.cashguo.top/gtvcizfowc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gtkctufubp.html

C#:   (end - start).TotalSeconds
来源：http://hz.gaohongyu789.top/gtwnbnqhtd.html

[J07] 比较两个日期
来源：http://hz.shuidangran.top/gtflbhdhjz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtbpucnnas.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.svipenyu.cn/gtteilcuvd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtmaervsky.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtlaxfloht.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnxiangtu.top/gtcpxeyrfs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yangfankeji.com/gtqqtebihf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtkpjeamal.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtmeyrdxks.html

[J08] 提取年月日与星期
来源：http://hz.yvedp.cn/gttyjaspna.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gotoacloud.top/gtwwmrdyhq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hongshengwenyu.top/gtohluunvj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gtndeaiuvl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.havefunace.top/gtdnyeaqyj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.iojbl.cn/gtoobjvuke.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dashuyun.cn/gtorbcxpdb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gtytutaset.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtbdqxgpkx.html

[J09] 时区处理
来源：http://hz.jiagoushi.top/gtoxqsyvzn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenzaomai.com/gtnrnzwasf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgfzy.top/gtscdoqgqm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtdzrdxynp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtjuldwsiv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zdqjudy.top/gtntziklns.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.9152youxi.cn/gtqqzhpsxl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.wangshuangyany.cn/gtpinofrkd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aibaodan.cn/gtyafdavei.html

[J10] 取今天 / 本月第一天
来源：http://hz.yangfankeji.com/gtwfnyemtm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ehwqpu.com/gtkorbqlvp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhijiandao.cn/gtcpwwillx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gtqibjgwmp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shanyushiyangkeji.top/gtdnrrkgrc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yongpay.top/gtrjkmkinq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangdashe.top/gtjdeexgnq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ywan-chungtsiang.top/gtjobxvndq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.svipenyu.cn/gtqbzashyc.html

================================================================================
来源：http://hz.chenlongwang.top/gttxopured.html

K. JSON 与序列化
来源：http://hz.cashguo.top/gtbbrgefxj.html

================================================================================
来源：http://hz.birdmap.top/gtdfdomdqz.html

[K01] 对象转 JSON 字符串
来源：http://hz.shangyingyoupin.top/gtfxbdpdhn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xziqi.cn/gtfoythisg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtkqcqjjgd.html

JS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtpfqciyui.html

TS:   JSON.stringify(obj)
来源：http://hz.cdnleiting.top/gtjbfkxfvy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangdashe.top/gtzyatlysd.html

Go:   json.Marshal(obj)
来源：http://hz.hfpthk.cn/gttkrrdpvy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gtpfilfpxn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtkffaxkpi.html

[K02] JSON 字符串转对象
来源：http://hz.havefunace.top/gtyxanjamk.html

Py:   json.loads(s)
来源：http://hz.shangyingyoupin.top/gtyiwqrctn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinyuanbaomall.cn/gtsfqwfwjk.html

JS:   JSON.parse(s)
来源：http://hz.jianghu66.top/gtsydubcji.html

TS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtufbrauri.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtofmqdmxr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtsvynemfd.html

Ruby: JSON.parse(s)
来源：http://hz.iojbl.cn/gtkdadanzh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jlsjyb.cn/gttsbnipyx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhoulong.xyz/gtadwaeacn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtouureygk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.svipenyu.cn/gteklcrzdy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenlongwang.top/gtslaooyrt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtadyicjtt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shangyingyoupin.top/gteiohlcaz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xingfuxueyuan.xyz/gttbsbflff.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gtfpojeunw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtmhejhtex.html

[K04] 读取 JSON 文件
来源：http://hz.cashguo.top/gtebisgxin.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtkiyqnhko.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.smart0.xyz/gtekoqlkkb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtvcmgvzuq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtyzuqrxdy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shzxlz.cn/gtkcvhdxpv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtxsumvejm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnxiangtu.top/gtkjpqspbg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.kuanghao11.cn/gthcykyksv.html

[K05] 深拷贝对象
来源：http://hz.dianchejie.cn/gtrohntbzm.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtszivdfwk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tanke756.top/gtxgzwtypi.html

JS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtcvmilxve.html

TS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtmqxrnsww.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gtduumpdfb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.52xcode.cn/gtutgqhyfs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuanzx.com/gtvtccutqz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xziqi.cn/gtlhsqyuse.html

[K06] 解析 URL 查询串
来源：http://hz.zycfv.cn/gtovtgvufv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.feifeiyinyue.top/gtulnqgctk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtqyjqofmo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtdfkhtyin.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtyhcuetxq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gtdubhiuna.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhengqikj.top/gtpuhxlnip.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenlongwang.top/gtllnrtugc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hfpthk.cn/gtokbjgfbe.html

[K07] 进制转换
来源：http://hz.svipenyu.cn/gtlojbxbnv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.0kj1m.cn/gtmphpinfz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtyqelsgje.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtqjmvyldx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtwriqzxbk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtyfmxrhhd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yonumen.top/gtkfiygses.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhongyouzk.top/gtruxmrqgc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenzaomai.com/gtzsngkqwy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ppjwa.cn/gtbmyvwodp.html

Py:   pickle.dumps(obj)
来源：http://hz.316326.xyz/gtflslobof.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhaomingkeji.xyz/gtehzfklak.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtztwxjzdk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.vqdsnc.cn/gtvligmlyd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtwmznpssm.html

Go:   encoding/gob
来源：http://hz.zdqjudy.top/gttivbnxxe.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenjidiqi.icu/gtqwrkgeju.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhengqikj.top/gttdeqzddn.html

================================================================================
来源：http://hz.c1oappe.top/gtweiqdqgb.html

L. 网络请求
来源：http://hz.cashguo.top/gtcrzpuoxq.html

================================================================================
来源：http://hz.hammf.cn/gtrsnccriz.html

[L01] 发送 GET 请求
来源：http://hz.yuxming.cn/gtiwrfxols.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tian-w.cn/gtvbfqlbnr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtyolzdlpb.html

JS:   await fetch(url)
来源：http://hz.hammf.cn/gtvepscqka.html

TS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtlzjaqcbl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cucudq.cn/gtsiajdjjo.html

Go:   resp, err := http.Get(url)
来源：http://hz.snrcjt.cn/gtdmaciaed.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aibaodan.cn/gtvjkuwqql.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtjlqixxhu.html

[L02] 发送 POST JSON
来源：http://hz.shzxlz.cn/gtcmefnjdt.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtdtemjsmq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hfpthk.cn/gtlahcfsjw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtcbssbjiv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtopfolgbu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.52xcode.cn/gtzcsbekky.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ybcxt.top/gtejgfzzoc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.316326.xyz/gtfjqtlrpk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxinkj.top/gtdlwmjehw.html

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gttvygbgod.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenjidiqi.icu/gtzphefpxa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cucudq.cn/gtonhvitue.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtbigzzofj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtrjcsjkjk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yueranfly.top/gtncvcskmx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nwbrower.top/gtrmganhex.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ybcxt.top/gtffszxsnj.html


<!-- 参考信息 -->