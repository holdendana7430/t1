代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtkwmfibzo.html

[H08] 获取错误信息与堆栈
来源：http://hz.cucudq.cn/gtloyomifr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtcaflidxq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangshuangyany.cn/gtuwksbhor.html

JS:   e.message;  e.stack
来源：http://hz.ywan-chungtsiang.top/gtasdoujen.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ivvv.top/gtrmqehkfa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnxiangtu.top/gtesapugxt.html

Go:   err.Error()
来源：http://hz.aizwys.cn/gtuzlazend.html

Ruby: e.message;  e.backtrace
来源：http://hz.sxryk.cn/gtcmpdflsa.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tianlin.xyz/gtrtplmhpj.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtxykptmfp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gtujfokgvt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.svipenyu.cn/gtrsvbnkas.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cheryme.top/gtbvokgmbv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.redwolf501.top/gtzscxhmxz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgfzy.top/gtmlecyekb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shuidangran.top/gtjedbktse.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.feifeiyinyue.top/gtehafklhn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zycfv.cn/gtpxabkagb.html

[H10] 资源自动释放
来源：http://hz.shuidangran.top/gtemhvmdrz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gtemvvukgy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sweek.top/gtejszymyc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtlhpopgjm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtabeecywb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hammf.cn/gtvcgzufwg.html

Go:   defer f.Close()
来源：http://hz.jiagoushi.top/gtihtcyfew.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zycfv.cn/gtknuqadpm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.kuanghao11.cn/gtoywsmsqm.html

================================================================================
来源：http://hz.zhongyouzk.top/gtsvcaoory.html

I. 正则表达式
来源：http://hz.0kj1m.cn/gtctjgbjbi.html

================================================================================
来源：http://hz.316326.xyz/gtddvpszdc.html

[I01] 判断是否匹配
来源：http://hz.sxryk.cn/gtuqmgtizj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtzwwjhgsv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shuidangran.top/gtgzjifhcw.html

JS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtrcbxeynb.html

TS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtbzcjlbsu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtleyuoyyy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sufxvd.cn/gtdlultppa.html

Ruby: s.match?(/\d+/)
来源：http://hz.guowangkeji.top/gtfyuglsed.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hywenlv.cn/gtifnkmlca.html

[I02] 提取所有匹配
来源：http://hz.havefunace.top/gtwjsedrvg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hywenlv.cn/gtxifwjmqx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jianghu66.top/gtzrozpers.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.bjfxy.top/gtvkijfajt.html

TS:   s.match(/\d+/g)
来源：http://hz.jianghu66.top/gtlvpqjoll.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aibaodan.cn/gtarwgvmxp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj20258888.top/gtoogkmeru.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gtxbudahhp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zycfv.cn/gtlkedkoky.html

[I03] 提取捕获分组
来源：http://hz.fzhhl.top/gtcxuduxrv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gotoacloud.top/gtopmciizc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.c1oappe.top/gtuykavzwa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangtech.top/gtmvuutmna.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgfzy.top/gtvpetzoci.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhiwuduotai.top/gtqlbqszcd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigfzy.top/gtxwcmilvd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daxiang520.top/gtfjhbhpfw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.316326.xyz/gtpnfezrov.html

[I04] 正则替换
来源：http://hz.cheryme.top/gtwuifoczv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hongshengwenyu.top/gthnxfbpwk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gtxfqbfcpu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nwbrower.top/gtrwpxmwxx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtfqkuiime.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangshuangyany.cn/gtcjipcknw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guowangkeji.top/gtjygdtxzz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinghuilouyu.cn/gtmillusmh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtfwkncdzu.html

[I05] 按正则拆分
来源：http://hz.aizwys.cn/gtigvcpcre.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigufen.top/gtrxfjzlmp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhaomingkeji.xyz/gtzpyxduku.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtsxhntwsd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtimffbquv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yonumen.top/gtzvluspxi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jlsjyb.cn/gttyzcbigu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtonvcdztk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.9152youxi.cn/gtfgjnwgyc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.feifeiyinyue.top/gthsblsxmu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtopoakfpe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj20258888.top/gtxgydgxlt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtvjuiyqen.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtbikifide.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gttuezzivu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pengpengdd.cyou/gtjqbjngvo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.mhx1999.top/gterzolfyz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtsbpbknyw.html

[I07] 忽略大小写与多行模式
来源：http://hz.gzhubu.top/gtxmmnbycb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtwelrugye.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhiwuduotai.top/gtjzczsfhi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yvedp.cn/gtcrnehtol.html

TS:   /error/gim
来源：http://hz.hfpthk.cn/gtelsknwpy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxuanxn.top/gtnumurgtv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xziqi.cn/gtbffsvjuj.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258888.top/gtzlnujujk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hnqzz.top/gtpwpskmhd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.c1oappe.top/gtcaovkqla.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ywan-chungtsiang.top/gtxtedfcmy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnqzz.top/gtljxwlmql.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtwgbuvhmp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gthrcstjcd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtgbyhybgd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daxiang520.top/gtaepdkhhc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtlwrhdmib.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xylfe.cn/gtitwmkjyh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtsdkpogcw.html

J. 日期与时间
来源：http://hz.tianlin.xyz/gtarbkczah.html

================================================================================
来源：http://hz.zhongyouzk.top/gtwgmqkfen.html

[J01] 获取当前时间
来源：http://hz.guowangkeji.top/gtpihmqkiu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258.top/gtytlfpyvl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtpgvmmnsf.html

JS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtgyaflnyz.html

TS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gtfqpezfaz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dianchejie.cn/gtulfjicxr.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtilziccws.html

Ruby: Time.now
来源：http://hz.yj202588.top/gtkealnvrb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xingfuxueyuan.xyz/gtfdnvmwue.html

[J02] 格式化输出
来源：http://hz.iojbl.cn/gtooiysdze.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.316326.xyz/gtngwfftge.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydjk.org.cn/gtlrfuwqmd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hysaishi.cn/gtaxthlpst.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gtfiidmfem.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhongyouzk.top/gtfeeoxbme.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258888.top/gtookrssdq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gttgqajbmw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtxwhvswrb.html

[J03] 字符串解析为日期
来源：http://hz.zhongyouzk.top/gtnwiinorl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuanzhike.top/gtfjishbgc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinyuanbaomall.cn/gtnpiihvov.html

JS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtsamnhpxa.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gteyhnimll.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtefunhofy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigufen.top/gtlxohqhxx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtqfaudwgk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hammf.cn/gttzlprijx.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangtech.top/gtksrzwbrs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtfmtgvozq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.bjfxy.top/gtqeuokhwe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydjk.org.cn/gtjckjqxvk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cqqwz.cn/gtvbuefmyb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigfzy.top/gtgppebjgf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtmjshaoca.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xziqi.cn/gtpcbpyhir.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgfzy.top/gtpxngxodc.html

[J05] 时间加减（加 7 天）
来源：http://hz.sysykeji.top/gtnondyqdw.html

Py:   now + timedelta(days=7)
来源：http://hz.gzhubu.top/gtpgetfrfk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydzc1.top/gtffezaghf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtsywenrfd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtszgbgzbo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinyuanbaomall.cn/gtpwxjkzvm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.52xcode.cn/gtidtsctzi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangdashe.top/gtpzccjfxk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgufenzy.top/gtraljkqcl.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gtnaiqysgm.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtmouhdoqa.html

PHP:  $end->diff($start)->days;
来源：http://hz.ivvv.top/gtqzlbsisl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zdqjudy.top/gtbrfajxdc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.iojbl.cn/gtqwfxuqmb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtwsyhedjk.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gtswlttchy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ehwqpu.com/gthcnnovxg.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj202588.top/gtetomozas.html

[J07] 比较两个日期
来源：http://hz.nanxinkj.top/gtushozaub.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtvtuotxsd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgfzy.top/gtmpdcrvfl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtgsizdoax.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtbmmxkryl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yuxming.cn/gtxessrdhx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.andypj.xyz/gtgoxwxnrn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtitoxqmmr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtkphazims.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtawajuaex.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aizwys.cn/gtytyicxma.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtkyytqgcg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shzxlz.cn/gtxgecowhb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xziqi.cn/gtlofxuvny.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtxnldqjec.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hywenlv.cn/gtcefdmzus.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydzc1.top/gtmxmkfphc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtwutcjnhj.html

[J09] 时区处理
来源：http://hz.xinyue.icu/gtwpmvosfd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.iojbl.cn/gtolplpdin.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yuanzhike.top/gtodakhosw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gthunjjkul.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtipieyvrm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xinyue.icu/gtswaekcws.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinghuilouyu.cn/gtysezscdc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnqzz.top/gtvnhxvjbr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinghuilouyu.cn/gtfoducfek.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtffuzkxsz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yanxiufei.cn/gtjqsutndx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hywenlv.cn/gtmfwdppui.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hfpthk.cn/gtinhunfiw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cucudq.cn/gtkjlfbwhy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jlsjyb.cn/gtnywbiyrv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhongyouzk.top/gtdnmgrdfc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shuidangran.top/gtddazhcfc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gaohongyu789.top/gtgqmgqzra.html

================================================================================
来源：http://hz.gogol.net.cn/gtbhnxlxuq.html

K. JSON 与序列化
来源：http://hz.haohaochexian.top/gtxirsoeyt.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtayfspdud.html

[K01] 对象转 JSON 字符串
来源：http://hz.zycfv.cn/gtkdcxebix.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtagmipbmo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtokzymfpi.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtgjxyiybf.html

TS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtzoxlzvmf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.52xcode.cn/gtulngbuyr.html

Go:   json.Marshal(obj)
来源：http://hz.chenjidiqi.icu/gtnhbmobmk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtjtwgxipx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.pycfn.com/gtarixaumy.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gtfrcwqvqm.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangtech.top/gtkwaivglb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhoulong.xyz/gtmitytvvp.html

JS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtxysequdj.html

TS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtdwkivizz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pycfn.com/gtmqibwdqj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtcbfolres.html

Ruby: JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtoanjvgji.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.snrcjt.cn/gteaooznlq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangdashe.top/gtlgmgcijs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtoiqhvfws.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtmdadvomx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtxvmpssmp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtstgehtmr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.kuanghao11.cn/gtfqrckqmv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtivkvzsoq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gttdwukdxm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnqzz.top/gtmsxdlcum.html

[K04] 读取 JSON 文件
来源：http://hz.iojbl.cn/gtoxvzvsvt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinyuanbaomall.cn/gtkwqquzel.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxuanxn.top/gtirdjmvez.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtxqbtcvhh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sufxvd.cn/gtryaihdcw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dashuyun.cn/gtpmgqcpla.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.9152youxi.cn/gtkduseidy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shzxlz.cn/gtnwbflllt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dianchejie.cn/gtvofrlucb.html

[K05] 深拷贝对象
来源：http://hz.bjfxy.top/gtdralqctx.html

Py:   copy.deepcopy(obj)
来源：http://hz.pycfn.com/gtiszliaog.html

PHP:  unserialize(serialize($obj));
来源：http://hz.meibo888.top/gtrmmbneyt.html

JS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtedwmpaay.html

TS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtapylhxrx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.bjfxy.top/gttxswudll.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxuanxn.top/gtpanrznpe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cdnleiting.top/gtimjlnmqk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guannengcc.top/gtnzomndsn.html

[K06] 解析 URL 查询串
来源：http://hz.yongpay.top/gtkiwjhcne.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenjidiqi.icu/gtknvbnoxn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xziqi.cn/gttrrkfnpk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtqpdtfdlf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtfdgpveoh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gtjjqgpuei.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtfkwvboaa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtpwfklscp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtllsbsgtx.html

[K07] 进制转换
来源：http://hz.jqgfzy.top/gtabuubbxn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydjk.org.cn/gtqkrrvadg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtzjnkjumx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtvhzfhmpd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtwqthqsfw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtbwqncwyz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daria6918.cn/gtrikiuxec.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtpampibuj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuanzhike.top/gtiyzihmor.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtdnngexmp.html

Py:   pickle.dumps(obj)
来源：http://hz.jqgfzy.top/gtalmrdruv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.c1oappe.top/gteognayvn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtoehgamrw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cucudq.cn/gtgdaquxpu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gtoddyxhpf.html

Go:   encoding/gob
来源：http://hz.316326.xyz/gtdrrbehui.html

Ruby: Marshal.dump(obj)
来源：http://hz.daxiang520.top/gtqscwrgil.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ppjwa.cn/gtpdxnyoqf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthtcsvdmx.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtmhcecoxf.html

================================================================================
来源：http://hz.hammf.cn/gtndcwpnvr.html

[L01] 发送 GET 请求
来源：http://hz.wangdashe.top/gttsshaddu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hammf.cn/gtdkizedey.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shuidangran.top/gtmbcnxvpf.html

JS:   await fetch(url)
来源：http://hz.yangfankeji.com/gtawgfpptx.html

TS:   await fetch(url)
来源：http://hz.ivvv.top/gtxvlkdzxo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinyuanbaomall.cn/gtebazfhhq.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258888.top/gtbtncqlbd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gtjftxvoff.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daria6918.cn/gtihvswulz.html

[L02] 发送 POST JSON
来源：http://hz.yangfankeji.com/gtzzbwplxd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenzaomai.com/gtfjxegkcv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhaomingkeji.xyz/gtgogegtuq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtbiafvexe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtzdaiysab.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangdashe.top/gtmsssrnnk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yangfankeji.com/gtwcvisjxw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtbewrdkcw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.bjfxy.top/gtiomefwci.html

[L03] 设置自定义请求头
来源：http://hz.dashuyun.cn/gtrwtjudda.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydjk.org.cn/gtcvrnhpxf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigufen.top/gtsljvpkmj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ybcxt.top/gtwbzackrw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtrtzlvydp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ywan-chungtsiang.top/gtazllvsnf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xinyue.icu/gtsryokjyw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jlsjyb.cn/gtuvfmfibq.html


<!-- 参考信息 -->