代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtaoqdhyby.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ybcxt.top/gtauhpsbgz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxuanxn.top/gtdlpdlggt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgfzy.top/gthupigzkc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigufen.top/gtoeoufyev.html

[H08] 获取错误信息与堆栈
来源：http://hz.shangyingyoupin.top/gtywqngvdv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangkeji.top/gtsbdhryam.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jianghu66.top/gtmdclkdai.html

JS:   e.message;  e.stack
来源：http://hz.dianchejie.cn/gtkkoujvvl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yonumen.top/gtjkpyuuuk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ywan-chungtsiang.top/gtyydldbli.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtdqrohwmi.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtmjvxncxc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.feifeiyinyue.top/gtvrlxkmqj.html

[H09] 带错误码的异常
来源：http://hz.zycfv.cn/gtmgwpxcfg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tianlin.xyz/gtsmiuqqua.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtjgbnmoae.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenzaomai.com/gtsyppcguz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shzxlz.cn/gtxyoeqkma.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hysaishi.cn/gttjadgfpi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yongpay.top/gtxwofvuvn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgufenzy.top/gtxzoshjef.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gaohongyu789.top/gtzoalfskb.html

[H10] 资源自动释放
来源：http://hz.jinqigfzy.top/gtmwvovtpl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gotoacloud.top/gtdgpapygr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtqkjfpqex.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtehczpboc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtqkayyyut.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yongpay.top/gtfyaduurw.html

Go:   defer f.Close()
来源：http://hz.ehwqpu.com/gthusrgzvo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gteubekdlx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtvzyvvmwd.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjwpicvbx.html

I. 正则表达式
来源：http://hz.sufxvd.cn/gtvrwkkbue.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtuilfwilp.html

[I01] 判断是否匹配
来源：http://hz.gzhubu.top/gttuuapybp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.haohaochexian.top/gtcewekemb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hysaishi.cn/gtosesfcoj.html

JS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtqfylsanm.html

TS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtkpxmzsva.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shuidangran.top/gtiicfxszb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guowangkeji.top/gtclrfonma.html

Ruby: s.match?(/\d+/)
来源：http://hz.sxryk.cn/gtzwsozkxp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cheryme.top/gtwuurlbih.html

[I02] 提取所有匹配
来源：http://hz.cashguo.top/gtfnoxyuki.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shanyushiyangkeji.top/gtouhucfrt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jiagoushi.top/gtsbcvfrkx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cdnleiting.top/gtqyiopvhm.html

TS:   s.match(/\d+/g)
来源：http://hz.zhoulong.xyz/gtawdsmlvl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenzaomai.com/gtoiwniqzz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zycfv.cn/gtheyabsaz.html

Ruby: s.scan(/\d+/)
来源：http://hz.meibo888.top/gtjdwfteal.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gzhubu.top/gtxvrbejvh.html

[I03] 提取捕获分组
来源：http://hz.hfpthk.cn/gtbslwfbsx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yvedp.cn/gthtcsqntj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yangfankeji.com/gthhcxovyp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tianlin.xyz/gtjglsdpeq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgufenzy.top/gtdxyfqsbz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shzxlz.cn/gtnxwiaeot.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258.top/gtyyxhlksk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gogol.net.cn/gthcqrggep.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yueranfly.top/gtytjurtba.html

[I04] 正则替换
来源：http://hz.svipenyu.cn/gtohslfkaa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ybcxt.top/gtvasgsgxp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gthwqqiase.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gtoturxbcp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtotpfhfzl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jianghu66.top/gtkqqaseza.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuanzx.com/gtldzodrty.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jianghu66.top/gtvcwskege.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gtdbmoglvd.html

[I05] 按正则拆分
来源：http://hz.tian-w.cn/gtdkhxpsgd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yanxiufei.cn/gtqfrebwxs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shangyingyoupin.top/gtitvhznmk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtapsyuhpu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtykpadnyd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cqqwz.cn/gtgmywxnde.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydzc1.top/gthahizhbm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtacpqnshy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258.top/gtlooafihs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinyuanbaomall.cn/gtvdstwtsd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtxasqvfew.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.havefunace.top/gtpwvxledn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gtpicryaxe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gthhnkmmdk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.birdmap.top/gtxzijssui.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shuidangran.top/gtrjytblls.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yonumen.top/gtfdtlddqr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtufibhsgd.html

[I07] 忽略大小写与多行模式
来源：http://hz.cashguo.top/gtwtzkekuk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aibaodan.cn/gtsttlrjwi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtjttoitme.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtzdtlcmwa.html

TS:   /error/gim
来源：http://hz.jinqigufen.top/gtsvvhgcjq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gaohongyu789.top/gtmiqynlqt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yonumen.top/gtrsbwwooe.html

Ruby: s.scan(/error/i)
来源：http://hz.shuidangran.top/gtyhmhwljf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigufen.top/gtbtgtxfex.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gzhubu.top/gtrmrpsvfa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ywan-chungtsiang.top/gtfwrhslpp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenlongwang.top/gtkneazxbl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gttdcvlqxu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtqarlyucl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nwbrower.top/gtipyozrud.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigfzy.top/gttleiqtnw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.birdmap.top/gtszyrkexb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtsllacddz.html

================================================================================
来源：http://hz.yj20258888.top/gtyzlcjsqd.html

J. 日期与时间
来源：http://hz.andypj.xyz/gtoxxfgcri.html

================================================================================
来源：http://hz.cdnleiting.top/gtdjytkjha.html

[J01] 获取当前时间
来源：http://hz.chenjidiqi.icu/gtzoxdweln.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yueranfly.top/gtxspbehqd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtpscgcdzl.html

JS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtrgibyfbk.html

TS:   new Date();  Date.now()
来源：http://hz.guowangkeji.top/gtuvfngtse.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtzgwdbmdv.html

Go:   time.Now()
来源：http://hz.c1oappe.top/gtsmohtgzb.html

Ruby: Time.now
来源：http://hz.quarkkingdee.top/gtguxlqxrz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.meibo888.top/gtiatwwiff.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gtxrebnnur.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtqifnjetf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtbzzinzxf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pycfn.com/gtjwbazhrq.html

TS:   d.toISOString()
来源：http://hz.sxryk.cn/gtjbhpeeuy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ydjk.org.cn/gttuhuvzfv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gttsgllcbk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtnpkybzqy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pengpengdd.cyou/gtplvtxmoa.html

[J03] 字符串解析为日期
来源：http://hz.bjfxy.top/gthtbaqebf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gtojyxxylf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hysaishi.cn/gtesmckzyg.html

JS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtumavnzwo.html

TS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtbapjwobu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtzkwsttsh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gaohongyu789.top/gthohmvzwy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtknmvcour.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ivvv.top/gtfjokirey.html

[J04] 时间戳与日期互转
来源：http://hz.daxiang520.top/gtpxlmqirw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgfzy.top/gtutpmspqh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yonumen.top/gtgzxbysxn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gtllrfxnbl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jiagoushi.top/gtpdeezwlb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cqqwz.cn/gtjdaelxlz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ywan-chungtsiang.top/gtxblfzwvd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gtphbbiaop.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.havefunace.top/gtzroidfzp.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenjidiqi.icu/gtgktsskke.html

Py:   now + timedelta(days=7)
来源：http://hz.sxryk.cn/gtowvmljrp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daria6918.cn/gtpquvlwud.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gtvvcyweow.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtbweomhuv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shuidangran.top/gtolcezsrq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenlongwang.top/gtgbqzmkix.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ybcxt.top/gtpgtkvmxe.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.kuanghao11.cn/gthtdzolxc.html

[J06] 计算两时间之差
来源：http://hz.xuetiantiany.cn/gtklcktelq.html

Py:   (end - start).total_seconds()
来源：http://hz.daria6918.cn/gtpayezjca.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtjvliyjtk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.c1oappe.top/gtxhofgyqi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yueranfly.top/gthyvfzzjw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuetiantiany.cn/gtzkwfkqjn.html

Go:   end.Sub(start).Hours()
来源：http://hz.feifeiyinyue.top/gtxaldytiw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cdnleiting.top/gtlqqstxgf.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhijiandao.cn/gtzydsxzoz.html

[J07] 比较两个日期
来源：http://hz.wangshuangyany.cn/gtlomeuqen.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtucgwhrcl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zdqjudy.top/gtrjiashwr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtbzumavfg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtwqpmlhtk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.andypj.xyz/gtmxefcehm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jianghu66.top/gtbmsrwttn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtcvhujzfr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtvlopnrkp.html

[J08] 提取年月日与星期
来源：http://hz.ydzc1.top/gtcjzcnuln.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtlzkqchco.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zdqjudy.top/gttgchihvy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shzxlz.cn/gtpcxgjkzk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jianghu66.top/gtxylvcvyl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtmpifzymk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ivvv.top/gttkdgafym.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.smart0.xyz/gtqsenqhoq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.vqdsnc.cn/gtugfmmgge.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gtenfdksfn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhoulong.xyz/gtlrrrvjbp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cheryme.top/gtmdxpjfyl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtifvquhda.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtkhpjlsvp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ywan-chungtsiang.top/gttxkgzcqp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenjidiqi.icu/gtqxpqpmwk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ivvv.top/gtzyjhaksc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hysaishi.cn/gtmbzefnmc.html

[J10] 取今天 / 本月第一天
来源：http://hz.pycfn.com/gtspdosnhq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gthxgnagyc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jlsjyb.cn/gtnocbmolk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtoawkscuq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ybcxt.top/gthktfffpi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.haohaochexian.top/gtanpebpry.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shuidangran.top/gtiqrrnylm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhoulong.xyz/gtxuymtqty.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.pengpengdd.cyou/gtiogaezfg.html

================================================================================
来源：http://hz.yj202588.top/gtsldeaqrq.html

K. JSON 与序列化
来源：http://hz.sufxvd.cn/gthdpdgwfj.html

================================================================================
来源：http://hz.9152youxi.cn/gtjdsqtpzi.html

[K01] 对象转 JSON 字符串
来源：http://hz.hysaishi.cn/gtmjuratnf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtjmmixqsh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtovqgjrdi.html

JS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtdplioubk.html

TS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtrwvpihod.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigfzy.top/gttlsoeune.html

Go:   json.Marshal(obj)
来源：http://hz.jianghu66.top/gtzzakzubu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jlsjyb.cn/gtoadlffmr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jiagoushi.top/gtrbebtcma.html

[K02] JSON 字符串转对象
来源：http://hz.cheryme.top/gtccjutlsb.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gtdvjkrkim.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.0kj1m.cn/gttmexmhxr.html

JS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtbtqpvvtt.html

TS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtqibrrcfc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jyoumei.cn/gtuuugbevu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtyciyggyb.html

Ruby: JSON.parse(s)
来源：http://hz.bjfxy.top/gtcxdsihik.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtabxtuvay.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shangyingyoupin.top/gtoyimvlrz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtlpjtuwys.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtaqhvaloo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtbweztuyr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtgxjqyfdy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.316326.xyz/gtmiukkfbv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.kuanghao11.cn/gtajxvkhsm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.quarkkingdee.top/gtlfpygico.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sweek.top/gtvvnlyqfd.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigufen.top/gtqiybilgp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cheryme.top/gtithwlhtu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tian-w.cn/gtolfuuazs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtjiupajqa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtxsfeabmx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ppjwa.cn/gtluydexvx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gtconidwzj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangshuangyany.cn/gtlsbhmguy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuetiantiany.cn/gtuncawhhb.html

[K05] 深拷贝对象
来源：http://hz.dianchejie.cn/gtgagrhezb.html

Py:   copy.deepcopy(obj)
来源：http://hz.shuidangran.top/gtvnseyuts.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cheryme.top/gthsephkrp.html

JS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtnlrmxopw.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtbitwkzgy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.smart0.xyz/gtusyfqqcs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gtgmbbdxyf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xziqi.cn/gtapsioqpw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yanxiufei.cn/gtpekqspso.html

[K06] 解析 URL 查询串
来源：http://hz.ydzc1.top/gtnhatznzj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dashuyun.cn/gtkowvprxg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhengqikj.top/gtonixfzcw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gtpgbqdhof.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtxwpctnzo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.c1oappe.top/gtrotvaogh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gttlzwsgkz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jyoumei.cn/gtftvheoww.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gtwzkkbxhj.html

[K07] 进制转换
来源：http://hz.pycfn.com/gtbszwpqtj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuanzx.com/gtlhbaoizj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.birdmap.top/gtsutttrcu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtuvdnzlcu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtexijyfbm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtypfqmgwf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tian-w.cn/gtxzwzsjfg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtikixuswc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yvedp.cn/gtwwnntakr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuanzx.com/gthfuuuoft.html

Py:   pickle.dumps(obj)
来源：http://hz.redwolf501.top/gtlhpveupq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gtpqvcgdqq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtzlprwblp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtfrmxmocg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cdnleiting.top/gtwacgnwot.html

Go:   encoding/gob
来源：http://hz.meibo888.top/gtwhwwjbsu.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhijiandao.cn/gtuyyqhcal.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guowangkeji.top/gttknufmup.html

================================================================================
来源：http://hz.gotoacloud.top/gtptutptjt.html

L. 网络请求
来源：http://hz.feifeiyinyue.top/gtmyjbbtkm.html

================================================================================
来源：http://hz.snrcjt.cn/gtnawesnnb.html

[L01] 发送 GET 请求
来源：http://hz.cashguo.top/gtqcagerji.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhoulong.xyz/gtfnulobqa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pycfn.com/gthtuzytkr.html

JS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtogmazlru.html

TS:   await fetch(url)
来源：http://hz.yj20258.top/gtopmnwfzy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtxljyqlim.html

Go:   resp, err := http.Get(url)
来源：http://hz.gaohongyu789.top/gtksdhwzkb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shangyingyoupin.top/gtjwardhws.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gthywdppsz.html

[L02] 发送 POST JSON
来源：http://hz.yj20258.top/gtitfcvbgu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtinuvztso.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jyoumei.cn/gtjztiajbv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gtfcqwpvdt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gthxxzeosa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shzxlz.cn/gtwplbvvmy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jianghu66.top/gtnuofqexp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangshuangyany.cn/gtmxaveicp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shanyushiyangkeji.top/gtcylpsjuu.html

[L03] 设置自定义请求头
来源：http://hz.kuanghao11.cn/gtzmmtgdey.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gotoacloud.top/gtqzuwjedx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xylfe.cn/gttvfuolfl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtlpbovekf.html


<!-- 参考信息 -->