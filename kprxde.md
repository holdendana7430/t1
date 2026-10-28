代发 wailian999

[H07] 断言
来源：http://hz.yuanzhike.top/gtzqcjgsjp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.daria6918.cn/gtwioofeax.html

PHP:  assert($x > 0);
来源：http://hz.jinghuilouyu.cn/gtxpfrjrea.html

JS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gteczusmoi.html

TS:   console.assert(x > 0);
来源：http://hz.9152youxi.cn/gtdgxlkjay.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fzhhl.top/gtmsqxxbon.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tian-w.cn/gtatkmsjmt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.vqdsnc.cn/gtmrubicjt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gthxabrhjd.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuxming.cn/gteojnhppn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jiagoushi.top/gtpyinqsnm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.snrcjt.cn/gtuutnjkib.html

JS:   e.message;  e.stack
来源：http://hz.gotoacloud.top/gtgtxqwvzl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fzhhl.top/gtqxdjktpe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnxiangtu.top/gtsoiudeat.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gttnotviyj.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuanzx.com/gteyxulibg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shangyingyoupin.top/gtggcuvueu.html

[H09] 带错误码的异常
来源：http://hz.guannengcc.top/gtzivttgaj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.meibo888.top/gtombettmh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pycfn.com/gtmflujdus.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yonumen.top/gtlmziqtnc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhengqikj.top/gtihqwpsrh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuetiantiany.cn/gtatxpeaqw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.svipenyu.cn/gtgwzuomnj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.kuanghao11.cn/gtxazrsypn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuxming.cn/gtzasafsir.html

[H10] 资源自动释放
来源：http://hz.chenjidiqi.icu/gtowauwtva.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhaomingkeji.xyz/gtvmtelwla.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.mhx1999.top/gtmfrtvpij.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtozcrnsnf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtzzcptsyq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhoulong.xyz/gtzngkpzpe.html

Go:   defer f.Close()
来源：http://hz.aizwys.cn/gtskgylvji.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.vqdsnc.cn/gttuwhlhhi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cashguo.top/gthiubyono.html

================================================================================
来源：http://hz.zycfv.cn/gtcwuqvzhi.html

I. 正则表达式
来源：http://hz.xylfe.cn/gtwwmctqbh.html

================================================================================
来源：http://hz.yuanzhike.top/gtfksfrphm.html

[I01] 判断是否匹配
来源：http://hz.guowangkeji.top/gtiwfxlonx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtxxbvmhue.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhengqikj.top/gttfcvnkgu.html

JS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtfcrfnbpi.html

TS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtgsygssyz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xziqi.cn/gtnjnznhwz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tanke756.top/gtpijjvdbg.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigfzy.top/gtyfrkdruh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gtbhofbsjj.html

[I02] 提取所有匹配
来源：http://hz.yvedp.cn/gtnjrkarzs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yonumen.top/gtwdnhgihf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.snrcjt.cn/gtlsptomnm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zdqjudy.top/gtwgqxbpfx.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtdbaflyzq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gtsqeadyeq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jiagoushi.top/gtrxgodfwg.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtzhnqxhqd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hammf.cn/gttuntzknc.html

[I03] 提取捕获分组
来源：http://hz.dianchejie.cn/gtjjqiewna.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gtgjpzrfsy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fzhhl.top/gthtfyomus.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.vqdsnc.cn/gtyqxqgpsz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gtekspjvfj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuanzx.com/gtxvmncyyb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.birdmap.top/gtfatpljgv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinyuanbaomall.cn/gtvjkdqnvi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigufen.top/gtwiamgwzu.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtwpocunkp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hongshengwenyu.top/gtjguqimpn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangtech.top/gtwlnldjkf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gtevxyyglv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtizsaayhy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangdashe.top/gtqoojnfez.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cashguo.top/gthqvsewvl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gteucbccmh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gaohongyu789.top/gtyzfjeads.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtjouztkgn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sxryk.cn/gtuedyfgfz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yangfankeji.com/gtbrjszikk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtrvmxgmvi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtiiucekzq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hongshengwenyu.top/gtytuzbmai.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenjidiqi.icu/gtmoxslyuk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtosrzopci.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtcfzbaaqc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuanzhike.top/gtanfcqhrt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtxgrmxmtk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yanxiufei.cn/gtyrdroduf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtckmehahz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtjnajbrou.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gtkaqzhdsz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.birdmap.top/gttpqdnoxp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gaohongyu789.top/gtrjbyohsl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtftycmcqo.html

[I07] 忽略大小写与多行模式
来源：http://hz.ehwqpu.com/gtaewqetdy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhengqikj.top/gtmorrrwzv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xinyue.icu/gtjlcabdgt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydzc1.top/gtownupozh.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gthkzyzxlt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gotoacloud.top/gtnymmhbif.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.wangdashe.top/gtthyannka.html

Ruby: s.scan(/error/i)
来源：http://hz.yongpay.top/gtpfyiecpp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.iojbl.cn/gtmbcholiz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cashguo.top/gtksxxlrsj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gtknmltstj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gtcngyktmr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtqiaupjgb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gttsxjivfs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtfilacxyf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shangyingyoupin.top/gttoglstks.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sysykeji.top/gtuheprfkt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aibaodan.cn/gtmruzcryo.html

================================================================================
来源：http://hz.yuxming.cn/gthnymakql.html

J. 日期与时间
来源：http://hz.vqdsnc.cn/gttqjctloz.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfiiqlbdx.html

[J01] 获取当前时间
来源：http://hz.zhoulong.xyz/gtzawnagku.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.mhx1999.top/gtidijuuhc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtdyjuzgfx.html

JS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gtihimxugl.html

TS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gthbursojd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangkeji.top/gttojwmooe.html

Go:   time.Now()
来源：http://hz.pycfn.com/gtbdyfeqvz.html

Ruby: Time.now
来源：http://hz.kuanghao11.cn/gtjnusepeh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtxfgmixmz.html

[J02] 格式化输出
来源：http://hz.shanyushiyangkeji.top/gtfoylbeci.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtlaslvdet.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtgefoydom.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.meibo888.top/gtftqtpjoc.html

TS:   d.toISOString()
来源：http://hz.yj20258888.top/gtpnmtzjsu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gotoacloud.top/gtzghhuufw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigfzy.top/gtkaqjxfca.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtjnjjnowf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnqzz.top/gtmebqdpsy.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gtwkfibibx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xylfe.cn/gthvqncbpr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenlongwang.top/gtzlkwsrkm.html

JS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtqbxgpjgg.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtujsxulef.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtpoexgjdj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zycfv.cn/gtziaovdxz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtrlhsnqkh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shuidangran.top/gtcahybdbc.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigfzy.top/gtloomqsle.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgufenzy.top/gtsuwzyhdx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xinyue.icu/gtnhrcfoad.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.havefunace.top/gtocbsajlf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sxryk.cn/gtiuwfuyug.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gzhubu.top/gtczxeunoy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gtrzwafzbf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258.top/gtjrvdtpqt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gtgvwoxzaw.html

[J05] 时间加减（加 7 天）
来源：http://hz.gogol.net.cn/gtdvyorddt.html

Py:   now + timedelta(days=7)
来源：http://hz.fengsongda.top/gtrbnwdnwr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yueranfly.top/gtytotytyg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtyiehoxjg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtuiaajeoq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xinyue.icu/gtfrskxzwa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangshuangyany.cn/gtpdgkimmx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jyoumei.cn/gtzylofvid.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnxiangtu.top/gtjzkxanrr.html

[J06] 计算两时间之差
来源：http://hz.yj20258888.top/gtkqyikvpn.html

Py:   (end - start).total_seconds()
来源：http://hz.hysaishi.cn/gtcsavljsx.html

PHP:  $end->diff($start)->days;
来源：http://hz.yvedp.cn/gtwewamtky.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.feifeiyinyue.top/gtmrynzleo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtiixcnxtx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhongyouzk.top/gtoybthxfa.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangdashe.top/gtpkedyjfk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.bjfxy.top/gtudsxkvgr.html

C#:   (end - start).TotalSeconds
来源：http://hz.haohaochexian.top/gtwatqojmd.html

[J07] 比较两个日期
来源：http://hz.zhixingplan.top/gtatehsmlq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtcouyaprv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtoxkscsmu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.dianchejie.cn/gtzkctctdo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtlysquojx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtetjfgred.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtjjsldgly.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtxkzkvasr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtlevwvjtd.html

[J08] 提取年月日与星期
来源：http://hz.nwbrower.top/gtlsznobgm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dashuyun.cn/gtwpxfhbne.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangshuangyany.cn/gteidwfmww.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jiagoushi.top/gteyndonwq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtepcbrevm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gthhdexzol.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yonumen.top/gtmsjbpsqk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.meibo888.top/gtfhvqmjyz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtxyjfgblv.html

[J09] 时区处理
来源：http://hz.guowangkeji.top/gtoiokgldf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.pycfn.com/gtibdpqzng.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gogol.net.cn/gtxsjuscoj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtylszdmhf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtciwreogx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtmtfypney.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.vqdsnc.cn/gtqcvqpwrg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj202588.top/gtvevenigq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuetiantiany.cn/gtbabxguov.html

[J10] 取今天 / 本月第一天
来源：http://hz.gogol.net.cn/gtcvgvgiim.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gthnxrswex.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gogol.net.cn/gtgmxrdphx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dianchejie.cn/gtgqbaeunj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.haohaochexian.top/gtubwpzily.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxinkj.top/gtixvvrisk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtwwboxoxh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ppjwa.cn/gtghnkejoq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ybcxt.top/gtiembainq.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlmlfyfvg.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gtjxqvuevs.html

================================================================================
来源：http://hz.shuidangran.top/gttpokyfky.html

[K01] 对象转 JSON 字符串
来源：http://hz.ywan-chungtsiang.top/gtncxbiyfr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtqcxnprxh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtbmqpkndk.html

JS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtpfjrxtul.html

TS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gteygpaagt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangdashe.top/gttorcgbfc.html

Go:   json.Marshal(obj)
来源：http://hz.cqqwz.cn/gtqvlsigyb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhiwuduotai.top/gtxswphfkk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dianchejie.cn/gtilsvhdom.html

[K02] JSON 字符串转对象
来源：http://hz.shuidangran.top/gtoypkbhqi.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtwswsrdpz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.vqdsnc.cn/gtaqilytcg.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtaynwhrvl.html

TS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtdtjtnwab.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.guowangkeji.top/gtjrxpahdh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gtjtoondqh.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gthdmwigyh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenlongwang.top/gtwoptuegs.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hysaishi.cn/gtkiuviglz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtrxpiprqz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtczvpotwy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yangfankeji.com/gtsdmffwyg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtyqkqbqba.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tian-w.cn/gtemehvccg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xylfe.cn/gtposvtndz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinghuilouyu.cn/gthasaqqmi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.c1oappe.top/gtnmhavptn.html

[K04] 读取 JSON 文件
来源：http://hz.jlsjyb.cn/gtcfasxdre.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.svipenyu.cn/gthiupqlin.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tian-w.cn/gtbcuolcuc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtalejzttp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gtusdhtymf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.kuanghao11.cn/gtxbufwrtx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gtshtaooek.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yongpay.top/gtghwwjkra.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tanke756.top/gtrvchkmye.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gtqdfzyiri.html

Py:   copy.deepcopy(obj)
来源：http://hz.feifeiyinyue.top/gtstwvxbpg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhiwuduotai.top/gtwlfsbgpo.html

JS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gtphvssmou.html

TS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtnevscqsx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ppjwa.cn/gtkplnfkzl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shzxlz.cn/gthemkluht.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.quarkkingdee.top/gtbsmigagv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dashuyun.cn/gtcbqtmvni.html

[K06] 解析 URL 查询串
来源：http://hz.xziqi.cn/gtzssrhdli.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sweek.top/gtsafcusux.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tian-w.cn/gtbomigfgv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtiuwsuaaz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtohbvlofu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.52xcode.cn/gtahxncgkw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yonumen.top/gtvxalovil.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yueranfly.top/gtejgnfkjj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.9152youxi.cn/gtprwhcafx.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtfvlverct.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shzxlz.cn/gtaveidrcs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ybcxt.top/gtpvvczpnp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtomzluoge.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtgyhlqbjk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtisvbjfwn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtqscpvjzl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shzxlz.cn/gtidddcjme.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.snrcjt.cn/gtikropwtj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangtech.top/gtusymoczx.html

Py:   pickle.dumps(obj)
来源：http://hz.zhiwuduotai.top/gttfmwsqqm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cdnleiting.top/gtywvpccwp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtelpprwzv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtippipkce.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aizwys.cn/gtgohwchbz.html

Go:   encoding/gob
来源：http://hz.ivvv.top/gtokodftrv.html

Ruby: Marshal.dump(obj)
来源：http://hz.tian-w.cn/gtetffucsp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daria6918.cn/gtrolpltye.html

================================================================================
来源：http://hz.ppjwa.cn/gtferulngp.html

L. 网络请求
来源：http://hz.hnxiangtu.top/gttnivardq.html

================================================================================
来源：http://hz.yuxming.cn/gtyzkwctnq.html

[L01] 发送 GET 请求
来源：http://hz.yuanzhike.top/gtlhebqwbf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.birdmap.top/gtyfcfavyw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hammf.cn/gtqmhbxbbt.html

JS:   await fetch(url)
来源：http://hz.smart0.xyz/gtdqjogasa.html

TS:   await fetch(url)
来源：http://hz.mhx1999.top/gtcbgxwsfs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtnsrqjmiy.html

Go:   resp, err := http.Get(url)
来源：http://hz.hywenlv.cn/gttukbndae.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.redwolf501.top/gtahsioovi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhengqikj.top/gtqyqwkjui.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtuigajtzj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.feifeiyinyue.top/gtmnvtkned.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pycfn.com/gturwcptib.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtqdmwgbft.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtnjlckvqd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guowangkeji.top/gtqtitvpcu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guannengcc.top/gtnkybxxtg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.quarkkingdee.top/gtkwwnxyoz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sysykeji.top/gtyecumskg.html


<!-- 参考信息 -->