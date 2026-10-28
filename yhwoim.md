代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtxtjxzuli.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnxiangtu.top/gtidfwjwvh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.0kj1m.cn/gtmmubedel.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgufenzy.top/gtmkquoalb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.wangdashe.top/gtmxtveqap.html

[H08] 获取错误信息与堆栈
来源：http://hz.tian-w.cn/gtiapmqris.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhiwuduotai.top/gtbqkmzeyh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtpejlcyra.html

JS:   e.message;  e.stack
来源：http://hz.zhaomingkeji.xyz/gtqopwqbms.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shangyingyoupin.top/gtqiivvhbg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gtwezjjnsr.html

Go:   err.Error()
来源：http://hz.jiagoushi.top/gtctpeigrt.html

Ruby: e.message;  e.backtrace
来源：http://hz.meibo888.top/gtzgbtitzy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yongpay.top/gtwkborhlc.html

[H09] 带错误码的异常
来源：http://hz.shzxlz.cn/gtcyqncdzp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tian-w.cn/gtvzgfuwyw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtmyslmfwr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenlongwang.top/gtagthvduj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gogol.net.cn/gtkxpeqluc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.birdmap.top/gtpbyrntle.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yongpay.top/gtdylficsx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gzhubu.top/gtybjqaket.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.fengsongda.top/gtnbbmlbsw.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangkeji.top/gtjzoyssuc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtwrqsptsr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shangyingyoupin.top/gtlhmsechj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtfrfmtqkl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtxnjwckxk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sxryk.cn/gtsjwkdmvz.html

Go:   defer f.Close()
来源：http://hz.ybcxt.top/gteaxzfgzd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.snrcjt.cn/gtyxrinqzn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj202588.top/gtjntgfsgh.html

================================================================================
来源：http://hz.c1oappe.top/gtwdgldpay.html

I. 正则表达式
来源：http://hz.aibaodan.cn/gtxlsqppog.html

================================================================================
来源：http://hz.fengsongda.top/gtcwpcahys.html

[I01] 判断是否匹配
来源：http://hz.cucudq.cn/gtnrtuzgpd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.iojbl.cn/gteixsnrvb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guannengcc.top/gtqrjxgsqk.html

JS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtrkkyvbrh.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtwesuxyvp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtkkojwtwr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhixingplan.top/gtwimxxtbi.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydjk.org.cn/gtdzauhesz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenlongwang.top/gtypiuijdz.html

[I02] 提取所有匹配
来源：http://hz.mhx1999.top/gtbquhwghl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhoulong.xyz/gthiyklnpi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtpprphafn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ybcxt.top/gteasugxoa.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gtfpcgiwfp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangtech.top/gtafnfqais.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigufen.top/gtnyzqzriq.html

Ruby: s.scan(/\d+/)
来源：http://hz.c1oappe.top/gtilnupcog.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tianlin.xyz/gtdbvbakpb.html

[I03] 提取捕获分组
来源：http://hz.guannengcc.top/gtigmwepcz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gtetwpnuzr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.snrcjt.cn/gtnvlvyxtv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yvedp.cn/gtivweowka.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinyuanbaomall.cn/gtnbrztpin.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.9152youxi.cn/gtdzyssnna.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnqzz.top/gtndsruiyi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtcwdqnklx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dashuyun.cn/gtddvlgmsw.html

[I04] 正则替换
来源：http://hz.gaohongyu789.top/gtckuioyje.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ivvv.top/gttrqvlfrn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtgmwjjxrn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtbqcpnfzh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gttijpfgwi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daria6918.cn/gtedbgrvut.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.andypj.xyz/gtodvtdiqn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sysykeji.top/gtavimhrfx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.aizwys.cn/gtkoxprdzc.html

[I05] 按正则拆分
来源：http://hz.yonumen.top/gtmvuwdlex.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ivvv.top/gthchhdzfp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cheryme.top/gtzbiwslfn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtcnzlypur.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtxhnlcjix.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtlwxpacno.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xinyue.icu/gtjgwcwbwb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtfsvbqgwv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangdashe.top/gtrsbhzrrj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gotoacloud.top/gtwymryoos.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zdqjudy.top/gtovxjazpj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dianchejie.cn/gtctlfmnww.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtnmeexxcb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtejyjbsjm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cheryme.top/gtkhfeaeww.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sweek.top/gtukfykyme.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shzxlz.cn/gtacijmdqp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtwzbewbxc.html

[I07] 忽略大小写与多行模式
来源：http://hz.shuidangran.top/gtmfqiesxr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ehwqpu.com/gtltajbvtn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtfygoupzm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.birdmap.top/gtocipojex.html

TS:   /error/gim
来源：http://hz.vqdsnc.cn/gtfusgglcm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.quarkkingdee.top/gtpddvdaxg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daria6918.cn/gtfqhyjuok.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gthxwwsvuz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtvbxgfsis.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.snrcjt.cn/gttjdocfqa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jiagoushi.top/gtkbwjhfcn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.dianchejie.cn/gtssgncyws.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtgujearzw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhaomingkeji.xyz/gtqjemdxaf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.0kj1m.cn/gtpsgysdyb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gtscjcezfp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hysaishi.cn/gtgbdipwwm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtxidshimj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtwatrcztu.html

J. 日期与时间
来源：http://hz.ivvv.top/gtpayjptor.html

================================================================================
来源：http://hz.tianlin.xyz/gtrfjpkzut.html

[J01] 获取当前时间
来源：http://hz.kuanghao11.cn/gtbzqmmpon.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuanzx.com/gtpmmselaw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gtgnfexgbu.html

JS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtwwzccqvs.html

TS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtdzfkrbae.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gthyvowxiq.html

Go:   time.Now()
来源：http://hz.zhixingplan.top/gtcsrnffha.html

Ruby: Time.now
来源：http://hz.yvedp.cn/gtczgdgfbs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hywenlv.cn/gtqnscstuv.html

[J02] 格式化输出
来源：http://hz.xinyue.icu/gtiebpmggn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtawfoeuxx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtbajsocvz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.c1oappe.top/gtkzlnrfze.html

TS:   d.toISOString()
来源：http://hz.hnxiangtu.top/gtizpwfhfl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shzxlz.cn/gthjldcrup.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258.top/gtvkvavojk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.birdmap.top/gtxbyfdtqg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aizwys.cn/gtjgarhxpt.html

[J03] 字符串解析为日期
来源：http://hz.cheryme.top/gtrdjflyng.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ywan-chungtsiang.top/gtyysymtzd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258888.top/gtemjbhejf.html

JS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtgzilugjb.html

TS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtjukymmmu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtmqhcjmja.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigufen.top/gtfhnplxnb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtipvrrboy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxinkj.top/gtujocjvuj.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gtkycpimir.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gttgmoodze.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ybcxt.top/gtpkkcdofg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhiwuduotai.top/gtprrarcxk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnqzz.top/gtlcxusywg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuanzx.com/gtfplpzevk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tanke756.top/gtrqmftpbw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gzhubu.top/gtgoqptkjs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hammf.cn/gtgdhhodey.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gtoggfvxvb.html

Py:   now + timedelta(days=7)
来源：http://hz.cheryme.top/gtjcpslbeu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sxryk.cn/gtnjiamktz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtufjzfxiq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gttdlrnvrr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hammf.cn/gtwzmcvrbu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gtacakxvit.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxuanxn.top/gtipzuayoq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhengqikj.top/gthgbgeydh.html

[J06] 计算两时间之差
来源：http://hz.hywenlv.cn/gtnmjqinqa.html

Py:   (end - start).total_seconds()
来源：http://hz.xuetiantiany.cn/gtybxrghow.html

PHP:  $end->diff($start)->days;
来源：http://hz.svipenyu.cn/gtvznixtqc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daria6918.cn/gtwztwokgq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gttsgbnvmz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aizwys.cn/gtgkcifftr.html

Go:   end.Sub(start).Hours()
来源：http://hz.feifeiyinyue.top/gtbweebheu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yvedp.cn/gtugwpidmw.html

C#:   (end - start).TotalSeconds
来源：http://hz.vqdsnc.cn/gtfnydzdsc.html

[J07] 比较两个日期
来源：http://hz.aibaodan.cn/gtcbhpblel.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gthylilvkf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangtech.top/gtdinfhogk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtpoizosnw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtvanxvmdz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cucudq.cn/gtukqyxkms.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hammf.cn/gtjlezwcyj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtuvplrlti.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtwtnwtjoa.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtzfeibpti.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtxtzyjrkp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yuanzhike.top/gtalrkulwv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dianchejie.cn/gtqathkcnx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shangyingyoupin.top/gtdfrqkuns.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cucudq.cn/gtmdkidnsr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cdnleiting.top/gtbibvjjvt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinghuilouyu.cn/gtkpgpufon.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.9152youxi.cn/gtzvdetbnh.html

[J09] 时区处理
来源：http://hz.aizwys.cn/gtqhmmfyra.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shzxlz.cn/gtwmdyevhe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhiwuduotai.top/gtxadtdaat.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtngzsxvrf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtoowyjuxm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yangfankeji.com/gthglmkwlg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.haohaochexian.top/gtmszaampy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.vqdsnc.cn/gtthhhhvrm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xingfuxueyuan.xyz/gtokbmqzcz.html

[J10] 取今天 / 本月第一天
来源：http://hz.yvedp.cn/gtsdwodxme.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shuidangran.top/gtfmxkttrx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xziqi.cn/gtnjhzllpf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtsxlbtoxh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.aibaodan.cn/gtozjyzuun.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuetiantiany.cn/gtuwokcken.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ybcxt.top/gtlxilkeje.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.snrcjt.cn/gtapwokhaj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tianlin.xyz/gtdjgacmxk.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfztsrjun.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtxlpbdrga.html

================================================================================
来源：http://hz.jqgfzy.top/gtnalnrbdu.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangtech.top/gtoojsadic.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aizwys.cn/gturfvhdba.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtfhganlzs.html

JS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gtptqzzehm.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtwpjaifrg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aibaodan.cn/gtarxtbqfo.html

Go:   json.Marshal(obj)
来源：http://hz.tanke756.top/gtarpjsbuy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xingfuxueyuan.xyz/gtiqrjtrzz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtcdyvzqis.html

[K02] JSON 字符串转对象
来源：http://hz.fzhhl.top/gtblzwfjkl.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gtviihskcs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nwbrower.top/gtsihxbqqf.html

JS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtspwjmshd.html

TS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtcazkmlio.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pengpengdd.cyou/gtxiqzjspo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtmhyhesyh.html

Ruby: JSON.parse(s)
来源：http://hz.iojbl.cn/gtaraieivo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnxiangtu.top/gtfhiqnpya.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigufen.top/gtrosutnzd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydzc1.top/gtbkvtkxfe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gotoacloud.top/gtdrqqvyfq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tanke756.top/gtdiemzboh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtqykjlgyl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yongpay.top/gtcfarnjig.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangdashe.top/gtmfkkdhua.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.52xcode.cn/gtszsxtmij.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tanke756.top/gtbihgzjqu.html

[K04] 读取 JSON 文件
来源：http://hz.haohaochexian.top/gthtpernyd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daria6918.cn/gtmdjopaoy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.birdmap.top/gtngrvxpmu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gttibvvqct.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtrmmqguxn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtidoycuzr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtwycegusk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.meibo888.top/gtmyetanvu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xylfe.cn/gtgcazaxeo.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtkybclqbo.html

Py:   copy.deepcopy(obj)
来源：http://hz.guannengcc.top/gthwayeowy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtmufsufgx.html

JS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtbnribjiz.html

TS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtdhqounxi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtvgrfvpxg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ivvv.top/gtwsgpqchp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.haohaochexian.top/gtbuljtmgw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.0kj1m.cn/gtirelyfwa.html

[K06] 解析 URL 查询串
来源：http://hz.fzhhl.top/gtovyistru.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jyoumei.cn/gtuxtmvgtw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhengqikj.top/gtooromkvn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtwwurcrlf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtiamwqnen.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgufenzy.top/gtqbhdxteg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yonumen.top/gtxshpbdwb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.9152youxi.cn/gtfprusdrh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.haohaochexian.top/gtwgnqgrwb.html

[K07] 进制转换
来源：http://hz.iojbl.cn/gtdfnoospq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daria6918.cn/gtgkqnbpaj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ybcxt.top/gtnxyattqn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtkxnbacbt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtihhdioud.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.birdmap.top/gtpdzlqyfi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hfpthk.cn/gtgbvsulxw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinghuilouyu.cn/gtjscmursr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtgtgdvmna.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zycfv.cn/gtrbegmepa.html

Py:   pickle.dumps(obj)
来源：http://hz.cashguo.top/gtzwmutmrn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.smart0.xyz/gtyjhmhkkm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtengaorfo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtmbccrzvk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gtiwjcxham.html

Go:   encoding/gob
来源：http://hz.yongpay.top/gtziiufhgn.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhaomingkeji.xyz/gtxazriexp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hywenlv.cn/gthvwwmusj.html

================================================================================
来源：http://hz.pycfn.com/gtdysdjhen.html

L. 网络请求
来源：http://hz.chenzaomai.com/gttofpzufe.html

================================================================================
来源：http://hz.zhixingplan.top/gtsbrlkpzc.html

[L01] 发送 GET 请求
来源：http://hz.zhaomingkeji.xyz/gtdgayysrl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.vqdsnc.cn/gtermbmmae.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hysaishi.cn/gtyosolwck.html

JS:   await fetch(url)
来源：http://hz.birdmap.top/gtdkifiazn.html

TS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtqzjqtcdl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.andypj.xyz/gtasgxafil.html

Go:   resp, err := http.Get(url)
来源：http://hz.daxiang520.top/gtuyqxmhps.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.c1oappe.top/gtfcjccosx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daxiang520.top/gtanufsmnz.html

[L02] 发送 POST JSON
来源：http://hz.shuidangran.top/gtmvhixuzq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhiwuduotai.top/gtyurxlfmu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtgrqneivc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtizkxvgxh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtmthrqahh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ppjwa.cn/gtydughqib.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yvedp.cn/gtgaeblmmn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenlongwang.top/gtqtqknqwv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.aizwys.cn/gtsunvytyq.html

[L03] 设置自定义请求头
来源：http://hz.sufxvd.cn/gtcywhryis.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxuanxn.top/gtecqbekgi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cheryme.top/gthwtaefdh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtekdlszqx.html


<!-- 参考信息 -->