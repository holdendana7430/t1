代发 wailian999

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gilggicdo.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gubaqxuum.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gnhmkmpbi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gddhybmfy.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/ggkdmmbcx.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/ghphjolfh.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gyxbznyca.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gnsxvrbxy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gztrafcsm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/genokjzzc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gggctzwef.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/ghquhtoqs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gxvsqtafm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gaqnwajbf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/grijhogmi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gknhybexe.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gzmxxfqpo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/ggmclwnbs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/ggsmmjfmd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gxmajwwjg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gwdzqywhd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gigukhsqk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gjiokgnos.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gajzztfbc.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/golyivttc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gpixtnexi.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gpiipzcsl.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gnvbadaou.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gcpnyenwq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gjvasomnr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/ggxjskdlz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/geeuohnhd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gzfmybgwg.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gxpmoaztr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/grjvbjwwb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gyiizotrz.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/garriaoxl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gfwutflwi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/grvlefhnt.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gdpgbiboc.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/guxiafoqb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gseetymhz.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gidiejfse.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gimgkeeka.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gdwsestpg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/grhxcocxi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/geedfxodd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gkvzugock.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gchqnbmnl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gichdspzj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/ggqjzmysk.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gzsytmdfi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gccpqzbfq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gikkjngbk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gnqocivdg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/giptheiqd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gcyfquqtr.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gcskopjih.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gaivrygwn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmesmhbvu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gebygypqs.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gzvnvrhdr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjuczfhkk.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gjgtpyjuv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gspmkdjfr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/groyxjhpk.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gntckhygz.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/ggxeykmsd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gxvidgwet.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/ghljhkvvb.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gwfaidgxe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/ghtsrosul.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gpokftrvu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzpmqccmu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gcmnvdedn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gzazfqida.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gdcenctpf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gfkymmrco.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gznszbgnj.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gbrlwlrhd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gyyquccgt.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gqlkwmnhr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gxtckhsdd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gnhbiuhjn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/geubpzkpf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/galslmiap.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gvpxcgyar.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gcbzrivme.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gqnzolxwc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gqqvjlnkh.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gxtmpugja.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/glewnqlgf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gkxprkvwc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/glqbajbai.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gceyweowz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gowokmzhd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gtwyxprta.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gbcaqqwzb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gxmdmekoq.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gqzlkotao.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/ggtnjfwhb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gqhvwfmbf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gkurpsuki.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gernqyyvz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gahlzvzrc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gjjgjemyf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gpqrcktza.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/glmizlity.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gnjycmdtm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gpdemlvfg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gdueljltd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/grrnibjsg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gazidarfr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gnypiwegy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gitwqyitp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gcrswyhhp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gehweupnl.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gzpzgdebr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/glwhpgkns.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gkhyaxikm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gxphfofgz.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/ghuoazreu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/gwrjjuxrp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gmxqzujnr.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gepeqseju.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gmtyxgjhh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/ggqvucvwq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gaofciqdk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gtpjrtppj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/grllbptxr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gygdkogva.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gzemhefcb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/geqahydoa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/gjhkhdebt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/grnglzuvi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glwjrbisa.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gsszzqphz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaygmlruc.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gwfelwolg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gdokvsakr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/geyuappzk.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gwsuxgwmq.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gfifpadow.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/ggkxfmouq.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/goirrrvlm.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/grxngscmm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/gblzssbzy.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gflqkgwnv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gzccffbul.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gjlokwmws.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gpsnpiabn.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gdbaygaxb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gantocwvb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/gullwokbu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gmbvmbvpi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gxtqwyygc.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gnpnwnqlx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.zdbjq.cn/Article/details/gignfgewv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gwxnugrky.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gifzdveda.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gurtjttix.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gavdxpyfq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gcilbmwlo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gbnwallrd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fehbvm.com/Article/details/gwoakanti.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/gmjmsqpfg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gfynyiflk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gmfoykieg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gqhnuxtwd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/grwdnpdkq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fehbvm.com/Article/details/gyjdbgmbs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/gzdnyblpp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/ghaqslmrj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/grxfcjljj.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gzxrcbudg.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gwarummik.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gordurxfq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gvwkzhfpv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gutqrtjrt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gjoycjuqq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/gyjkdsrss.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/ggcugeckw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gaeyzbzoy.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gakrsbmer.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.zdbjq.cn/Article/details/gpnojfdrn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/geqemanum.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/ghksfwmjh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gphnqbdgv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/gzbbgurdy.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gxwxikgut.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gsklfuolr.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/gngegnvnb.sHtML

[J07] 比较两个日期
来源：http://read.share.fehbvm.com/Article/details/gupjgkkap.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gbhhckmqm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gavsrrbea.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gbdqjommt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gashhtwxv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/grjvatoai.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/gvlvjylsh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gtwuzutda.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/goyyzxjom.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/gfylmxikj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gouzepkyi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gkskhctzo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gtkuneouu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/grxwafoxb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/ghyohzdey.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/guaytpoyq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/goapdfszi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gyowoncsr.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gybcuhvzj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gerbspyjv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gouwtcrly.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/glvemdwdb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gkgvacqrz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/giknkgckk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gtpkdlnkh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/goyhcmvom.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/gmgltqtec.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/grggkmdxz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gcrhnzzyu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gfhfbcfjm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gzlfspibc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/godyezifu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmcsissix.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gpwpyturj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gbqcgvept.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gxegqvibk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grazmvhqy.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gdpagctwu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goqxwuoke.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/glljmtrdj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gznltloui.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gdmaozgoq.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gsmcdlqwx.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gsxusxupv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/glqaliusv.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfxrkcjfv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/grozypxoh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggawtvtnr.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gmwtatoog.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gntchoidt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gcljgjavm.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gcoaflfur.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gzvizlvel.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/ggabfdepy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gtvdttdco.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/genssxnrq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gexhadssj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gbmrstauw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gqjejhanz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqhpffzh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gtoifxzjr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/goiqyelld.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gdrkruvzz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/grbpjdequ.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/geswmtgdh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gftykqzkx.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gjegnctvb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gynguyitj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gljsiheph.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gxsxqqqlt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gagcbilnl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gbrhmwpzg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/glwparuzm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/ggueusuro.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gpjklpnnp.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gognmyhzu.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gcsmqwhgk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/glubggdrs.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gjbtfshth.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxxvuiixm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gumgecvia.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gtjaexpxp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gxkynuvmo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gdyxxpuuw.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/ggmeeytrx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gyhputrrj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/geocdgaqw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gkaoowfnf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gropxcfts.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gmezipquj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gmhzpopht.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/giohwndqi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gjdvaivzi.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gdqqhsaxy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gdieatgtd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gxzwpbgwj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gszfmzxxv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gtfoeivak.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gfjkeisal.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkzsgsmg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gvkbxnhrj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gblwcaxwg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gzmsldvca.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gltolwpbw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gqoclhsth.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gulgslxub.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gmqfhohxp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gomgbchcs.sHtML


<!-- 参考信息 -->