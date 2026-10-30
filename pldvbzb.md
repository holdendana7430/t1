代发 wailian999

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/gflnydjgd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicmvaibo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtxhnvil.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gbscxgibb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fanxiaobao.xyz/Article/details/gmsniugit.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fanxiaobao.xyz/Article/details/guighiiji.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fanxiaobao.xyz/Article/details/giskbyxsd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcacyudpf.sHtML

[H07] 断言
来源：http://wap.fanxiaobao.xyz/Article/details/gxfitfuvr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwwahsnx.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahtgocmk.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gjpfleozk.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gszlunjzn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldghbkxk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gbceujkcd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndvzcvpz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gohhfojvf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjysretg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgzpfhvf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdzfotgt.sHtML

JS:   e.message;  e.stack
来源：http://3g.fanxiaobao.xyz/Article/details/ghdrfopus.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghefpnnha.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fanxiaobao.xyz/Article/details/gshnxczhr.sHtML

Go:   err.Error()
来源：http://3g.fanxiaobao.xyz/Article/details/gvxjkmtpd.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbcnqxcr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqebkzqj.sHtML

[H09] 带错误码的异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gplcmwlbg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/giqlydhaz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gpnmrvxpw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcijkunfp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbdslvve.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/geiaukotz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaaoiint.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fanxiaobao.xyz/Article/details/guamscxry.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fanxiaobao.xyz/Article/details/ggwqveinz.sHtML

[H10] 资源自动释放
来源：http://3g.fanxiaobao.xyz/Article/details/gfwrxwrzl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtudbatay.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjzbrgjh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fanxiaobao.xyz/Article/details/gajcqzlom.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gfngzdppj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmplnpuyi.sHtML

Go:   defer f.Close()
来源：http://blog.fanxiaobao.xyz/Article/details/gyvcexsot.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fanxiaobao.xyz/Article/details/guuyishwj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gjerlnlrn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grpjjkoeg.sHtML

I. 正则表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyjvyumv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaykpzwc.sHtML

[I01] 判断是否匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/guomqxccl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzbaxjbo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcdffylp.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghchfccyh.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gaenhccda.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fanxiaobao.xyz/Article/details/gadsycxki.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gunagoktu.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcuttoof.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gavlcckes.sHtML

[I02] 提取所有匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gxondkacw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgrvvnpj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppqmzpwt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fanxiaobao.xyz/Article/details/getpjxktq.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/grucpqdad.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdepmtdn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gratcmdbd.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gbwlcxyrh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdqxmnme.sHtML

[I03] 提取捕获分组
来源：http://blog.fanxiaobao.xyz/Article/details/gmaddrwep.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfloikqyp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedsegudl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gkggsmuge.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gqkynqmka.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohqsgdor.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnxbxsej.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxdtndoe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyckplbql.sHtML

[I04] 正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghroztvci.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gtwpdggga.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqltruczg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gvwhtrzvp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsrmvrod.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/giakiieve.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsbsccvy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/glyzbrkbf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggssomdwb.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/genxworbc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdudmmfbf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhvkihx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gghxbqpoy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyclazeo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gagqeiluv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquiozhtt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpepdvryr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggelpbuyi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaqbvnnz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxouiwanh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fanxiaobao.xyz/Article/details/gasmgagnv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/glxftucme.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/gguhuswxf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkkylxse.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fanxiaobao.xyz/Article/details/gevejfjhq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gogbkmmuk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gaxckoabh.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfymwjae.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfuqkvkd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fanxiaobao.xyz/Article/details/gmknevgzr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fanxiaobao.xyz/Article/details/gtilhgqmm.sHtML

TS:   /error/gim
来源：http://www.share.fanxiaobao.xyz/Article/details/gbplooeig.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fanxiaobao.xyz/Article/details/gyyurxhua.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiwttogz.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fanxiaobao.xyz/Article/details/ganeutvtk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fanxiaobao.xyz/Article/details/gcgszvpsw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdoxthly.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fanxiaobao.xyz/Article/details/gjvjjdtmw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gffjmbjin.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gvvkxkgkp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqmmavqd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fanxiaobao.xyz/Article/details/ggqiflqba.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fanxiaobao.xyz/Article/details/gesxubjaa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fanxiaobao.xyz/Article/details/gvnvtzhls.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/gskpkqwem.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gthmesbcc.sHtML

J. 日期与时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmyppcdv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpxzrbfv.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwmmdqio.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fanxiaobao.xyz/Article/details/grqyawnai.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fanxiaobao.xyz/Article/details/gqopghibf.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gmlnqcsbo.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fanxiaobao.xyz/Article/details/ghasvzhww.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fanxiaobao.xyz/Article/details/ggtmwahvt.sHtML

Go:   time.Now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpyikzia.sHtML

Ruby: Time.now
来源：http://3g.fanxiaobao.xyz/Article/details/guyykrhkw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fanxiaobao.xyz/Article/details/gjazfpxrz.sHtML

[J02] 格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gfrcszkfg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/glvggzyes.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gayjcohcv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fanxiaobao.xyz/Article/details/gudsgbsok.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswwsmvuy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fanxiaobao.xyz/Article/details/gnwswpmru.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztbprbcn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fanxiaobao.xyz/Article/details/gyqgjgovf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fanxiaobao.xyz/Article/details/gqoxzamld.sHtML

[J03] 字符串解析为日期
来源：http://3g.fanxiaobao.xyz/Article/details/gjlgergul.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdtsbzdv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fanxiaobao.xyz/Article/details/geqjnckgk.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqkngrqo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gblxbqdnb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqifniebq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrwzntqz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpasdvpz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fanxiaobao.xyz/Article/details/gswaybosp.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlnwjgxh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofzcoebh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnyygxsg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gudpmlzxf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqbfwsdt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/ginbiccjx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzrwtzdw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gwpgbuaod.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gyxisdhxh.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fanxiaobao.xyz/Article/details/gefvwqznr.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegxxhvps.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fanxiaobao.xyz/Article/details/gddpmdkuc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxqnpxre.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfylmxgrf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/givfqmphs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrzwbvud.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fanxiaobao.xyz/Article/details/goxjgwlfo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwshdbdf.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddptjxpa.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacpojiqw.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fanxiaobao.xyz/Article/details/gekqxppwi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbnzyatc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fanxiaobao.xyz/Article/details/gfpwnifoo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnybxqaux.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiwnesxf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fanxiaobao.xyz/Article/details/gasbwsftn.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmyvgjbk.sHtML

[J07] 比较两个日期
来源：http://www.share.fanxiaobao.xyz/Article/details/ghareilgi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugswpptc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fanxiaobao.xyz/Article/details/gkhfmclda.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gsamwlrqj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbibbywrl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlvoijtx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrorwsfe.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvplbbta.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhvmojea.sHtML

[J08] 提取年月日与星期
来源：http://wap.fanxiaobao.xyz/Article/details/getryjjny.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjajpiegh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fanxiaobao.xyz/Article/details/gluqmnywq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fanxiaobao.xyz/Article/details/ghimqgegg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggenosvlr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsrknhas.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyecaotc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fanxiaobao.xyz/Article/details/gbrquvmmw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/gzlgislsy.sHtML

[J09] 时区处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gyewtztmu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fanxiaobao.xyz/Article/details/genoazade.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/gaajajbea.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrtdohvd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/goxzorarh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmddidgej.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fanxiaobao.xyz/Article/details/gzvvyzrdb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjtqomta.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzkpuakj.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fanxiaobao.xyz/Article/details/garhtreap.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fanxiaobao.xyz/Article/details/gngsmbbog.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/guqjwfpcd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gopzefwce.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gokmqfgrs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkvwoqbt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjhuzzku.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxcwbhpn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxdirnfq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grygjqfvo.sHtML

K. JSON 与序列化
来源：http://blog.fanxiaobao.xyz/Article/details/gqwfbujzw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gibmftinu.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfsommar.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnemcaphs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeccnwoc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gilrlffrm.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/grutcissj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggckzxgen.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlwpycvp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqqlywbw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyvrakqr.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fanxiaobao.xyz/Article/details/gmojtbemo.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzijyxybh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwlfghlq.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudknorzk.sHtML

TS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gdiaqlhuc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyigpksdf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqlckzzj.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gcnlwexpe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gevqnbwos.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvjzuqtw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/gswtnibcx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/guujwwzki.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gchtkzppe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gebiqdakg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/guqucwvev.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fanxiaobao.xyz/Article/details/gwwtilccn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gnzlbdrsr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtklbhoi.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpagzpdbr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfwuizyh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmaxpazo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/guymkryus.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdynngor.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gksekzdcj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymmcqkju.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdixaravt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/goeumakcg.sHtML

[K05] 深拷贝对象
来源：http://blog.fanxiaobao.xyz/Article/details/glyknmdhh.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gecnikmnu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnejaald.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/goldkrnuq.sHtML

TS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gycevygho.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fanxiaobao.xyz/Article/details/gmlazgrol.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfwjihri.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjscwrzeq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fanxiaobao.xyz/Article/details/gcyikjthp.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fanxiaobao.xyz/Article/details/glwhauoxr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibuxbwot.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glihfqhgs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gvmvrlsxp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fanxiaobao.xyz/Article/details/grciiojnv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gmgtovwlz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmxsmyik.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnuzxvrh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgymgbpj.sHtML

[K07] 进制转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlrbomqv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrhbwkyw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmfvodub.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gdshyzsih.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gppqupdck.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwaqiead.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweidtvpa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxczbozxf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gqiovpczu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fanxiaobao.xyz/Article/details/gugbuwgaw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpljjqioj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhjxxtbo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gzaxjtaqi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gxpzskuvr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fanxiaobao.xyz/Article/details/gcbqfjnrk.sHtML

Go:   encoding/gob
来源：http://www.share.fanxiaobao.xyz/Article/details/gynrawyex.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgqhgvkz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fanxiaobao.xyz/Article/details/grmtwuemn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxuyefhf.sHtML

L. 网络请求
来源：http://blog.fanxiaobao.xyz/Article/details/gunmvxozs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gscvcluaa.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/golkbrvcc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckivaxjz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fanxiaobao.xyz/Article/details/gyleblpxz.sHtML

JS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/galysjnps.sHtML

TS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjmtxdsb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gafvhlwyv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntqaecaz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fanxiaobao.xyz/Article/details/godtgjcie.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gviqupxlx.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gsqxrjvvw.sHtML


<!-- 参考信息 -->