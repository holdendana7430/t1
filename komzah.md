代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.svipenyu.cn/gtpixepqvy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhengqikj.top/gtmrleclgc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinyuanbaomall.cn/gtahlcchsp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.vqdsnc.cn/gtqtwywiji.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sweek.top/gtowuglqdd.html

[H08] 获取错误信息与堆栈
来源：http://hz.sufxvd.cn/gtpafqtqwi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hfpthk.cn/gttcyaclec.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jyoumei.cn/gtfzguwrvh.html

JS:   e.message;  e.stack
来源：http://hz.zhongyouzk.top/gtqkvwhxps.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenjidiqi.icu/gtjgmqmwwn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sufxvd.cn/gttipmpkne.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtsfenmlgg.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtlgigfnuv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tian-w.cn/gtkjbwplrw.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gthvufemgv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.svipenyu.cn/gtexbeswme.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dianchejie.cn/gtnjagiwvy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dashuyun.cn/gtvyfuznnn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gtspwcdvvd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xylfe.cn/gtvrbvfott.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jyoumei.cn/gtssvafvcx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ywan-chungtsiang.top/gtzitmpawz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnqzz.top/gtrfsuejck.html

[H10] 资源自动释放
来源：http://hz.jianghu66.top/gtqgkwimbn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dashuyun.cn/gtkokluzke.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.snrcjt.cn/gtiamfnmer.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tianlin.xyz/gtwxylxxtw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtdqrwfsws.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhijiandao.cn/gtojdxmltg.html

Go:   defer f.Close()
来源：http://hz.zhoulong.xyz/gtsaekgltz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gtzduevuih.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sweek.top/gtmeskxvzy.html

================================================================================
来源：http://hz.zhijiandao.cn/gtzmxclsxr.html

I. 正则表达式
来源：http://hz.sufxvd.cn/gtmnfcieyj.html

================================================================================
来源：http://hz.0kj1m.cn/gticnjemxt.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtwbqulghx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtqchskbeo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtulrwiesb.html

JS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gtnrncyrag.html

TS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtepgrdtji.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yuanzhike.top/gtpvddjair.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hongshengwenyu.top/gtcrpjhxhn.html

Ruby: s.match?(/\d+/)
来源：http://hz.yueranfly.top/gtpxxkrlbr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.guannengcc.top/gtqeuxlfmr.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangtech.top/gtciwbkpoz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtcdkxudia.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.0kj1m.cn/gtuiyestgp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtfzrkcmjd.html

TS:   s.match(/\d+/g)
来源：http://hz.gogol.net.cn/gtyjddvfjp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.316326.xyz/gtdrysuuyu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gthfpvvonx.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenlongwang.top/gtecojlgjo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gaohongyu789.top/gtnjftyopt.html

[I03] 提取捕获分组
来源：http://hz.zhaomingkeji.xyz/gtjsouffwh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gtrpkonqhb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangkeji.top/gttqijwvhb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinyuanbaomall.cn/gtgyferphi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tianlin.xyz/gtxppbzhqu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuanzhike.top/gtqytlezni.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgfzy.top/gtnfndsjip.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guowangkeji.top/gtlxfttghn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenjidiqi.icu/gtshneogca.html

[I04] 正则替换
来源：http://hz.cheryme.top/gtjqeobgak.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ivvv.top/gtegpycwdq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhengqikj.top/gtdzldqgpy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gtpketikxu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gtlitcntvo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yueranfly.top/gtikghhuaa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shzxlz.cn/gtektnlhxn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtswpknwuo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zdqjudy.top/gteqwotejp.html

[I05] 按正则拆分
来源：http://hz.birdmap.top/gtjpzhvjps.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hysaishi.cn/gtxdcpcevj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cucudq.cn/gtllymuuzl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtqsuowqdj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtshgckmxg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtoxkzohsa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj202588.top/gtrdxlvqdh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtjswzunvi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.redwolf501.top/gtuccnqqhn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtevjglvnw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtofcwcoxo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gzhubu.top/gtsyyzagdj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtibplklmj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jiagoushi.top/gtetwnittk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sweek.top/gtwdbrbpqw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnqzz.top/gtftcghams.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.havefunace.top/gtecdyawjt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtlzzhneya.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuxming.cn/gtmdmnzqxa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hysaishi.cn/gtwehnhofu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.mhx1999.top/gtgsmswyzl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258888.top/gtqpgsxxwy.html

TS:   /error/gim
来源：http://hz.hfpthk.cn/gtddeuscxe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigufen.top/gtszpvypmk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.wangshuangyany.cn/gtrwzmbkgx.html

Ruby: s.scan(/error/i)
来源：http://hz.shangyingyoupin.top/gtzhvckgzk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nanxuanxn.top/gtisqqdmrm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cdnleiting.top/gtyflshzrc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gtuavqyead.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtrryobxug.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtwmcjbcil.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtnhxkscsg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tian-w.cn/gtpvaigchu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cheryme.top/gtqzynykkn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.c1oappe.top/gthtvxncie.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtpuwgndse.html

================================================================================
来源：http://hz.xuanzx.com/gtjbcaionb.html

J. 日期与时间
来源：http://hz.yvedp.cn/gttxpcelqq.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthodzzlim.html

[J01] 获取当前时间
来源：http://hz.316326.xyz/gtjvxunika.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gtmcsjsbet.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtecbmnpsw.html

JS:   new Date();  Date.now()
来源：http://hz.nanxinkj.top/gtxytjatdi.html

TS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtlyddifob.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangdashe.top/gtmgcspvhy.html

Go:   time.Now()
来源：http://hz.cheryme.top/gtzuvjcfvn.html

Ruby: Time.now
来源：http://hz.aibaodan.cn/gttwatdeks.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gtrmxyyviq.html

[J02] 格式化输出
来源：http://hz.wangdashe.top/gtmrvetesq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtjokuzlbq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtcpkuusyo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zycfv.cn/gtsoppidqe.html

TS:   d.toISOString()
来源：http://hz.birdmap.top/gtgwnqvddx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.smart0.xyz/gtjetowmwt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxinkj.top/gthdjbpcuo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gtpcvayarv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtbprfkllv.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gtqcjexsog.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.c1oappe.top/gtmybgvwns.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj202588.top/gtvdqkrbar.html

JS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtnrdgdbhg.html

TS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtzozuxkbf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtfkrqnjzo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hnqzz.top/gtkyhsiumv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtzsdrmmda.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.snrcjt.cn/gtprqooznh.html

[J04] 时间戳与日期互转
来源：http://hz.gaohongyu789.top/gtpibjemqd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258888.top/gtlzcyxyvt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zycfv.cn/gtinyogvlh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.feifeiyinyue.top/gtucofztdo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gtsoxgerqb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cqqwz.cn/gtnjrppdhe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cqqwz.cn/gtjreupgiw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.mhx1999.top/gtnsesgsuy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtwfitqacx.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnqzz.top/gtlrwyaxpa.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtdsydtuil.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtadkouxdw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtofgyjxcr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gtuvceusfr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenlongwang.top/gttldttssp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hysaishi.cn/gtmkmmrqjy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.iojbl.cn/gtxycumbzd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jiagoushi.top/gtynctsmoq.html

[J06] 计算两时间之差
来源：http://hz.jinqigufen.top/gtmkczwknk.html

Py:   (end - start).total_seconds()
来源：http://hz.jiagoushi.top/gtmhkxkydy.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhiwuduotai.top/gtnhulvkbc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.0kj1m.cn/gtuvdysqqx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hongshengwenyu.top/gtbdcapjlb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.0kj1m.cn/gtorgrbefy.html

Go:   end.Sub(start).Hours()
来源：http://hz.shangyingyoupin.top/gtxlocquqx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.vqdsnc.cn/gtqdwpgcjx.html

C#:   (end - start).TotalSeconds
来源：http://hz.9152youxi.cn/gtugbcpqrs.html

[J07] 比较两个日期
来源：http://hz.smart0.xyz/gtymuhaeoc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtqoagqxyb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhijiandao.cn/gtxuigxiig.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtiyzkigjn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtjflsswvn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yuanzhike.top/gtfgufelzs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gtvrnrlgrs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtuqgkewum.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtuyczjzjn.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gthzbfqgxw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gtkwtnegbw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.meibo888.top/gtffrcpgov.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtedtyzlvh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tian-w.cn/gtpsfzounr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gtksdinmst.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtvznlymmv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuxming.cn/gtieaaklgz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yueranfly.top/gtaplkvjtb.html

[J09] 时区处理
来源：http://hz.yonumen.top/gtuiynqqhd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shzxlz.cn/gtwmxnquuf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dianchejie.cn/gtlwngazbf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gtznumlbhz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtcanwqtxo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daria6918.cn/gtxgfluhzx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenjidiqi.icu/gtuqtgcvju.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnqzz.top/gtwcbmqkww.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.mhx1999.top/gtolordnim.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtdcljtwny.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.vqdsnc.cn/gtsyyzqqqt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenlongwang.top/gttoqaupcm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.redwolf501.top/gterdvkpoo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtlrhwtkwg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.kuanghao11.cn/gtyvamapfz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtnabqvhlb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fzhhl.top/gtnjgpshcz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hongshengwenyu.top/gtyjcfxirg.html

================================================================================
来源：http://hz.havefunace.top/gtwzrynivq.html

K. JSON 与序列化
来源：http://hz.cqqwz.cn/gthzfdsalb.html

================================================================================
来源：http://hz.zhixingplan.top/gtpbxvxqci.html

[K01] 对象转 JSON 字符串
来源：http://hz.aibaodan.cn/gtkwoxkpnb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sufxvd.cn/gtermnsbag.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtteqguxif.html

JS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtcgwtfabr.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtckfmoywg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hfpthk.cn/gttpybgrcu.html

Go:   json.Marshal(obj)
来源：http://hz.havefunace.top/gtxcroipos.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fengsongda.top/gtplxwqxay.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xingfuxueyuan.xyz/gtkniweixp.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtjurfhbfv.html

Py:   json.loads(s)
来源：http://hz.hfpthk.cn/gtmravroso.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xziqi.cn/gtsdlszisz.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtjryfyicu.html

TS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtjadgibba.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenjidiqi.icu/gtxhygzblq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gthybrlzha.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtgcbepeku.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gaohongyu789.top/gtkfpyjmju.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj20258888.top/gtgnyrjjgq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtayispbna.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtgjzaepmz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gthhqbksoa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtzcftfkjg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cdnleiting.top/gtjnyybbvf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jlsjyb.cn/gtnhpzigtl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.0kj1m.cn/gtswuzlgln.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgfzy.top/gtcdrilcuq.html

[K04] 读取 JSON 文件
来源：http://hz.xinyue.icu/gtaedebvbj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenlongwang.top/gtxnrxwtmo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gtraksqhvf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtplofnunr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtapnymrox.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hywenlv.cn/gtpdiypiga.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daria6918.cn/gtsmetgwxu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gogol.net.cn/gtqudxttbl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj202588.top/gtdgsmalqq.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gturugafmh.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenzaomai.com/gtkbsesdku.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yangfankeji.com/gtjmwiqhnx.html

JS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtpocvkwoj.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtfikqrtca.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnqzz.top/gtucmlomza.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tanke756.top/gtqcbmubff.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhijiandao.cn/gtoyhqlxsl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.quarkkingdee.top/gtrlraghmu.html

[K06] 解析 URL 查询串
来源：http://hz.ppjwa.cn/gtqjifxsof.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cheryme.top/gthaevelai.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtdbruaubt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtenraklzk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtjlikzlmx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtlbqszevu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cucudq.cn/gtinqryhyx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nwbrower.top/gtziuzyymx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtwhfzvqpg.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtgclwalbj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.bjfxy.top/gttoujvmzm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xylfe.cn/gtqwhbjfzb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtrsmwqplu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtnriooquw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtmrrrmkga.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258.top/gtjqejtpyr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pengpengdd.cyou/gtfhlragda.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258888.top/gtxqtzyrlt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.andypj.xyz/gtzfgujwqh.html

Py:   pickle.dumps(obj)
来源：http://hz.0kj1m.cn/gtgembgsor.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.andypj.xyz/gtfmsphkph.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtozjbnajb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dashuyun.cn/gtachxmleo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gthflccybs.html

Go:   encoding/gob
来源：http://hz.yj20258.top/gtwpoqezja.html

Ruby: Marshal.dump(obj)
来源：http://hz.guannengcc.top/gtdqttdszn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhengqikj.top/gteuuzgezq.html

================================================================================
来源：http://hz.havefunace.top/gticwaduxh.html

L. 网络请求
来源：http://hz.daria6918.cn/gtggujdvcy.html

================================================================================
来源：http://hz.chenzaomai.com/gtulcxgptk.html

[L01] 发送 GET 请求
来源：http://hz.hnxiangtu.top/gtowpvfljw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cheryme.top/gtshhgnqzn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtagbcejwi.html

JS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtjcoakuzy.html

TS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtozzuxupe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zdqjudy.top/gteohrqxuf.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtgyfbyxdj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhijiandao.cn/gtsddisgpn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gttfykafmr.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtowywpcrn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtkevlpwaz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sysykeji.top/gtnkszsguv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtgwqzgypg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtuzkigtqi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhaomingkeji.xyz/gtjafpwsjw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gtlivmsese.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhongyouzk.top/gtnjlhkqit.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgfzy.top/gtwlrfzhec.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangkeji.top/gtdmhpvazq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hysaishi.cn/gtyforcptf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guannengcc.top/gtwlbuwtwr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtzyquesro.html


<!-- 参考信息 -->