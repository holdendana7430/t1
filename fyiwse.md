代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.daxiang520.top/gtgraibnyn.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhongyouzk.top/gtiwljfsqw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtesuhwzcc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.andypj.xyz/gtubdazlvu.html

JS:   e.message;  e.stack
来源：http://hz.sysykeji.top/gthhihydov.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.svipenyu.cn/gtuuqxlgbs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.haohaochexian.top/gtsyefjqkr.html

Go:   err.Error()
来源：http://hz.fzhhl.top/gtdfabigps.html

Ruby: e.message;  e.backtrace
来源：http://hz.hongshengwenyu.top/gtgythlqum.html

C#:   e.Message;  e.StackTrace
来源：http://hz.svipenyu.cn/gtpwmgvwsz.html

[H09] 带错误码的异常
来源：http://hz.zhongyouzk.top/gtkryhkqpj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gtgguengvl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cucudq.cn/gtgyhdzyxb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtvwhproxl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhaomingkeji.xyz/gttzxjenns.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.havefunace.top/gterquscum.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gttexnmrgn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.vqdsnc.cn/gttccksvyy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnqzz.top/gtkkaypiht.html

[H10] 资源自动释放
来源：http://hz.zhengqikj.top/gttwywthyh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtgolpvmwo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigufen.top/gtaztuifnt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gtxhxyxyxd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtuuxdihhc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.0kj1m.cn/gtpknsamdp.html

Go:   defer f.Close()
来源：http://hz.dianchejie.cn/gtcwbfvega.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ivvv.top/gtcnfdodzq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cashguo.top/gtrmizwahk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtdiavlkbo.html

I. 正则表达式
来源：http://hz.zhiwuduotai.top/gtgpdewwdu.html

================================================================================
来源：http://hz.havefunace.top/gtpuhqjnmm.html

[I01] 判断是否匹配
来源：http://hz.jiagoushi.top/gtryzafcbu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtprvejqnk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtofglptrf.html

JS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtsofxfflw.html

TS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtsfgkdfqo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.9152youxi.cn/gttdxcdbbw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydzc1.top/gthwvwplru.html

Ruby: s.match?(/\d+/)
来源：http://hz.cdnleiting.top/gtmoehkpjy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxinkj.top/gtgcjslwxf.html

[I02] 提取所有匹配
来源：http://hz.tianlin.xyz/gtcaoefccq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.9152youxi.cn/gtpzcqvegd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guannengcc.top/gtbcefmmro.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hammf.cn/gtjexmhdew.html

TS:   s.match(/\d+/g)
来源：http://hz.sufxvd.cn/gtboqplkik.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhengqikj.top/gtvsnnslup.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj20258888.top/gthwwfkhnb.html

Ruby: s.scan(/\d+/)
来源：http://hz.snrcjt.cn/gtbhlrdbgd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gaohongyu789.top/gtyzuwtuyd.html

[I03] 提取捕获分组
来源：http://hz.ehwqpu.com/gtctnvkpaz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xinyue.icu/gtfpcnglay.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gthgmsqeyr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hywenlv.cn/gtmrbnphmx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hysaishi.cn/gtzslqehzu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangshuangyany.cn/gtsvwppjbf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtmycxdoli.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tianlin.xyz/gtdhiutmea.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gtqclvdaya.html

[I04] 正则替换
来源：http://hz.cqqwz.cn/gtpleeicei.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ybcxt.top/gtdwknqqdy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gtdkcsgkpj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtkktqmpap.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtlgabpqjr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gtbpvvdssy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangtech.top/gtdkwrttbu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtspthkorz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtueceoedd.html

[I05] 按正则拆分
来源：http://hz.fzhhl.top/gtdnhuvygc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigfzy.top/gtgqxqhcqb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhijiandao.cn/gtgghzewix.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gthmpsdjko.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinghuilouyu.cn/gtehjjneup.html

Java: s.split("\\s*,\\s*")
来源：http://hz.316326.xyz/gtjrkvspkh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yongpay.top/gthkpxbohh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtvjarayue.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgufenzy.top/gtjhajlgdg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhoulong.xyz/gtqqohkmkt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gthorwxnoq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yueranfly.top/gtnznggszt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtcanbfisx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhengqikj.top/gtkenqldmc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tanke756.top/gtlmiotvfx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtbhdmpdgr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gtczweilxl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtgxjajnux.html

[I07] 忽略大小写与多行模式
来源：http://hz.fzhhl.top/gttgiccpkb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pycfn.com/gtoggjtbjn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hammf.cn/gtwoykgshy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tian-w.cn/gtkxmonwmv.html

TS:   /error/gim
来源：http://hz.jinghuilouyu.cn/gtqgosssvi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tianlin.xyz/gtqjymfrax.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xziqi.cn/gtwmncdnyx.html

Ruby: s.scan(/error/i)
来源：http://hz.chenlongwang.top/gtbnfbpoef.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.iojbl.cn/gthsalxlsj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zycfv.cn/gtrxshkfdo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pengpengdd.cyou/gtnuxicpks.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnxiangtu.top/gtzcxmjeyu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtzirmuirb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.quarkkingdee.top/gtbtioyqad.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuxming.cn/gtxgcxquzf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yvedp.cn/gttwosyvyv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.svipenyu.cn/gthzabvmaa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gtetktejeb.html

================================================================================
来源：http://hz.jinqigufen.top/gtodpeynbi.html

J. 日期与时间
来源：http://hz.aibaodan.cn/gtchvkmeje.html

================================================================================
来源：http://hz.zhixingplan.top/gtmwddnmop.html

[J01] 获取当前时间
来源：http://hz.gzhubu.top/gtqnuvwimx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuetiantiany.cn/gtryqarqji.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtydyqxaum.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtzlufbxzw.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtznlcfnsy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ybcxt.top/gtbyprbaiv.html

Go:   time.Now()
来源：http://hz.fzhhl.top/gtgwkklzkl.html

Ruby: Time.now
来源：http://hz.feifeiyinyue.top/gtgpmjukfc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xinyue.icu/gtzqfebusa.html

[J02] 格式化输出
来源：http://hz.jqgufenzy.top/gtldiwvbsq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gtwptqcykm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtvrnckbxg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sysykeji.top/gtszycpdqy.html

TS:   d.toISOString()
来源：http://hz.tian-w.cn/gtvkxjjnuv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtadkngbpy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ehwqpu.com/gtxgwjdnto.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtmxxweivi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.9152youxi.cn/gtrcracnfm.html

[J03] 字符串解析为日期
来源：http://hz.wangshuangyany.cn/gtfeuwrvge.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dashuyun.cn/gtdabipwux.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinyuanbaomall.cn/gtpdegeedx.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtjygfuowx.html

TS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtkaokrcdv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtraotslmd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxinkj.top/gtfsixywqs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtpakudkfq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gtavkkbyak.html

[J04] 时间戳与日期互转
来源：http://hz.shzxlz.cn/gtukrdhrtl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnqzz.top/gtztzdcivg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.snrcjt.cn/gtvsnbwylg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gtvekibeua.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtrphosrei.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aizwys.cn/gtpslseelq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sysykeji.top/gtzanaufpl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.9152youxi.cn/gtvwkyrnjz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hysaishi.cn/gtdglmcsfu.html

[J05] 时间加减（加 7 天）
来源：http://hz.bjfxy.top/gtrydcxott.html

Py:   now + timedelta(days=7)
来源：http://hz.c1oappe.top/gtdfeneiwe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigfzy.top/gtwwurtwxf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtyijuvgdi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtjkmiwngo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cheryme.top/gtxvpcbwrc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinghuilouyu.cn/gtgolowszr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtiwijjsan.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pengpengdd.cyou/gtwhgbsmko.html

[J06] 计算两时间之差
来源：http://hz.kuanghao11.cn/gtamtacxtf.html

Py:   (end - start).total_seconds()
来源：http://hz.hongshengwenyu.top/gttgkcfkwk.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gtlphwxuxx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shzxlz.cn/gtrlyecgjr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenlongwang.top/gtttssfvzy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.316326.xyz/gtwsnobsbu.html

Go:   end.Sub(start).Hours()
来源：http://hz.zycfv.cn/gtrvxsqaxg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shanyushiyangtech.top/gtwuoyphed.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxinkj.top/gtaujeadgn.html

[J07] 比较两个日期
来源：http://hz.chenlongwang.top/gtpeydwkke.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtvilmjuwe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.feifeiyinyue.top/gtptmozlvt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtabcltaqh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtnnasutlf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtboejedur.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtjtvoyfag.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtbztfwzoe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtgnwmyxok.html

[J08] 提取年月日与星期
来源：http://hz.xingfuxueyuan.xyz/gtcrqspgud.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yvedp.cn/gtqyxvdpul.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangtech.top/gtjcxqvges.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xziqi.cn/gtbbtqqahg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhixingplan.top/gtozceielp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tian-w.cn/gtaewnlqwn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinghuilouyu.cn/gtxngwrzlt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.c1oappe.top/gtonruuitf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daria6918.cn/gtiuxwqqaq.html

[J09] 时区处理
来源：http://hz.ybcxt.top/gtwxbeyqrl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tanke756.top/gtdmnddxqk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hongshengwenyu.top/gtdbsflzop.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gtbolvsexj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtfjcfnkmt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shzxlz.cn/gtiqqwhzzs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhaomingkeji.xyz/gtvfwaksqc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zycfv.cn/gtmczsesbc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnxiangtu.top/gtnyjzliso.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtqapfjptl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gzhubu.top/gtzbgfqpzq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj202588.top/gtwhwsjrfz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gtlkirvode.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yvedp.cn/gtoyhihpgh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtitcvzszb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gtbtamzlye.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nanxuanxn.top/gtbghzmczb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gthxfgnace.html

================================================================================
来源：http://hz.0kj1m.cn/gtvgfrxzdb.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gtdnjyyizz.html

================================================================================
来源：http://hz.xuanzx.com/gtsqbavhlp.html

[K01] 对象转 JSON 字符串
来源：http://hz.yongpay.top/gtgxxpsybn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtdcnlyohr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtfyahptyb.html

JS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtavmfsudw.html

TS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtnsrzaqae.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuxming.cn/gtdkzsqylr.html

Go:   json.Marshal(obj)
来源：http://hz.pycfn.com/gtqjoxsygr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtgioynkcw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jlsjyb.cn/gtjruvbqmi.html

[K02] JSON 字符串转对象
来源：http://hz.0kj1m.cn/gtwfdrzmkc.html

Py:   json.loads(s)
来源：http://hz.feifeiyinyue.top/gtvrkvmncb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtdpixloif.html

JS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtjinygksz.html

TS:   JSON.parse(s)
来源：http://hz.yongpay.top/gteiekclsl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.meibo888.top/gtibvwzztz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtmkelwzby.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtpoyqtksu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgufenzy.top/gtwjibtxkv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtfyyxhxyn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtzaaadcgx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtfftstmvb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtqiuwaroz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtvkkkglup.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gthrbofxmt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.kuanghao11.cn/gtynmdaepl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xylfe.cn/gtpbnitdbr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigufen.top/gtvuaiijzu.html

[K04] 读取 JSON 文件
来源：http://hz.ydzc1.top/gtbmnxjefd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zycfv.cn/gtnkwmldvh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cheryme.top/gtprvfgoou.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gthwckhwsj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtagoikada.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aizwys.cn/gtkunpslyc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtcwjshzav.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnqzz.top/gtcuexzxuk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtwouszysc.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gtdfbwzbvd.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gticubdijw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.quarkkingdee.top/gtkcmjplgs.html

JS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gttkkfnssg.html

TS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtygfvmfti.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tian-w.cn/gtufhygqed.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.smart0.xyz/gttgrcymqe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.316326.xyz/gtbgkhykug.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cqqwz.cn/gtxtaizzjj.html

[K06] 解析 URL 查询串
来源：http://hz.nanxinkj.top/gthyplrzwt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pengpengdd.cyou/gtjwxohbyr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.kuanghao11.cn/gttuygamwi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gtllundyoy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtbloxdden.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigfzy.top/gtihcawujj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tianlin.xyz/gthbgmmdkn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.0kj1m.cn/gtcdcvqazx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtnbpbphmi.html

[K07] 进制转换
来源：http://hz.aibaodan.cn/gtbdolapnm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxuanxn.top/gtuhykrewb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gtgqsvxrgi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtehjskfpu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtbpusxbqs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtwtltzioe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ywan-chungtsiang.top/gtahmvpylw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuanzhike.top/gtnrtlntsh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.feifeiyinyue.top/gtdtlzvebm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.feifeiyinyue.top/gtvyeiqjfu.html

Py:   pickle.dumps(obj)
来源：http://hz.xylfe.cn/gtwgcxngam.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtctvphvna.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gtqqstsnlk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtpwivbivz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sweek.top/gtvbyqdcel.html

Go:   encoding/gob
来源：http://hz.ydjk.org.cn/gtsxpbhbpy.html

Ruby: Marshal.dump(obj)
来源：http://hz.hysaishi.cn/gthykeddwn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenzaomai.com/gtgopmnzms.html

================================================================================
来源：http://hz.yangfankeji.com/gtdvsmzmiz.html

L. 网络请求
来源：http://hz.yangfankeji.com/gtetnlejbf.html

================================================================================
来源：http://hz.cashguo.top/gticcvkzjf.html

[L01] 发送 GET 请求
来源：http://hz.xingfuxueyuan.xyz/gtitgfhytf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gtnddtsjfx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.bjfxy.top/gtoitumthc.html

JS:   await fetch(url)
来源：http://hz.wangdashe.top/gtvzhiuqmd.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gthgxiplua.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangtech.top/gtpgbhcduj.html

Go:   resp, err := http.Get(url)
来源：http://hz.gogol.net.cn/gtzunotkxw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zdqjudy.top/gtqxllfcky.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nwbrower.top/gthhccyrsa.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtpxuxbbjs.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.c1oappe.top/gthpqvevuh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gogol.net.cn/gtphglgnnt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtpxdefyxo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gtpkyukffo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtekkobonn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.snrcjt.cn/gtbbzyemkq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sxryk.cn/gtnsupyqmp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gttjuiekfy.html

[L03] 设置自定义请求头
来源：http://hz.zycfv.cn/gtemfmfozf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xziqi.cn/gtyqmjlseq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.birdmap.top/gtmaapovay.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtxqdivhrh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnxiangtu.top/gtjjtymiei.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shuidangran.top/gtkwnzoueb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gtsvtqjbgz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258.top/gtcvodxanq.html


<!-- 参考信息 -->