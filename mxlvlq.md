代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhiwuduotai.top/gtjsuydyju.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenlongwang.top/gtkuakchud.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgfzy.top/gtbermhdju.html

C#:   obj?.A?.B ?? default
来源：http://hz.zycfv.cn/gtpbsayyfg.html

[H07] 断言
来源：http://hz.yj202588.top/gtkwkjtvch.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xylfe.cn/gtnbfatqgv.html

PHP:  assert($x > 0);
来源：http://hz.xylfe.cn/gtafhipleb.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtgonhnhoo.html

TS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtfzononwl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.redwolf501.top/gteubadjzi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhijiandao.cn/gtuvtlkcsy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenzaomai.com/gtatczjjot.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gtvjgtdkpr.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangshuangyany.cn/gtpbfliqao.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtbfszpbfu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sxryk.cn/gtrbtzxvus.html

JS:   e.message;  e.stack
来源：http://hz.fzhhl.top/gtkdwovwca.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yongpay.top/gtebdhnddu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gotoacloud.top/gtrudgyvej.html

Go:   err.Error()
来源：http://hz.pycfn.com/gtikqimnqs.html

Ruby: e.message;  e.backtrace
来源：http://hz.gogol.net.cn/gtqgwxziqm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhengqikj.top/gtzvgkybej.html

[H09] 带错误码的异常
来源：http://hz.jyoumei.cn/gtheabherq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daxiang520.top/gtrcievbpj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zycfv.cn/gtmyssytxj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.smart0.xyz/gtudvztlds.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgufenzy.top/gtbomroenb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gtyeyyatpp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daxiang520.top/gtzijtbfql.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gogol.net.cn/gtqracqhzp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sufxvd.cn/gthvzwsszy.html

[H10] 资源自动释放
来源：http://hz.quarkkingdee.top/gtryeihbbt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenzaomai.com/gtyfzosgyg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhongyouzk.top/gtmgewajhl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtsoqqwffd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtzicmqyzn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.iojbl.cn/gtakavdfuq.html

Go:   defer f.Close()
来源：http://hz.zhengqikj.top/gtfydrjmzv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangkeji.top/gtnsadiyye.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.haohaochexian.top/gtthzulbaw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gteqqxtjak.html

I. 正则表达式
来源：http://hz.dianchejie.cn/gtwwrytgph.html

================================================================================
来源：http://hz.xziqi.cn/gtktgfqfpz.html

[I01] 判断是否匹配
来源：http://hz.chenlongwang.top/gtjqquikxz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258.top/gtrmdjdwqb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtebvitgvo.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gteyzrtwcm.html

TS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtysqncmwq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sxryk.cn/gtpulwqvpv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pengpengdd.cyou/gtsgkwovod.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangtech.top/gthyuqqmmb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gaohongyu789.top/gtzmifpcml.html

[I02] 提取所有匹配
来源：http://hz.ppjwa.cn/gtlhibkclc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.wangshuangyany.cn/gtfdygxfut.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxinkj.top/gtvqolfdno.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.birdmap.top/gtxoqfnkdm.html

TS:   s.match(/\d+/g)
来源：http://hz.zhijiandao.cn/gteejfpljq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangdashe.top/gtkstwpida.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pengpengdd.cyou/gtbckktxkm.html

Ruby: s.scan(/\d+/)
来源：http://hz.jianghu66.top/gtknqgotey.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daxiang520.top/gtdgobiscp.html

[I03] 提取捕获分组
来源：http://hz.sxryk.cn/gthjjtipdj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pengpengdd.cyou/gtjmkpmkxv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtepxltebr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.svipenyu.cn/gttnluvaiy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jlsjyb.cn/gthjjvixhf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.quarkkingdee.top/gtkdzpewsc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtivwyhrqx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yuxming.cn/gtrflumwcp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cdnleiting.top/gtjnjdlmxv.html

[I04] 正则替换
来源：http://hz.aibaodan.cn/gtvdjgnjoa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.quarkkingdee.top/gtyvcndyje.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gteglnqgml.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtdzkqfmbi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtpklyxiud.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yvedp.cn/gtbwzzdgnr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtdibnrddd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.9152youxi.cn/gtliqbiulj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cucudq.cn/gteyyjdyti.html

[I05] 按正则拆分
来源：http://hz.zhaomingkeji.xyz/gtmghnvvnm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gttqncaprx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.haohaochexian.top/gtbulcvcso.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtxdovlvld.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtkvhpsdwe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhengqikj.top/gtcxrvgqrw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yanxiufei.cn/gtxpgtuuna.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtppyuarpl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gtgxdkshcy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgfzy.top/gtpmxqgwlz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtewksodym.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnqzz.top/gtikapjwgj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtmdfuzgxm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gttgeyluon.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hywenlv.cn/gtdlalaiah.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yonumen.top/gtptiqtdvw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhiwuduotai.top/gtripdawza.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gturiyunrb.html

[I07] 忽略大小写与多行模式
来源：http://hz.fengsongda.top/gtnafxkhax.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.birdmap.top/gttygdjslj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.52xcode.cn/gtpbwmulet.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yvedp.cn/gtipcoewhp.html

TS:   /error/gim
来源：http://hz.mhx1999.top/gtiainkyqy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hfpthk.cn/gtxjdghhtm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangkeji.top/gtcypvfwhz.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gtyubxmxeg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shuidangran.top/gtpkuemrdw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sysykeji.top/gtqmhwrkgl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangdashe.top/gtfsgbkzsa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.haohaochexian.top/gtlxjhwvzo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gthdwgagwe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtduxovmlk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zycfv.cn/gtbdmpxfgo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhiwuduotai.top/gtdkikvymo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtvhduhgnm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtppqwxqzb.html

================================================================================
来源：http://hz.gzhubu.top/gtlcbzzctt.html

J. 日期与时间
来源：http://hz.chenzaomai.com/gtwetifrkn.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnyimbowz.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtpwmlgohx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.52xcode.cn/gtmuvpkjor.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gtllthsmqf.html

JS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gthfvyzydx.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtelipslqp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jiagoushi.top/gtwllqqisp.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtmgarsuab.html

Ruby: Time.now
来源：http://hz.quarkkingdee.top/gtfruehfih.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sufxvd.cn/gtvriievuv.html

[J02] 格式化输出
来源：http://hz.ydzc1.top/gtiruziero.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gtndgcenpg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtlqfwixoe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj202588.top/gtbedupwim.html

TS:   d.toISOString()
来源：http://hz.yongpay.top/gtdhcrtuub.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtmcnmmsfv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gogol.net.cn/gtlzphoysk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtnveccykk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhengqikj.top/gtcaggamfo.html

[J03] 字符串解析为日期
来源：http://hz.ppjwa.cn/gtnzfgywss.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.0kj1m.cn/gtruzvfulc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.9152youxi.cn/gtjucxgvpi.html

JS:   new Date("2024-01-02")
来源：http://hz.cashguo.top/gtoupmflnn.html

TS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gttgdgmync.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtzneczrva.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtzkglroyo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtlwwctdbw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.andypj.xyz/gtwcwmigsc.html

[J04] 时间戳与日期互转
来源：http://hz.cashguo.top/gtgehvfkol.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.aibaodan.cn/gthiiytgls.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxinkj.top/gtcjxqdacp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hongshengwenyu.top/gtiyextunv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtkqrobmoj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jyoumei.cn/gtrgnubqyy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.smart0.xyz/gthnurfoog.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.feifeiyinyue.top/gtcegqoakq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gogol.net.cn/gtvkopsdbm.html

[J05] 时间加减（加 7 天）
来源：http://hz.sysykeji.top/gtgrlsebqb.html

Py:   now + timedelta(days=7)
来源：http://hz.redwolf501.top/gtdpddxfkx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.0kj1m.cn/gtkxtmdvbp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtealueekg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtmsqfcruo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtgistoalf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gtuxigyhqc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenzaomai.com/gtxeummxqy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.guowangkeji.top/gtlnvzvbfd.html

[J06] 计算两时间之差
来源：http://hz.xuetiantiany.cn/gtyqgvwmhy.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigufen.top/gtkvkophuk.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuanzhike.top/gtprcomebe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cashguo.top/gtftwpxnka.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tanke756.top/gtxddlpahp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dianchejie.cn/gteqvlyngf.html

Go:   end.Sub(start).Hours()
来源：http://hz.shuidangran.top/gtmxcmybdz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.52xcode.cn/gtzhnofwvy.html

C#:   (end - start).TotalSeconds
来源：http://hz.xylfe.cn/gtgcsdiplp.html

[J07] 比较两个日期
来源：http://hz.ywan-chungtsiang.top/gtmxzorhwr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gttwztjrqw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aizwys.cn/gtksrxvkpv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtfidqjjlp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtrzwzfjzh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ybcxt.top/gtvphrlqai.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sysykeji.top/gtfefkzqpy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtdoiqhxwj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtolypfdcp.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtfaekjsud.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtipznpwgc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangkeji.top/gtgurclxyl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuxming.cn/gtcbzcccbu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cashguo.top/gtnvfcplkt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnqzz.top/gtlajzfktm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.meibo888.top/gtdlqijdwq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aizwys.cn/gtoqbcryut.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.52xcode.cn/gtxibpjhqf.html

[J09] 时区处理
来源：http://hz.hywenlv.cn/gtpsrtmidn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yvedp.cn/gtwihzwypu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hnqzz.top/gthdvtzgtq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtrdtxzlgf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtnhsufzox.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yongpay.top/gtwaiqanxo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xziqi.cn/gtecfgvvna.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.vqdsnc.cn/gtzfafamku.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.c1oappe.top/gttlakweym.html

[J10] 取今天 / 本月第一天
来源：http://hz.hammf.cn/gtitsdpane.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhoulong.xyz/gtjdkzkxfl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gzhubu.top/gtldtnimzy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxuanxn.top/gtztbkskih.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtuzrqzzvb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zdqjudy.top/gtsdynujyl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.daria6918.cn/gtrdyuscmq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gotoacloud.top/gtjdvfznqh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yvedp.cn/gtihkekltm.html

================================================================================
来源：http://hz.nanxinkj.top/gtwqcohzyg.html

K. JSON 与序列化
来源：http://hz.ivvv.top/gtvmprtxrg.html

================================================================================
来源：http://hz.redwolf501.top/gtukbnoodg.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhengqikj.top/gtjfrjnknr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cashguo.top/gthpywtwxx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtvwupymwa.html

JS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtqvktueif.html

TS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gttvygapad.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fengsongda.top/gthgsskpjf.html

Go:   json.Marshal(obj)
来源：http://hz.ehwqpu.com/gtshhvqmab.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yangfankeji.com/gtbynmrndr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ybcxt.top/gtpxkhzcrf.html

[K02] JSON 字符串转对象
来源：http://hz.cdnleiting.top/gtrovrgwfi.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtortjdkcp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sysykeji.top/gtewegzcbv.html

JS:   JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtpyaututy.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtnkatqfcr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cucudq.cn/gtdvkqsgyy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtvpvtrovn.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigufen.top/gtyjuqxcaa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gttjdmsvao.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pycfn.com/gtudqgdijo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.andypj.xyz/gtwzrhuunt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtgwzyveke.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtmufctsmd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtqoatiqhx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gtbeympuwh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cucudq.cn/gtwftygeli.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhongyouzk.top/gtgkwfcare.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtxybtkgpp.html

[K04] 读取 JSON 文件
来源：http://hz.cucudq.cn/gthrcohciq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenzaomai.com/gtypqycrkk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yuanzhike.top/gtexfqzpks.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sweek.top/gtxgygjrqu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtlihuibob.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenlongwang.top/gtfjcoeeuc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtndsygiww.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gtmwljlnlj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sweek.top/gtqgrbltzc.html

[K05] 深拷贝对象
来源：http://hz.gaohongyu789.top/gtlskyfaat.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangtech.top/gtmicnwruf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yanxiufei.cn/gtubnwhzkq.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gtkkultdyd.html

TS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtlxuesbqd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gtrzpsjswl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnxiangtu.top/gtgskhjnyn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.iojbl.cn/gtvuyshefn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xingfuxueyuan.xyz/gtdtjelbep.html

[K06] 解析 URL 查询串
来源：http://hz.sweek.top/gtfstmwnht.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigufen.top/gtdijiuwyf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gtscczjbyi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gthpzpmwdj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gtbaxqfteo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangdashe.top/gthlqocxul.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.birdmap.top/gtlcwyrabg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtqwvzgjzr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtuuyjtphi.html

[K07] 进制转换
来源：http://hz.nanxuanxn.top/gtbzulhtbd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gtrrlimuzt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.smart0.xyz/gtppheugud.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtirlzouvn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtfcsaztcl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtnpbzhcyx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtqgnutyad.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydjk.org.cn/gtulieafge.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pengpengdd.cyou/gtnzbbmfmt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.feifeiyinyue.top/gteamolzqk.html

Py:   pickle.dumps(obj)
来源：http://hz.yj202588.top/gtrqzsffve.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jyoumei.cn/gtrqqweowi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gtihajyjfc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtdeacnjrw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hongshengwenyu.top/gtfymyghvd.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gtdgfhuecs.html

Ruby: Marshal.dump(obj)
来源：http://hz.gogol.net.cn/gthrapnoqq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhaomingkeji.xyz/gtsiraldei.html

================================================================================
来源：http://hz.daria6918.cn/gtigaxqlmd.html

L. 网络请求
来源：http://hz.xziqi.cn/gtrflqmjdo.html

================================================================================
来源：http://hz.dianchejie.cn/gtqtyzxacz.html

[L01] 发送 GET 请求
来源：http://hz.jiagoushi.top/gtcstohyhj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gtktwvrpwt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydjk.org.cn/gthadmidnc.html

JS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtffnypbdo.html

TS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtksczxbtu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.haohaochexian.top/gtmypcgcse.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtkkitljnn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gtwegvccsf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dianchejie.cn/gtrgqzuanc.html

[L02] 发送 POST JSON
来源：http://hz.yj20258.top/gtosrxqvrk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.andypj.xyz/gtpjwtqoby.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gtjazxrlqk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtzilogbwm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtjoyuvznd.html


<!-- 参考信息 -->