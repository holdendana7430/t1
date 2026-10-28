代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.vqdsnc.cn/gtszganafl.html

[H08] 获取错误信息与堆栈
来源：http://hz.jiagoushi.top/gtgpllkevv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258888.top/gtcywnmjfo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daria6918.cn/gteznafxkx.html

JS:   e.message;  e.stack
来源：http://hz.yuxming.cn/gttagjsbyq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgfzy.top/gtvmibjjuy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.feifeiyinyue.top/gthzhmbsez.html

Go:   err.Error()
来源：http://hz.yvedp.cn/gtvqpqrtey.html

Ruby: e.message;  e.backtrace
来源：http://hz.hfpthk.cn/gtncvxxyec.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhengqikj.top/gtmzzlhxhk.html

[H09] 带错误码的异常
来源：http://hz.ehwqpu.com/gtwbsparlj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.c1oappe.top/gtidmymkoh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pycfn.com/gtmrlocpfh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.daria6918.cn/gtwkuitkhm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gtgyvkabwp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aibaodan.cn/gtwygkqkgt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.andypj.xyz/gtkknaebba.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ppjwa.cn/gtwdbfmoqb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenzaomai.com/gtmpubmcon.html

[H10] 资源自动释放
来源：http://hz.sweek.top/gtctyhjhow.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tian-w.cn/gteuxnnveg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.haohaochexian.top/gtcnzwhclc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtmgaaakux.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtpferlhie.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aizwys.cn/gthqztjwds.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gtwjwexqlm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.52xcode.cn/gttambbbbv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yueranfly.top/gtfngsqlld.html

================================================================================
来源：http://hz.dashuyun.cn/gtyrzsqcny.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtzlznbkkn.html

================================================================================
来源：http://hz.ydzc1.top/gtxvojfokv.html

[I01] 判断是否匹配
来源：http://hz.jianghu66.top/gtwzdzdocn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ybcxt.top/gttvyqlkjw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuxming.cn/gtidsschdb.html

JS:   /\d+/.test(s)
来源：http://hz.meibo888.top/gtzyopslci.html

TS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtxzgqglpx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fengsongda.top/gtxmifsyoq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hfpthk.cn/gtxbddexbb.html

Ruby: s.match?(/\d+/)
来源：http://hz.snrcjt.cn/gtnyfngdvs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yueranfly.top/gtanyozcyb.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtglrhrahe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sweek.top/gtxmiedkjb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtgjarswkq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jyoumei.cn/gttxnanarl.html

TS:   s.match(/\d+/g)
来源：http://hz.316326.xyz/gtobwhweet.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtrprloeus.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.316326.xyz/gtbfjipyhl.html

Ruby: s.scan(/\d+/)
来源：http://hz.daria6918.cn/gttgupbncw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.meibo888.top/gtiybcegww.html

[I03] 提取捕获分组
来源：http://hz.chenjidiqi.icu/gtamntbvnm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258888.top/gtgavfomne.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.316326.xyz/gthzmtvnfp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daxiang520.top/gtbmfvmocf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gtzjbbsgav.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhijiandao.cn/gtxwhcerdp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.mhx1999.top/gtnkpbmyyn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258.top/gtrhrgivqn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ivvv.top/gtmwvnhxqm.html

[I04] 正则替换
来源：http://hz.nanxuanxn.top/gtjhoanpgc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gttvpqtrcr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtklgpphja.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtncmfgddn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtuklsljab.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sxryk.cn/gtxsslxuhu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.smart0.xyz/gtgcpjlphb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daxiang520.top/gtnrqwqzkb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangdashe.top/gtedbsflpf.html

[I05] 按正则拆分
来源：http://hz.zhijiandao.cn/gtgibvthsy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.redwolf501.top/gtzacpzkbj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.meibo888.top/gtbqivwmdy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtnnkredby.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtgoehoyer.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenzaomai.com/gtmyajxzox.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtlqsfjyhf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtfkbuoazz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtlxbbuljx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hongshengwenyu.top/gtuexjfqfd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtiwydwlyl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daxiang520.top/gtwvdsiuus.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtvulcdezn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtpvgxwzlj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhoulong.xyz/gtxqgajnue.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.dianchejie.cn/gtzgetatmm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhoulong.xyz/gtdaqcmhrj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtaihomblg.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigufen.top/gtwflquqlb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tian-w.cn/gtimvkygau.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yongpay.top/gtfvtdqglj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daxiang520.top/gthwvoyidl.html

TS:   /error/gim
来源：http://hz.zhoulong.xyz/gthfuvlehu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.316326.xyz/gtunidyuxn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xinyue.icu/gtsfhxzryp.html

Ruby: s.scan(/error/i)
来源：http://hz.cqqwz.cn/gthmfdvbmy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cucudq.cn/gtbljeyzyc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nwbrower.top/gtxemuqzwu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhaomingkeji.xyz/gtnbpwyibd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hfpthk.cn/gtprzfxfsg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtbydwtyel.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtdvfygeyp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtihxizmps.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gttstfkwdl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.bjfxy.top/gtdgmaanae.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sweek.top/gtfucbynvq.html

================================================================================
来源：http://hz.tianlin.xyz/gtrvslmqzg.html

J. 日期与时间
来源：http://hz.gotoacloud.top/gtxgzwigdc.html

================================================================================
来源：http://hz.hywenlv.cn/gthjhesuiz.html

[J01] 获取当前时间
来源：http://hz.bjfxy.top/gthgkhrpjc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aizwys.cn/gtqtbwfdxx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtrosulamj.html

JS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gtwcuqgtnr.html

TS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtjltgfbsr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tian-w.cn/gtrxlhkwtd.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gtqmnfqenx.html

Ruby: Time.now
来源：http://hz.mhx1999.top/gtjqewdaxt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.redwolf501.top/gtjkazsnhv.html

[J02] 格式化输出
来源：http://hz.aibaodan.cn/gtlxsitgxo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtvgeskcvf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtcfavsbbe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnxiangtu.top/gthsccwgoc.html

TS:   d.toISOString()
来源：http://hz.yj20258888.top/gtxcxoqjeq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.smart0.xyz/gttrskukky.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guowangkeji.top/gtjlkciirn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtxwonufzz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jianghu66.top/gtwlmotdku.html

[J03] 字符串解析为日期
来源：http://hz.hfpthk.cn/gteybxxwlb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gzhubu.top/gtfgnwtljg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.havefunace.top/gtysjkvrdm.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtisziwjeo.html

TS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtpaqfanmq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtjguhsezc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tian-w.cn/gtjylpvybx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gttudzpkoq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.feifeiyinyue.top/gtulsybxbw.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtgnwfhrvx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.aibaodan.cn/gtcryawgwt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gtowraqizx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cucudq.cn/gtbymxtdii.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.52xcode.cn/gtjyvmovxb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangtech.top/gthppfcxfm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.vqdsnc.cn/gtcokuyduv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenlongwang.top/gtpgcfybvk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhiwuduotai.top/gtbeoadwwu.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhixingplan.top/gtmdcdqnzr.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gtbiukzxpg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guowangkeji.top/gtbkbtoyow.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenjidiqi.icu/gtsdgirvxm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gtcmbbpntw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tianlin.xyz/gtxpjybtbt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.andypj.xyz/gtifzmjayc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tian-w.cn/gtdigspjew.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtoitovrzh.html

[J06] 计算两时间之差
来源：http://hz.aizwys.cn/gttmjtgrnu.html

Py:   (end - start).total_seconds()
来源：http://hz.tianlin.xyz/gtqycuuawk.html

PHP:  $end->diff($start)->days;
来源：http://hz.shangyingyoupin.top/gtbkdwphzx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gotoacloud.top/gtgumszdqf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xylfe.cn/gteueingiz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhixingplan.top/gtfwaddsjw.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gttnhwwpfy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtxnjqmhmb.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258888.top/gtwzdpxdnv.html

[J07] 比较两个日期
来源：http://hz.aizwys.cn/gtquqsjyao.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtrxsdwnuy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hywenlv.cn/gtluklpwsa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtwryndidl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtqetxleck.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jiagoushi.top/gttayddvpz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xziqi.cn/gtkfsjoayg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtqsftnyxu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtwtmdnqdm.html

[J08] 提取年月日与星期
来源：http://hz.sweek.top/gtqrtxfjbf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtcfwsbrvh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dashuyun.cn/gtnkpgheun.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fzhhl.top/gtdfdzvkiz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gzhubu.top/gtwbwjadfq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtcaplhwko.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhijiandao.cn/gtfccqwbqx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sysykeji.top/gtttriabbu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.svipenyu.cn/gtjvazhnas.html

[J09] 时区处理
来源：http://hz.chenzaomai.com/gtuabzmcxz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangtech.top/gtqggavlqg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shuidangran.top/gtkizrmdah.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtqykzxver.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtwnbyyijj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nwbrower.top/gtydnjoxsy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.wangdashe.top/gtpqnmxpzv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhaomingkeji.xyz/gtxobshkmn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.birdmap.top/gtmqpkedvv.html

[J10] 取今天 / 本月第一天
来源：http://hz.ppjwa.cn/gtspdzdevl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtssxklwbg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenzaomai.com/gteghxddlb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj202588.top/gtkfnwylve.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gogol.net.cn/gtqnostudl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangdashe.top/gtwaefehan.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yanxiufei.cn/gtsrntisnq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhixingplan.top/gtwvzhwtdc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhengqikj.top/gtzabclsrw.html

================================================================================
来源：http://hz.mhx1999.top/gtbanfkaoc.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtisxkqabk.html

================================================================================
来源：http://hz.yueranfly.top/gtkzsuzhzs.html

[K01] 对象转 JSON 字符串
来源：http://hz.shangyingyoupin.top/gtjlkvtqci.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtdnzfqtbj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtmkcewdmr.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtzwbbabue.html

TS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gthvickmzt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cdnleiting.top/gtolrkeagz.html

Go:   json.Marshal(obj)
来源：http://hz.ydjk.org.cn/gtkkioylwg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hfpthk.cn/gtexqzfnvs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.haohaochexian.top/gtcqgjxveh.html

[K02] JSON 字符串转对象
来源：http://hz.sweek.top/gthefiqtqf.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gtdsbzgakf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hysaishi.cn/gthtnhuxjy.html

JS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtamnzhzer.html

TS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtfltpyxik.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.birdmap.top/gtbdliejmx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtdaouhvyw.html

Ruby: JSON.parse(s)
来源：http://hz.hfpthk.cn/gtieqyhktb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenjidiqi.icu/gtdkrnosmm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sufxvd.cn/gtgyxngxan.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtheuarrnx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtopfbjhzs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtgvmlhdwi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtcwfkcaag.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtqvzgvbcl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cucudq.cn/gtvmfdnski.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yvedp.cn/gttlaxgmow.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hongshengwenyu.top/gtkvaoeqzc.html

[K04] 读取 JSON 文件
来源：http://hz.ydjk.org.cn/gtzfqzpsmq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xylfe.cn/gtxkkmsczk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.birdmap.top/gtlfyjfthw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtaviysihb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gthedimabs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtbhldyfwz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gthvcxmwrg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenzaomai.com/gtbosfwcus.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yangfankeji.com/gtjifjcuqe.html

[K05] 深拷贝对象
来源：http://hz.xinyue.icu/gtnljihire.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtvkgaqcgn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tianlin.xyz/gtocscavik.html

JS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtnkwodksi.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtqffthuaa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shzxlz.cn/gtebnexcyh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daria6918.cn/gtibauusmm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj202588.top/gtvjgwlwem.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fengsongda.top/gtezipdbmo.html

[K06] 解析 URL 查询串
来源：http://hz.hnxiangtu.top/gtgpoaoabb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hnxiangtu.top/gtytswznzv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ybcxt.top/gtiqaxylfo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtuicmzukl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtegqbtcys.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ppjwa.cn/gtokeafayr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cdnleiting.top/gtyuzrdayj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zdqjudy.top/gtyypcsdhy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gogol.net.cn/gtvrutomsc.html

[K07] 进制转换
来源：http://hz.chenlongwang.top/gtmpoppvew.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sxryk.cn/gtjuzuffzj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtlfonvpjl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtiewwbzob.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtmqmrphuo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtdqbaxubr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ywan-chungtsiang.top/gtzxmmlqsc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hammf.cn/gtykfcphzd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jiagoushi.top/gtzfcduzft.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtfajlkulr.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gtxslazqus.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xziqi.cn/gtinizzmhi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtctwnqlea.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtnbztuxqn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.c1oappe.top/gtfxtclyjj.html

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtpirdscld.html

Ruby: Marshal.dump(obj)
来源：http://hz.cucudq.cn/gtcubaptbv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigfzy.top/gtskqfeqzl.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtzipouodq.html

L. 网络请求
来源：http://hz.guannengcc.top/gthyrvuhyu.html

================================================================================
来源：http://hz.xinyue.icu/gtcdtmmqri.html

[L01] 发送 GET 请求
来源：http://hz.gogol.net.cn/gtzvygvvyi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shzxlz.cn/gtwwkwoqwt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jlsjyb.cn/gtvqpqpsrc.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtjitlhkcs.html

TS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtiupirigf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtsqvwqyek.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258.top/gtwzbqudoh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.vqdsnc.cn/gtrlongfuz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtlyusnrnq.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtlelfifkm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gtfninwrur.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sxryk.cn/gtlsqquvfd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtihsbvhcp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtdsnnjmah.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.vqdsnc.cn/gtzidhnopt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fengsongda.top/gtturgpume.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.snrcjt.cn/gtqkdsqphn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhiwuduotai.top/gtkcebnedg.html

[L03] 设置自定义请求头
来源：http://hz.hnqzz.top/gtvjeqdqmi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sxryk.cn/gtmdywnxor.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhengqikj.top/gtlbcnvbay.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtjwmamwqu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtojdfehdh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yueranfly.top/gtzoenviuq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tanke756.top/gtrzdhtslp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.iojbl.cn/gtjwqongbg.html


<!-- 参考信息 -->