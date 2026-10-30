代发 wailian999

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gbgpldqus.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gmpqurfju.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gedmindff.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gxasbfpty.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gwynanorh.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gdmwirzat.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/glultjvsh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gnjkjlrwu.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/guygejunt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gjwjvfyyl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gworwzmwq.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/ggcikyhxa.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gsuczywbt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gqaswisgq.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gfrnzurey.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gcglajugc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gnxghjxgs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gkqxorbug.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gwaeknymr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/ggaiksslq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gkqxqcwuz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/guvxjvmoq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gmrunewdo.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gtpzokyah.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/grjbtmssk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gfgilnbub.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gmoeowdxe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gqkviumqx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gdorqetag.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/ghnhpuxrd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/ggtsqjbta.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gupyvyimq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnrkchbml.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gtgnppikr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggkedwrip.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/ggwcedwot.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkmlpahv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gstlcfnys.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gpjljngvg.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gjionxssr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gvrktpfgp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gvdqsknef.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gmsthgwhg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gjypeoccs.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/ginhepgjj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gibkrsvws.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.hesvh.cn/Article/details/gpmbdidhj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gwbxytwjh.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gvymcxnpj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gpfvrdubn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gtnrmupcr.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/glorxgdja.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/grwsywirp.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/goivkjxkr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcosmulbc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gqutxzppx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gvloowqww.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gkgyhscom.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gncllajru.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/ghdusktcs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gcleiwriw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gkdtlslmr.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gmbypwkfx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gsvlwfgpe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gikhwndzo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gaissxdqo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gcncurouj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gecoalsso.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/geaudoknd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gblttjkvv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/glwoiqfnu.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gthhqsdop.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gepzsvldw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gdxmwajqx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gsxigwwbv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/grijdzpfm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gjgwfgscg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gxaqbvrqx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gewjtgino.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fehbvm.com/Article/details/gzsalohrq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gntnanqnn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gaaemkrhb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/ginodbvpg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gwmcxlkmp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gddddanbm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gwibssnvd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/grfnsdohc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gsqgwaroa.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gypqohkkd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gvcdremwy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gtwzuckgv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/givrfrojq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gsxgharur.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/gvmcgtuzq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gymikkcyd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/goayalhid.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gqhxtqeda.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/ggenupcii.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gwwsrxoti.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/guupmtcex.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/ghmwuwlwm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gyhdtmobc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/ghnlunsyc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gebgzglsw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gwdkuxvdx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gzsifuvbn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gnynyfbou.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghodqqzly.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/grwlcbzkw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gacvqojpv.sHtML

[J01] 获取当前时间
来源：http://www.share.zdbjq.cn/Article/details/guudhzxxo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gixotppaq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/ghnqdxtww.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gtisavput.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gedawyhdc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/gjrvxevmr.sHtML

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/gtrkolzql.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gjjncryml.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gcbygjydl.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gbsktxdvc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gqmdakugc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gqypuewhx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/glwokmzno.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/ggeyvjibt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gpkortxwp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/gsvsmzmtn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gmuceeert.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gdqlkhmii.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gezjorduy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gxrwqaehc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gbjfhcfdq.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gyztonnvr.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/glkeazmgi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gmxnlmqpg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gkmyspfzl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gjimjggxa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gerkrkkpc.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/gvvpaepks.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gdcsdxqpn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gupizliri.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/ggypexjec.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gbrgvtvnn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/glhrejfte.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gsutjizqm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/ghqtgfeji.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/gmumprvwj.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gazycpyoe.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/gpwywjeie.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/gmuxhwemp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gcweuhdob.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gpfohhfws.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gwntluzhu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/ghtxavtat.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gzsstgwtn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gilqprolq.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gptrekxdn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gzdrjtjzw.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gqnkhdtaw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fehbvm.com/Article/details/ggxvenqoe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gxjpupuvr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gsnmzqxlz.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.hesvh.cn/Article/details/gxjkcrcgb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/glgbislxb.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gaenzflbv.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/guaqdvybr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gpkstynga.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.zdbjq.cn/Article/details/gjxginmow.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gycvxrcrr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gqkarlunp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gbmfvpxfi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/gsjrejdyi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gpnmuxfcd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/grycosvkb.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/gobtyjgqf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gzgsvxddz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/geypietch.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/ggaelvgzz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/ggmoepqcy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gpvnctbxe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/gjngrddle.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gusdwrfcp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gutdzzrbz.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/gsbpejhvb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gmlvkjgsy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gbgigayfl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gzdsbvxdw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gvhjqbggl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gvawaykoa.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/gcybjzpff.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gtthkkwck.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gzyupbfip.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gfrifwssm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gofmygfvq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gkdmjrbot.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gdugyhoao.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gizssymrs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfghyiwpc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gmkmajfzs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gpqsasbdt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/gbwqovdeq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfjhnkyli.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gvqdljnpe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjbvbeehf.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gnpbkjuuf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gbvhzzsnu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gtqrsnief.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gtllsblso.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gjebfdbpx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gdmwxdqou.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gldnwjkav.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gonxlmndm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gujthzzrz.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gluyovowb.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gkwznlpsq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/guttqxbnj.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/galskbpff.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gtxhdnopa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gesnahsbz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gokdiozrh.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwzvegdey.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gorfdujci.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gnjhoyjtc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gzvkpowkt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gpmcegibu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/ggcrutxgf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gezfxveur.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/ggepbolud.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gxmdajdya.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/guwypdegs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gpulphkmb.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gvfneywwj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gtpyjkmdg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gtvpvxqbo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gxgsluyln.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gxibhexuv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/gnweuiblg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/guzhpjfdt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gibsnbfdk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gijfxpark.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/grueldplf.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/ggfundjsd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gohihuqtv.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gamqqgmpe.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gldqarytu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gkexysdoj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gizuipwib.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gbiznfzcr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gkavrezcg.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gohsghlez.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/guczhnfrc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gkjwmvzcs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gtfqmovzm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gnwjzafgk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gmhzcszzc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/ggmaocezy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gaozklfng.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gcjpjzpwh.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gyhidqsjk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/genievejp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gwqigalku.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdakrkyfb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gegcbgkts.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/ggbzxpuhz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/goezybewe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gigzadytu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gvpkdlnki.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/ggsdgmeum.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gjfkclvse.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gdwlzwmwi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gnfqwxvxu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gybakfvsp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gnsvkfoth.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gbvecfepz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/grqipsyzt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gxjgsskia.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gssuhgnrt.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gpnnvscfc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzjpysrvj.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gleiejfjo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gztetsmoc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gchmemdig.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gprnxkvmr.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gnxavdsyv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gnfhgrsyh.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gjtnadqhh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gjxwittgc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/grqkubyja.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gecaexqzr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gxdsagumn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/geovsddkb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/giaoqbkab.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gzdyiiuih.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gcjqnscgw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gtxxilumt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gfaxmwbuh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gmwfobanw.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gehlygnco.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gyqhectey.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gkdjufcox.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gzmodrvlu.sHtML


<!-- 参考信息 -->