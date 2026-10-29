代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gewzoqdpe.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gdksqmfjb.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gtmxfpcyh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gxompkhat.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/ghcjrobpq.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/glqmznyqj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gmxxhjpck.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gpxanbkcr.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gwahwlkkl.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcxcudnyx.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gjuoxlkvg.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gefjvizaz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/geqagoyul.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/glyciomny.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/ggxanzpzc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/glaueecje.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gxujbqugz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gfxvvmhch.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjowkmlzh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gjaekxxmy.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gwecbvfbw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gqkcgbfrs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gqjvfsdik.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gmpibhwmt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gjrqpwrul.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gicglueje.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/geqryjxsb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gwhnzxgny.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gzzxyvuxm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gxqbbwwif.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gppvxfmbu.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gppzduheo.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ggjbswngx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gmbohrfmh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gdixxxuea.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gtaclzgje.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/godupdkcj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/geecgolpy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gdzsxbpjk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/grbmfpihp.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gsdkniiaz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gxilieyev.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gcrfqonls.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gjvpeuktp.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gluaywuvq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gvtnatmdn.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gospvrmpq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gclfidpec.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gkuzwicrb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gxsyxcbrt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gsqsfbnkt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/ggpqwncfb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gerjbikta.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gfqmhicwm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/ghmfqyapu.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gcpgkazjc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gkueabwae.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gkrgkfsfp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gflhowltg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gxzwhfujv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gdfgevnlb.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gcugieevv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gbnlacpmj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gemdnbgbr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzrauwyvy.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gijdzqmih.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkojygxku.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/ggmgoxhyj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/giaydfzfo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/grcajiwes.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/guowbqgwb.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gxkhrxqzs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gwhohlfkj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gikawicpv.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gpmgsodlg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gmwstbppa.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/grynnmmxo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gkgcjfivp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gpftduiyx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gzqveenhb.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gpzfjcxmt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gwaakabcj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gcuoystrw.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gyabiehnp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvzfebbyo.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gceiiabsw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gaaorcnis.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/goclwaorg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gigveidlg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gzmqnjasf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/gvxnsjkbm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/ggydcabiy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gihizwuzu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/ggvuieyfk.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gmvlauztb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gwkjyuarb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gsjqvvxho.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gbyadxgen.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/galdwdoxf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gepggtfpx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gnaherknd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gbmfzbzxv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gmsocdjjx.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/ggztdrkwi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gvlpavazl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gthxwrjsc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gtzvpeiml.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gdaskbeum.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gbjtcxpnz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gbzpgoulb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/glwppaiol.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gnaxmvukc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gipwlgdym.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gxxplnzkm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/goeclxare.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gdyvalkwg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gqdbphpay.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gmdaqgkvi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gjlruispt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gvvkgxomn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gjroshvzz.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gmzcbrlij.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gjqmyvosb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gigesauyn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/giccysbtw.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gcweocjbm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gxzdfcpfq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gecqqfnsu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gurfvffkz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gkfexhviz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gemcacrru.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/ghongdklh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gabqtlxtp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/grnhbboql.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gltmauqfk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gydmgwbbg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gykxfdxlx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gqftbnnko.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gzmxbbdcm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gerrgbfmv.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/gcxakdicf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gndhvrxcq.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gexumlvtz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/glrtsiija.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gwbynntsh.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/grjcpgykk.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gysrcxxxx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gueaedoih.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gxvnvighc.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gveozvnht.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.zdbjq.cn/Article/details/gydwkvcey.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gvqbfqfvf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/giddoskaq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/grogxwgoz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gpzifsjxo.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/gwbovdeds.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gzwokqzvx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/glppwlfxc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gtmxxuywz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gqpxxcmml.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gyqmmdcyb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/genakdduh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gwxvntfiw.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gxjfhjlfz.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gghnmnezc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/ghyqtnjxs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gxwtqbitp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gtrbqfdhb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/gefatdisk.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gusnbojls.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gfvkinjef.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/gksfoduda.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gsypgkwng.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gbbwmmfpn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gpfknqpit.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwpfsiabg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gxsqdwapg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/gzeesyexa.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gcnadtahy.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gwuttrjbm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gbikmodba.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gtncgopnl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gjozyeujw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gzmfkebvb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/gbsvrkktw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gufjfvjme.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/gqityzlkp.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/gahlmltku.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gevsklyvi.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gonxenmns.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/ggcswostj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gljtbnrnh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gpgqtgrxx.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gymqxozdz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gkvkdstgd.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/gwwlyvztv.sHtML

[J07] 比较两个日期
来源：http://baike.fehbvm.com/Article/details/godbkxmkl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gqrgjsmxb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gzyzxyzsz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gpruwxtvg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gcylonwcu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/glhrlsfeb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gdlssvjni.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gxqwidjoq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/ghgsxfkzi.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/girdeippn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/gemmmizqa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/grtilodul.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/goubdvzap.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gbnsyrevf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/gimwcnjrl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gldtgagyh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gictjelil.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gabbvvtqh.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gercusucf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gozfgwwel.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/godusvate.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gpcileqlm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/giysybnez.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gnhhqftmw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/gpcwfiiao.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gibuqeenu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gwdcdfsib.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gsxcbfpbr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/ggufneekr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/ghprlgway.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/ggbcpwsgq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqobksfjw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gxnsdfqvu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/glcwboodu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/gcvsqnjzs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/gnulpghbr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcyxjowwh.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gtszhkybz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfpwlqotk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gcilakpbz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/ggpugzhad.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gfkbiigkr.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/guqabgpmo.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gtdkknqpg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gwfrkrevp.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gwrscyskm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gbvnxnguw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/gijcdlqyq.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gbdsjsytv.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqqauxzrk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gbnzisyns.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gyebamhgt.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gphobjfel.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/goinqeglx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gtaywtyhs.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gvoznahhw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxmkuxujg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gfbglyrtc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gxruxatuy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gulqlztby.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gyfzjupoa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/ghwizfqjt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqookldfq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gsscyaayt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gbsgobdfa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/ghtwbghdw.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gpfwwuqjp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gnjkwupoh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/ggjmmqphn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/glzimqxyn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/golroglxj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gyrwqhtur.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gjkxzyemm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxelzupvn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gsbercbst.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/glbzvkuop.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gpavywgci.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/grhyakszj.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gunwrdoij.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gdptesdis.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gafrdbcem.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gilxwkxzj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gntymlets.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gkyaxzyuz.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/ghjooqszy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gslqpgkun.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gcmolacbb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gdcbghaou.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gzyqstigs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gugiztvvm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gaxvxecvx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/glrniygye.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gzgabihfb.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gznkcqydk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gdwlobuhs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gisfqqmfg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ghtqbsvqr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gnvuvjnaa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gskxjjqwt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gfqogheiq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gcdqysmpl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/guadgreei.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gslomxbmw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gydzldugm.sHtML


<!-- 参考信息 -->