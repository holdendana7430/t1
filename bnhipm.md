代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.jqgfzy.top/gtyabtnzlj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jiagoushi.top/gtruabgdlw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pycfn.com/gtahjjppuu.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gtzeajrtra.html

Ruby: e.message;  e.backtrace
来源：http://hz.aibaodan.cn/gthnyfdehh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cashguo.top/gtccwgracd.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtliudhcna.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yonumen.top/gtetzsiuwz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.haohaochexian.top/gthcswujwk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xinyue.icu/gttxttrgnp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aibaodan.cn/gtpxkcdnyk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.daxiang520.top/gtcpebitwj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gotoacloud.top/gtvsqxglbp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.52xcode.cn/gtytzvicfm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gzhubu.top/gtztpbguws.html

[H10] 资源自动释放
来源：http://hz.havefunace.top/gtsjfuoekc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtcschuvgf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guowangkeji.top/gtmitapuib.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtpkngwbdy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtgnkdsupt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhijiandao.cn/gtbqxmqyho.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gtjjgkudvz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sysykeji.top/gtsdpywtam.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtqteqeosp.html

================================================================================
来源：http://hz.ppjwa.cn/gtghezwbxw.html

I. 正则表达式
来源：http://hz.c1oappe.top/gtvssaamsm.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtazcjkque.html

[I01] 判断是否匹配
来源：http://hz.ppjwa.cn/gtfivrkrou.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nanxuanxn.top/gtollosecr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gogol.net.cn/gtrzaesllb.html

JS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtlbeovacs.html

TS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtskrepjqf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.haohaochexian.top/gtuaklrmuz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtjudhfupm.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gtcomybnrt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yongpay.top/gtmrwajhbf.html

[I02] 提取所有匹配
来源：http://hz.hnxiangtu.top/gtumdmlrge.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sysykeji.top/gtefusgqrs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cdnleiting.top/gteggzhtew.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.guowangkeji.top/gtqcnllxum.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgfzy.top/gteowqjnhs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtuctuproy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.mhx1999.top/gtatdnhvor.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gtcxioxovc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gtsdzpnwev.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangtech.top/gtxxjsehad.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258888.top/gtawaqmoua.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtrhdqoacc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jlsjyb.cn/gtvoagrlwd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yonumen.top/gtmtukixbo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sysykeji.top/gtouonmjll.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daria6918.cn/gtmdeitqez.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gtkkplhezu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.meibo888.top/gtgmajaevl.html

[I04] 正则替换
来源：http://hz.yongpay.top/gtwlppsfpe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tian-w.cn/gtrotzfvyt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gtwhrummkc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtkgsepnvs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtbeichyko.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gtkrrrejvx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.0kj1m.cn/gtkgedgpdh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shuidangran.top/gtzxttjxkt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenzaomai.com/gtqeqxubwi.html

[I05] 按正则拆分
来源：http://hz.aibaodan.cn/gtkepivkqu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.0kj1m.cn/gtiwnaxaxe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhixingplan.top/gtoidwgfgl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtymjfrtxg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtwpezbcgx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuanzhike.top/gtnzqmjxtc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cashguo.top/gtpsxwnkny.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtuxdgnzrr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hysaishi.cn/gtbncopzuo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yueranfly.top/gtsbqtjfwt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtcmnhqqil.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.quarkkingdee.top/gtputskrys.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtgwqgvuei.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtxgznbvrl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhijiandao.cn/gtztyynfvi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hysaishi.cn/gtaevqrwwh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jiagoushi.top/gtojiusfnf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtlzipzodt.html

[I07] 忽略大小写与多行模式
来源：http://hz.tian-w.cn/gtgpqqkfwq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtanqlczhc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.kuanghao11.cn/gtacqmgvof.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.c1oappe.top/gtkrgzxgxm.html

TS:   /error/gim
来源：http://hz.guowangkeji.top/gtsnrsveen.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tianlin.xyz/gtgsnviftf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhiwuduotai.top/gtwkacnkjh.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gtlkxageqa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtioxikojp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.smart0.xyz/gtkvicfwyi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gzhubu.top/gtmxcazdij.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hywenlv.cn/gtzuywvvmu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gthfslxusw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtqvoepshc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gtkyccljgo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shzxlz.cn/gtwysaexoz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhiwuduotai.top/gtbgvwjvms.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtdvfueyif.html

================================================================================
来源：http://hz.zhixingplan.top/gtdxjvqjxy.html

J. 日期与时间
来源：http://hz.cucudq.cn/gthlvzknbt.html

================================================================================
来源：http://hz.guowangkeji.top/gtpbikfzml.html

[J01] 获取当前时间
来源：http://hz.sxryk.cn/gtwtppddyp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sufxvd.cn/gtqvyvrytz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.fengsongda.top/gtvsnrnbbm.html

JS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtrwbshcaj.html

TS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtlwhjwmvs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dianchejie.cn/gtaexhrhlg.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtexzmuszk.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gtofmeubdm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dianchejie.cn/gtmcvwjebj.html

[J02] 格式化输出
来源：http://hz.wangshuangyany.cn/gtammrvrct.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtgqwmbxlu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtgveaweul.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgufenzy.top/gtmrflexnk.html

TS:   d.toISOString()
来源：http://hz.jyoumei.cn/gtaxzcftau.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuanzhike.top/gtzzrnnvsc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258888.top/gtcvvbqfig.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtlrrdrtsy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhiwuduotai.top/gtwvtztiyw.html

[J03] 字符串解析为日期
来源：http://hz.tianlin.xyz/gtlzhosinw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nanxinkj.top/gtdbogbvsm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tian-w.cn/gtbiwlcxzb.html

JS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtzycbvrjt.html

TS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtgzuylqzr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gtjrxvdxts.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guowangkeji.top/gtnzfsyixv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tanke756.top/gtyqwwjobe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xingfuxueyuan.xyz/gttbofozbd.html

[J04] 时间戳与日期互转
来源：http://hz.yvedp.cn/gtocouivim.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhongyouzk.top/gtyarykvay.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aizwys.cn/gtsfibjacq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnxiangtu.top/gtawggztar.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hfpthk.cn/gtnsuxylqz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.quarkkingdee.top/gtqvqhnprq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tianlin.xyz/gthhtbcutd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj202588.top/gtaogfgkjc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cqqwz.cn/gtxszotbta.html

[J05] 时间加减（加 7 天）
来源：http://hz.guannengcc.top/gtesvqexwv.html

Py:   now + timedelta(days=7)
来源：http://hz.yongpay.top/gtztxkfkaj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtruaohbmr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.snrcjt.cn/gtdnillsfd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gtreiptvma.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aizwys.cn/gtxqdqlfvv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yanxiufei.cn/gtcnauoild.html

Ruby: Time.now + 7 * 86400
来源：http://hz.haohaochexian.top/gtvixzpodh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.havefunace.top/gtlrimybvl.html

[J06] 计算两时间之差
来源：http://hz.cheryme.top/gttchfxihe.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxinkj.top/gtiguvsego.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gttoqbkqju.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ehwqpu.com/gtyfinuyjs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtlgxidypn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gtewkecsjc.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhixingplan.top/gtunlkyuci.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj20258888.top/gtsjywtmge.html

C#:   (end - start).TotalSeconds
来源：http://hz.aizwys.cn/gtkrsqlxpa.html

[J07] 比较两个日期
来源：http://hz.mhx1999.top/gtiikcveef.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtsoammnzm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangtech.top/gtgtiqamsd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtfepdvwyx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtjnifusvk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenzaomai.com/gttiacobyj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shuidangran.top/gthptwjxyz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtcjynblvt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtlukfwcjj.html

[J08] 提取年月日与星期
来源：http://hz.iojbl.cn/gtqawarrya.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.quarkkingdee.top/gtwcyrlamw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tian-w.cn/gtwrjhnilh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gzhubu.top/gtfbodxici.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnqzz.top/gtentwpamh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dianchejie.cn/gtngzqzjze.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cashguo.top/gtcqkfltai.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gtvbmerlhy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yanxiufei.cn/gtvizdaufp.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gthafxjsmb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhiwuduotai.top/gtmvqizjcg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.haohaochexian.top/gtlkkpmmbi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtthnlibpz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.quarkkingdee.top/gtltyjqcsa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtormunbgm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sweek.top/gtnkrncfkc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.feifeiyinyue.top/gtwxledppt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gtyuxwxzhd.html

[J10] 取今天 / 本月第一天
来源：http://hz.jlsjyb.cn/gtpfluljij.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.redwolf501.top/gteowxznmo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangtech.top/gttzlqhcrr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xylfe.cn/gtcvhyspbg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.aizwys.cn/gtqbiocsyv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtwaspgubw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hywenlv.cn/gtnwupmjtc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtvgqxbyri.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtgnswuvyn.html

================================================================================
来源：http://hz.yonumen.top/gtnnxwffzb.html

K. JSON 与序列化
来源：http://hz.yvedp.cn/gtmgsoeyaj.html

================================================================================
来源：http://hz.fengsongda.top/gtmabyuasy.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtzecrgvca.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtoxqlskht.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtcvkvfhwl.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtaususpln.html

TS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtbsuxitwt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhongyouzk.top/gtnyitisys.html

Go:   json.Marshal(obj)
来源：http://hz.hnxiangtu.top/gtudjxdavj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dianchejie.cn/gtvtfjvvga.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxuanxn.top/gtpdaphnag.html

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gtjivrwwop.html

Py:   json.loads(s)
来源：http://hz.cdnleiting.top/gthujeqqhp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuetiantiany.cn/gtaanyzgxx.html

JS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtrvcgrngu.html

TS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtnzzzslvj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.c1oappe.top/gtzdfdsslf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtpcmdpdaw.html

Ruby: JSON.parse(s)
来源：http://hz.hnqzz.top/gthqdpimxh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.andypj.xyz/gtojkmlwnr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xuanzx.com/gttrwogrtn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtdsoudhgf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtuzovhhwg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtjbeykmve.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtyyvhjwqb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gtillunbmg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.snrcjt.cn/gtdnihllah.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.havefunace.top/gtbqitythm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gtzawwsbqq.html

[K04] 读取 JSON 文件
来源：http://hz.vqdsnc.cn/gtpgrqwlwk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangshuangyany.cn/gtdzuqwlpf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yueranfly.top/gtwhowgili.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gtjkfroazh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gtsrccywyt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tian-w.cn/gtkoqvbobp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pengpengdd.cyou/gtafoptarc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.meibo888.top/gtlpxmotys.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtmnxkyied.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtkgtiwais.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenlongwang.top/gtwadfnuxo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xinyue.icu/gtpxdhjmam.html

JS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtwxuyhgkh.html

TS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtkyjfnxew.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhengqikj.top/gtbjdwaswl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtlvohxgxg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.9152youxi.cn/gtmzdkfofj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhengqikj.top/gtkzwmhofz.html

[K06] 解析 URL 查询串
来源：http://hz.pengpengdd.cyou/gtjeqfpyuj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigufen.top/gtmxcixclj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhoulong.xyz/gtgopmxekn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtnobiflho.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtgumsbocp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ivvv.top/gtbgomesgb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.redwolf501.top/gtcudfspjt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenlongwang.top/gtdybuqmdz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtuypxxrlr.html

[K07] 进制转换
来源：http://hz.jinghuilouyu.cn/gtsytobgsj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.316326.xyz/gtiavmoaop.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangdashe.top/gtofoxpbrh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtwsdzsgtb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtgoqkbvew.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtjlqlcfnx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.birdmap.top/gtatzdmibk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinghuilouyu.cn/gtbueamowc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gtqukklqvx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.vqdsnc.cn/gtvnkyncwl.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gtdevzixxi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nanxinkj.top/gtxcssgths.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtnqxwrcmh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtczyfbfpw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydjk.org.cn/gtazlwbzmn.html

Go:   encoding/gob
来源：http://hz.bjfxy.top/gtwbveqkqw.html

Ruby: Marshal.dump(obj)
来源：http://hz.9152youxi.cn/gtddskdxyb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.pengpengdd.cyou/gtnidvqbiz.html

================================================================================
来源：http://hz.gogol.net.cn/gtzusdhrhv.html

L. 网络请求
来源：http://hz.aizwys.cn/gtedeukvsf.html

================================================================================
来源：http://hz.meibo888.top/gtvaxfvsfz.html

[L01] 发送 GET 请求
来源：http://hz.zhixingplan.top/gtsmdbolnl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xinyue.icu/gtwuzqiney.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangdashe.top/gtcsofarwy.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtmemcfhvb.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtbabhhrmd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.feifeiyinyue.top/gtwzqaaejl.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnxiangtu.top/gtctruwtmd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zycfv.cn/gtzsnukblq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sxryk.cn/gtnfmklobq.html

[L02] 发送 POST JSON
来源：http://hz.cheryme.top/gtheiexeuc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xinyue.icu/gtlobsokcs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gtvjkcprhr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtikgvfhjb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gtkzyelzex.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yanxiufei.cn/gtsbofehtp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daria6918.cn/gtmgtzfuvn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xziqi.cn/gtwcamunqk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigufen.top/gtfdrpxjiq.html

[L03] 设置自定义请求头
来源：http://hz.hammf.cn/gtawahmpcb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.birdmap.top/gtwnyzljba.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sxryk.cn/gtkxgkbyik.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gthffascif.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cashguo.top/gtigevwsti.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jiagoushi.top/gtjunyuilq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.316326.xyz/gtqqysxzrf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydzc1.top/gtrefcbmsg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtaqhdlyzn.html

[L04] 设置超时
来源：http://hz.ivvv.top/gteabnqjlq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ivvv.top/gtsqlgnssm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xziqi.cn/gthnohogqv.html


<!-- 参考信息 -->