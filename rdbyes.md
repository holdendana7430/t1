代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtrioytvux.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtgcwdztzg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhoulong.xyz/gtnicpemjs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ivvv.top/gtvcdqrfnv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tanke756.top/gtmaainrfg.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigufen.top/gthelvfsyh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangkeji.top/gtlftzylme.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xziqi.cn/gtcrlpbbgg.html

JS:   e.message;  e.stack
来源：http://hz.xylfe.cn/gtdasghkbj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtjiwnpsbf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dashuyun.cn/gtvuxnlbmg.html

Go:   err.Error()
来源：http://hz.yvedp.cn/gtbmazanem.html

Ruby: e.message;  e.backtrace
来源：http://hz.xylfe.cn/gttwjaqnju.html

C#:   e.Message;  e.StackTrace
来源：http://hz.0kj1m.cn/gtdhmcjinv.html

[H09] 带错误码的异常
来源：http://hz.andypj.xyz/gtawdpgxfu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hywenlv.cn/gtpprfoets.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtskhmkzqa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gtuybntafm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgufenzy.top/gtcbdixwhs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.pengpengdd.cyou/gtcudgeeiw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258888.top/gtrezdvfic.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigufen.top/gtxphknctd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gogol.net.cn/gtirnmyjdg.html

[H10] 资源自动释放
来源：http://hz.ehwqpu.com/gtudjheulb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gzhubu.top/gtvbdaeqpl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangdashe.top/gthffepyer.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtsmnflect.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtpcpduvxl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dashuyun.cn/gtbquokiko.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtbonvniwp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cashguo.top/gtwffxzrux.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtoiyedeac.html

================================================================================
来源：http://hz.zhongyouzk.top/gtynedevav.html

I. 正则表达式
来源：http://hz.sysykeji.top/gthyqiyzwu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtsiayczfq.html

[I01] 判断是否匹配
来源：http://hz.guannengcc.top/gtsswzufvg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtrjcrdpxy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aibaodan.cn/gtmovgnyoh.html

JS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtwdjzkkfq.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtfdizndph.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigufen.top/gtvytddssk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gzhubu.top/gtquqlaqlq.html

Ruby: s.match?(/\d+/)
来源：http://hz.gzhubu.top/gtxfzjcjig.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yvedp.cn/gtuockfgpm.html

[I02] 提取所有匹配
来源：http://hz.redwolf501.top/gtfecaeejx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gogol.net.cn/gtgmmlkmrh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yongpay.top/gtgzjljypx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtktggyzcv.html

TS:   s.match(/\d+/g)
来源：http://hz.ywan-chungtsiang.top/gtuiorfpii.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhongyouzk.top/gtjfibvnws.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jlsjyb.cn/gthjmuuhyb.html

Ruby: s.scan(/\d+/)
来源：http://hz.cashguo.top/gtonhpimms.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtszagoyxj.html

[I03] 提取捕获分组
来源：http://hz.aizwys.cn/gtqhvjzutq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.316326.xyz/gtbccxgvds.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cheryme.top/gtkwrwasgd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hongshengwenyu.top/gtgxwzydct.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gtxbcgqwgt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gtbiblkguz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtyfaqnjja.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenzaomai.com/gtfdxsejxl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xingfuxueyuan.xyz/gtwpclmjvz.html

[I04] 正则替换
来源：http://hz.jinyuanbaomall.cn/gtlvcvuecp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gthxyproqv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtntlanlui.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtncgooadb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hywenlv.cn/gtywzhzone.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gtlybjmtgg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xylfe.cn/gtfccghzbb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tanke756.top/gtwmreenly.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.feifeiyinyue.top/gtjqnvkqhq.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtwodohljz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinghuilouyu.cn/gtcgqhjbvx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fzhhl.top/gtagnkgvzd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtuiczfmzq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtqhvsbguf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sweek.top/gtlubzefrm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtvcpuhsrg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gthwdquvkn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258888.top/gtoyggopkj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigfzy.top/gttjqmjpyx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.haohaochexian.top/gtyaqkqipz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtloqmhtnk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtyggrwymt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtxvgnrqcb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hysaishi.cn/gthllpnrnb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shangyingyoupin.top/gtsocbfdyo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.haohaochexian.top/gtnvfclbhz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.quarkkingdee.top/gtwiypothg.html

[I07] 忽略大小写与多行模式
来源：http://hz.dianchejie.cn/gtrrfdievu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jlsjyb.cn/gtjphttkgs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hfpthk.cn/gtqbyccylu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pengpengdd.cyou/gtfmmljfdz.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtkjmtbawy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtsgimlpsd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zdqjudy.top/gtovmysfne.html

Ruby: s.scan(/error/i)
来源：http://hz.zhaomingkeji.xyz/gteuftjrbk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hnxiangtu.top/gtkzxwrbuk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jiagoushi.top/gtqmixiwro.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shangyingyoupin.top/gtksmxojtk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gotoacloud.top/gttctsxpmc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtupiqcfct.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtjtoagnzt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gtqcdckafh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.smart0.xyz/gtoyyeftat.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtjyygqcxa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtfbwpfrax.html

================================================================================
来源：http://hz.tian-w.cn/gtnofkqjya.html

J. 日期与时间
来源：http://hz.tianlin.xyz/gtzuhcmrnv.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbmqymmjf.html

[J01] 获取当前时间
来源：http://hz.fengsongda.top/gtjujhxaao.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhixingplan.top/gtobdgqawq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtxdjxnuqo.html

JS:   new Date();  Date.now()
来源：http://hz.gotoacloud.top/gtthlvnpkl.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtofdcohdj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daxiang520.top/gtfnkrdjyk.html

Go:   time.Now()
来源：http://hz.yonumen.top/gtmofbfmrh.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gtjnukthdb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hfpthk.cn/gtozualvmi.html

[J02] 格式化输出
来源：http://hz.9152youxi.cn/gtuimsbmna.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtqziyllxd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gttyhvsedx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.redwolf501.top/gtrcuoocos.html

TS:   d.toISOString()
来源：http://hz.tian-w.cn/gtrcfuhccj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jyoumei.cn/gtylilivpb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.haohaochexian.top/gtakxhnoeh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hysaishi.cn/gtuwkqlpjx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtnjanoxrl.html

[J03] 字符串解析为日期
来源：http://hz.xuetiantiany.cn/gtwcoyuvil.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tian-w.cn/gtiehmzwfg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gtrsfquzls.html

JS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtbjrsfvgc.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtlkuwwliu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtyiadmlog.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shzxlz.cn/gttpalkyxr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtswgjimlo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gtgcxdzlgn.html

[J04] 时间戳与日期互转
来源：http://hz.ydzc1.top/gtrmkmvhnc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gtbgsdexay.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aibaodan.cn/gtegcaupuk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.birdmap.top/gtltpsmivj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnqzz.top/gtvqakjpkz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtkmeojuow.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.9152youxi.cn/gtxfviqael.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gzhubu.top/gtwndtqbwq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuanzx.com/gtzarwowsx.html

[J05] 时间加减（加 7 天）
来源：http://hz.0kj1m.cn/gttjmrerrr.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtpvzmxkui.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.smart0.xyz/gtooupbzwe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtxoerzcpl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gaohongyu789.top/gtxxjonuib.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.feifeiyinyue.top/gtehepcouo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.bjfxy.top/gtvfozaane.html

Ruby: Time.now + 7 * 86400
来源：http://hz.birdmap.top/gtfodhbmda.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gtemsxodgi.html

[J06] 计算两时间之差
来源：http://hz.wangdashe.top/gtrjahnlgx.html

Py:   (end - start).total_seconds()
来源：http://hz.hysaishi.cn/gtosuirsel.html

PHP:  $end->diff($start)->days;
来源：http://hz.ppjwa.cn/gtebwtkadg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ywan-chungtsiang.top/gtpfzcvgdw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtyapvyefx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxuanxn.top/gtplumbdup.html

Go:   end.Sub(start).Hours()
来源：http://hz.cucudq.cn/gttsbsutrs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtofqozuis.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhengqikj.top/gtlxqhwmqf.html

[J07] 比较两个日期
来源：http://hz.bjfxy.top/gttxsumtto.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtayvhftzx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xingfuxueyuan.xyz/gtjhbxsnma.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtfgjvaqjk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gttrcwalya.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gaohongyu789.top/gtlvkyyemd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhongyouzk.top/gtxxttwoxn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtgwsfbnxi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtoexocavs.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtzskmnzmf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.snrcjt.cn/gttmqwdcit.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yuanzhike.top/gtzxkjycmo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jiagoushi.top/gttnhawewp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gtjafnpswc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtlbqwbauj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxuanxn.top/gtdcdznwxn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhiwuduotai.top/gteoxoswov.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.redwolf501.top/gtquzujbrv.html

[J09] 时区处理
来源：http://hz.hnxiangtu.top/gtidayrxcq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yangfankeji.com/gtvsrvnwyl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenjidiqi.icu/gtyhyvkpcq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtgrkkzkaw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtxxawoafh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtcfopsyfe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.quarkkingdee.top/gtpapbgksl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxuanxn.top/gtdsrucwck.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cheryme.top/gtswidzyfj.html

[J10] 取今天 / 本月第一天
来源：http://hz.sxryk.cn/gtyvosijyk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gaohongyu789.top/gtfuztqgyq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fzhhl.top/gthkzattei.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gotoacloud.top/gtwilmfalm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hywenlv.cn/gtkngkvstr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gttcfpmguk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gteabkijsp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtavzxthmp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aibaodan.cn/gtpfrrkyrx.html

================================================================================
来源：http://hz.ppjwa.cn/gtlkqazeyu.html

K. JSON 与序列化
来源：http://hz.ppjwa.cn/gtqvharriy.html

================================================================================
来源：http://hz.nanxuanxn.top/gtriyzmlxn.html

[K01] 对象转 JSON 字符串
来源：http://hz.cqqwz.cn/gtwnorxojm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sufxvd.cn/gtbxinnjyj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtzlhfqjib.html

JS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtfdssyrat.html

TS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtocxbpqvz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jyoumei.cn/gtcnyfjqds.html

Go:   json.Marshal(obj)
来源：http://hz.zhoulong.xyz/gtwttycltt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zycfv.cn/gtaqaoqkyb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sxryk.cn/gtxdwroihc.html

[K02] JSON 字符串转对象
来源：http://hz.jinyuanbaomall.cn/gtaevsshqd.html

Py:   json.loads(s)
来源：http://hz.zhoulong.xyz/gtfitsrcty.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pengpengdd.cyou/gtnocwvljh.html

JS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gteyrdxrlh.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gthcvkhvfz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhoulong.xyz/gtoqiatwlb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gteoipgphg.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtmvnzjqqf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fengsongda.top/gtcakbeltd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gtfogbbldw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtcfpgdzqf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gthfscmdhh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtapgkzlob.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtajfaowdc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.316326.xyz/gteajpntoj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.vqdsnc.cn/gthaiyrvau.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtschcoueq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pycfn.com/gtojxqmvkj.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtdislgyap.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenlongwang.top/gteyjnqqbp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sufxvd.cn/gtswxbqgxi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtwtqqqhdd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtpsyvlsjo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinyuanbaomall.cn/gtxdrjthpv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtgwuahzvw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daxiang520.top/gthxxsllvj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydjk.org.cn/gtiaiexgaz.html

[K05] 深拷贝对象
来源：http://hz.ybcxt.top/gtrktnbdga.html

Py:   copy.deepcopy(obj)
来源：http://hz.shuidangran.top/gtlawnegjp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shzxlz.cn/gtcuzuocjn.html

JS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtyvcxxnjn.html

TS:   structuredClone(obj)
来源：http://hz.sweek.top/gtoyfozxbe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yangfankeji.com/gtcjumlzqm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gttqxuptfj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.kuanghao11.cn/gtrlswfzps.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.havefunace.top/gtxzvnfnlq.html

[K06] 解析 URL 查询串
来源：http://hz.chenjidiqi.icu/gtwbwcpruv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hnxiangtu.top/gtlijdcwjj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tianlin.xyz/gtdokdazem.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtyjjsqfjv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gttrwgunfg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgfzy.top/gtcphvgahs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtlpyhnkue.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.316326.xyz/gtluszccyz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.birdmap.top/gtenxyjibh.html

[K07] 进制转换
来源：http://hz.andypj.xyz/gtmzizfcim.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtsucylxgf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.quarkkingdee.top/gtsfurtqgr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gthfvypxpy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtiqjcehfv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtgcqtsuyp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtzrymhegv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gaohongyu789.top/gtmeuqkjin.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gtavlnlsco.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtfkimullz.html

Py:   pickle.dumps(obj)
来源：http://hz.zdqjudy.top/gtyecqnyig.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangtech.top/gtqyhdrrjk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtlekknvgw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtyusoqrvm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.birdmap.top/gtqevuzzee.html

Go:   encoding/gob
来源：http://hz.xingfuxueyuan.xyz/gtomuuryxx.html

Ruby: Marshal.dump(obj)
来源：http://hz.316326.xyz/gtnvkbduii.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guowangkeji.top/gtzdubxqkj.html

================================================================================
来源：http://hz.dianchejie.cn/gtthrqfiur.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtsazqpdhk.html

================================================================================
来源：http://hz.xziqi.cn/gtkmmdiptl.html

[L01] 发送 GET 请求
来源：http://hz.chenlongwang.top/gttrpllsam.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cheryme.top/gtmcrmqvcj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gtaftvtrrs.html

JS:   await fetch(url)
来源：http://hz.tian-w.cn/gtcrptkkmr.html

TS:   await fetch(url)
来源：http://hz.wangdashe.top/gtldwdfzti.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jqgufenzy.top/gthzbthyzc.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtosefuwxo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.snrcjt.cn/gtadealkjg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shuidangran.top/gtigyejwat.html

[L02] 发送 POST JSON
来源：http://hz.316326.xyz/gtuuktybip.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.c1oappe.top/gtwgzzlobo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jianghu66.top/gtgamnfybi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtvqacenjm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.52xcode.cn/gtasueztua.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.birdmap.top/gtghhbdydi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gticpzdyys.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tanke756.top/gtiwxgtsnz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgfzy.top/gthuhsockw.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtbcrbzghe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tanke756.top/gtprlwalfi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuxming.cn/gtpqrcmbzj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtcspisxxh.html


<!-- 参考信息 -->