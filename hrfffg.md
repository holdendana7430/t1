代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtpcpqhela.html

[H08] 获取错误信息与堆栈
来源：http://hz.nanxuanxn.top/gtfswrydiy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhengqikj.top/gtwnghduwr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigfzy.top/gtcpmkkmhq.html

JS:   e.message;  e.stack
来源：http://hz.bjfxy.top/gtdexpioah.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.havefunace.top/gtuiobzhae.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenlongwang.top/gtstqzduvv.html

Go:   err.Error()
来源：http://hz.tian-w.cn/gtijjknnmc.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhaomingkeji.xyz/gtbbhinzia.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yangfankeji.com/gthcmllmow.html

[H09] 带错误码的异常
来源：http://hz.pengpengdd.cyou/gtlyovhdjr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jlsjyb.cn/gtpuhfkdrl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangshuangyany.cn/gtdyaglmin.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuanzx.com/gtwrlkecjn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj202588.top/gtcclnrbgc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jiagoushi.top/gtglnqthev.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtadbnmsen.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxinkj.top/gtxxmdctwh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gaohongyu789.top/gtrfenbhww.html

[H10] 资源自动释放
来源：http://hz.svipenyu.cn/gtsyehkjao.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.snrcjt.cn/gtqwfplolg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenlongwang.top/gtusnpcjlp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtnlolxyhf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtegnvjkzg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangshuangyany.cn/gtxywkdesw.html

Go:   defer f.Close()
来源：http://hz.yj202588.top/gtjtkytvgv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yonumen.top/gtcewhqwyu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gogol.net.cn/gtqcvomwkj.html

================================================================================
来源：http://hz.tianlin.xyz/gtrpsrhxop.html

I. 正则表达式
来源：http://hz.ywan-chungtsiang.top/gtxdjfhfli.html

================================================================================
来源：http://hz.nwbrower.top/gtqrtunegf.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gtemxkqbwr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gttbxaqtit.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgufenzy.top/gtplunrhsf.html

JS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gthezwbqcj.html

TS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gtztoklxnq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.vqdsnc.cn/gteyfdsxtm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhixingplan.top/gtdwfqziih.html

Ruby: s.match?(/\d+/)
来源：http://hz.yangfankeji.com/gtiumolllu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yonumen.top/gtxcvaljci.html

[I02] 提取所有匹配
来源：http://hz.ehwqpu.com/gtjldyphbu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258888.top/gttcgrytjm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangshuangyany.cn/gtcifuiroq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.52xcode.cn/gtlutagjxl.html

TS:   s.match(/\d+/g)
来源：http://hz.dashuyun.cn/gtfzwzkggr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yueranfly.top/gtbkpytdbq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxuanxn.top/gtcoxmnhkf.html

Ruby: s.scan(/\d+/)
来源：http://hz.snrcjt.cn/gtebcrncgt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cheryme.top/gtmiqzodji.html

[I03] 提取捕获分组
来源：http://hz.316326.xyz/gtefrxlvkn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guannengcc.top/gtynrbqyai.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj202588.top/gtgqdenpzm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ybcxt.top/gtjyxbxkyi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhengqikj.top/gtehmryait.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ivvv.top/gtlxieuwan.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtmkvwpxmy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gzhubu.top/gtkfcatpga.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shuidangran.top/gtuquogmal.html

[I04] 正则替换
来源：http://hz.ydjk.org.cn/gtqowlevjt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhijiandao.cn/gtgzpbixtu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sxryk.cn/gthljzpsxy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtyviqnyhm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gthydwqykh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yanxiufei.cn/gtglqtlglo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangdashe.top/gtcebkvmbf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yangfankeji.com/gtbnyeqxcl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yonumen.top/gtmnakfvib.html

[I05] 按正则拆分
来源：http://hz.zdqjudy.top/gtwehpkhds.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yanxiufei.cn/gtzekgmkel.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gtsixtavii.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gthavszrss.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtliakvldg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigfzy.top/gtnmjxfgbg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenlongwang.top/gtpvybgdhj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtxhqesnzr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangdashe.top/gtkbjpntzw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yangfankeji.com/gtscagziyt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtmqrhpeki.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nwbrower.top/gtvcsrsnri.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydzc1.top/gtnccxprgd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtxxegavau.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtvzgoqtqj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhixingplan.top/gttcdwgiqj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fzhhl.top/gtajrpakty.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtveuyslss.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtabezxvil.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuanzhike.top/gtpapxrmfi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hammf.cn/gtswgvvxkt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258888.top/gtuxszxwqw.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtrdvpvtrm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aibaodan.cn/gtzlozcolr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuanzhike.top/gtamctybeq.html

Ruby: s.scan(/error/i)
来源：http://hz.cqqwz.cn/gtkelyltuy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.vqdsnc.cn/gtrilumdvb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yangfankeji.com/gtgxsjgpfp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daria6918.cn/gtsslrnakn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtbwnlitxb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtoajwewmi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtpofulcmx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtgfwrkxyl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daxiang520.top/gtvhoopnho.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cucudq.cn/gtzfufgfws.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtxvgtvmht.html

================================================================================
来源：http://hz.meibo888.top/gtguaxolkg.html

J. 日期与时间
来源：http://hz.haohaochexian.top/gtphgzvlih.html

================================================================================
来源：http://hz.zhoulong.xyz/gtsnhnmrqk.html

[J01] 获取当前时间
来源：http://hz.cqqwz.cn/gtvjsebomy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnxiangtu.top/gtgeqrbrtm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtneyxbfdm.html

JS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtkwcwdhun.html

TS:   new Date();  Date.now()
来源：http://hz.meibo888.top/gtbgdbbzia.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jianghu66.top/gtavocucph.html

Go:   time.Now()
来源：http://hz.sweek.top/gttqjkvydy.html

Ruby: Time.now
来源：http://hz.chenzaomai.com/gtjxaqhobu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tanke756.top/gtegxvnroa.html

[J02] 格式化输出
来源：http://hz.hfpthk.cn/gtrmockmrt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtmhsnxogz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtdxsgimof.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gttfrhyaav.html

TS:   d.toISOString()
来源：http://hz.xuanzx.com/gtjjldrkph.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.smart0.xyz/gttrjezfsw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gtssdfuajc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtwjtsmnan.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtnpufmlzp.html

[J03] 字符串解析为日期
来源：http://hz.jyoumei.cn/gtniqkflcl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtjvvytcpp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangkeji.top/gtaivueazz.html

JS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtlzohydfy.html

TS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtjqxpfnfq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtocfalrnx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gzhubu.top/gtioolzits.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtbyannyhq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinghuilouyu.cn/gthuavatyp.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtnfunzzfe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhaomingkeji.xyz/gtwopkzrwx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.52xcode.cn/gtwppdonrx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.feifeiyinyue.top/gtnhwjenwy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.andypj.xyz/gtgvmwtvyt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinyuanbaomall.cn/gthhqhhkdu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.vqdsnc.cn/gtagyeuftx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.aibaodan.cn/gtzodygmog.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinyuanbaomall.cn/gtgfdwwhab.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gtsagbqqgf.html

Py:   now + timedelta(days=7)
来源：http://hz.xingfuxueyuan.xyz/gtbnxvtfbw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhoulong.xyz/gtmzecyzck.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtzjeekijq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtxmljkamb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daria6918.cn/gtydfdavwo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gzhubu.top/gtrclfwwot.html

Ruby: Time.now + 7 * 86400
来源：http://hz.meibo888.top/gtzrwreinn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gturjcpspm.html

[J06] 计算两时间之差
来源：http://hz.c1oappe.top/gtmqtxnmiy.html

Py:   (end - start).total_seconds()
来源：http://hz.sufxvd.cn/gtaydfqgwx.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtwrlkpeyp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.haohaochexian.top/gtbnnndjhn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xinyue.icu/gttitnpoid.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guannengcc.top/gtfazvpgnh.html

Go:   end.Sub(start).Hours()
来源：http://hz.yangfankeji.com/gtjayuagda.html

Ruby: end - start                 # 返回秒数
来源：http://hz.haohaochexian.top/gtnupvjtxa.html

C#:   (end - start).TotalSeconds
来源：http://hz.birdmap.top/gtuqiirvju.html

[J07] 比较两个日期
来源：http://hz.wangshuangyany.cn/gtubssitfa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtcofltlio.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gtxflxrjtf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtxllihknm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gtzpgkckmt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtwldriwby.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sxryk.cn/gtqptvrmnc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtgwjbvhub.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gttrzsjnjo.html

[J08] 提取年月日与星期
来源：http://hz.smart0.xyz/gtnqmgwkwx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtuxdflzev.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinyuanbaomall.cn/gteoasazjt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zycfv.cn/gtjvgzcrff.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuxming.cn/gtinletbzc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtpzzjftzh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.52xcode.cn/gtbripuilb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yvedp.cn/gtsxscrjpx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.feifeiyinyue.top/gtxpclxpyu.html

[J09] 时区处理
来源：http://hz.redwolf501.top/gtjdimfmrb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinghuilouyu.cn/gttedxemhy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhijiandao.cn/gtjbdbtzkc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gttnpybzmv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtnrjkvhdm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shanyushiyangtech.top/gtutsivxme.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gzhubu.top/gtkpctiocu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhoulong.xyz/gttdzapdxh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtaobxlfit.html

[J10] 取今天 / 本月第一天
来源：http://hz.ywan-chungtsiang.top/gtdequitfe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.0kj1m.cn/gtytzmxocm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yueranfly.top/gtlltzsulw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zdqjudy.top/gtcfyegkua.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.svipenyu.cn/gtcxeatzbx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cqqwz.cn/gtgauciybk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aizwys.cn/gtmhtrybfl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigfzy.top/gtaumskvog.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtktbelees.html

================================================================================
来源：http://hz.dianchejie.cn/gthaiecqhz.html

K. JSON 与序列化
来源：http://hz.zhijiandao.cn/gtxpsafvmm.html

================================================================================
来源：http://hz.cheryme.top/gtdasijyum.html

[K01] 对象转 JSON 字符串
来源：http://hz.cdnleiting.top/gtlbscpbau.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtuyundyyd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtqvrmtaat.html

JS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gttcbuukzg.html

TS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtpijumaww.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenlongwang.top/gtwhvaluvx.html

Go:   json.Marshal(obj)
来源：http://hz.gzhubu.top/gtsxfujnle.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gtpnakcbdf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.snrcjt.cn/gtxpofhntb.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258.top/gthhfcmuvi.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangtech.top/gtsvssoyoo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jyoumei.cn/gtanunsodb.html

JS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gthcfgmkus.html

TS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtgumsarwq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.guowangkeji.top/gteirxygfo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtxsmbsatn.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtuctvtxfc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtaxpcwpro.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pycfn.com/gtgpolzxhv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtosqczrgo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtrjfspaif.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtmrowkjtp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtnnmvpugu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ehwqpu.com/gtgrwyuxet.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daria6918.cn/gtqtjvyraz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtriwgalto.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuetiantiany.cn/gtcvvqlpiq.html

[K04] 读取 JSON 文件
来源：http://hz.shuidangran.top/gtxwsuhbfj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aizwys.cn/gthojinell.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yonumen.top/gtznriryue.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtpqpnmibe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtvyqnldim.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.kuanghao11.cn/gtdcavfyqg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gtuhpfvxzq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258.top/gtrduhoilk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtdejqjrxy.html

[K05] 深拷贝对象
来源：http://hz.kuanghao11.cn/gttuasfycy.html

Py:   copy.deepcopy(obj)
来源：http://hz.tianlin.xyz/gtgbptvlna.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenzaomai.com/gttgzoglld.html

JS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtkuupsxez.html

TS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtengnbobs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gtzipavnyq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.wangdashe.top/gthtnphnlc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.andypj.xyz/gtmkstynrx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.mhx1999.top/gtwshlncgj.html

[K06] 解析 URL 查询串
来源：http://hz.xinyue.icu/gtepqmnwkz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtsymvxetj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sysykeji.top/gtqzjujmly.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gtxgtcqvwn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtvythpcta.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxuanxn.top/gtiaunyzzf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtkesqpyrw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtngngspxa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuanzhike.top/gtyscupjay.html

[K07] 进制转换
来源：http://hz.gaohongyu789.top/gtqszcrfid.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gtfmeqthpb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jiagoushi.top/gthxfucoij.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtdtyavjxz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtokytmlhl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtivlaibym.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.kuanghao11.cn/gtoflaxulr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxinkj.top/gtjzashcmo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sufxvd.cn/gtztukrpda.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gtitxwwbmv.html

Py:   pickle.dumps(obj)
来源：http://hz.xuanzx.com/gtlrbsnwnn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gzhubu.top/gtoxibongi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtncsdrgtm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gthwlmcdaw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtohvqanva.html

Go:   encoding/gob
来源：http://hz.hongshengwenyu.top/gtlkujkwsw.html

Ruby: Marshal.dump(obj)
来源：http://hz.guowangkeji.top/gtakszczyf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtoarnmvzm.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtlidzedev.html

L. 网络请求
来源：http://hz.gaohongyu789.top/gtngxvyjmy.html

================================================================================
来源：http://hz.fengsongda.top/gtcbomgxqj.html

[L01] 发送 GET 请求
来源：http://hz.yvedp.cn/gtggkltrjj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hywenlv.cn/gtijzkhypv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ivvv.top/gttgstxlgk.html

JS:   await fetch(url)
来源：http://hz.hnqzz.top/gtoqxvwszk.html

TS:   await fetch(url)
来源：http://hz.yuxming.cn/gtcetllwxb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cashguo.top/gtoiceanxw.html

Go:   resp, err := http.Get(url)
来源：http://hz.aizwys.cn/gtckfauuzb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.9152youxi.cn/gtevampjtn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenjidiqi.icu/gtznkiwery.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gteunztttq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gtldatlrcg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shanyushiyangtech.top/gtefhxbjpi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtwllaqzux.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtpyjhlugn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.0kj1m.cn/gtauwvhngs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cqqwz.cn/gtxuovhear.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.svipenyu.cn/gtkmxczmxn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gzhubu.top/gtuqqwdrgj.html

[L03] 设置自定义请求头
来源：http://hz.jqgufenzy.top/gtiatsyapm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnxiangtu.top/gtjjoivnce.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nwbrower.top/gtoipaetrr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtkiegfzvo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fengsongda.top/gtavtrjvjt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtknxjxuuo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gtbydztxcq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtcuomurzc.html


<!-- 参考信息 -->