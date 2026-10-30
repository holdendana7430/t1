代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsezrvge.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcgpttew.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksetdodc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdzwumgui.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkxlehipn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxopzsdxb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gclvtmodd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtjafqxge.sHtML

[H03] 主动抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gdzxqwrtt.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fanxiaobao.xyz/Article/details/gxfnrlwgt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqgeiwjx.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/ghqqoltdb.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gqyeuswcw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbchbtudx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fanxiaobao.xyz/Article/details/gwlhogzfx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgwzsgly.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gtaebymsb.sHtML

[H04] 自定义异常类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfytwxkn.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/giawlwhfk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeymaoqd.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/gajqqtvmg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghmbdzvip.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbqlcakt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghufhbrbq.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyomtaiv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggphhtwkc.sHtML

[H05] 捕获特定类型
来源：http://blog.fanxiaobao.xyz/Article/details/gsakfanqc.sHtML

Py:   except ValueError as e:
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcclyhzq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fanxiaobao.xyz/Article/details/gighgiygf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwxzhzew.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkncwcgtw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gncvddjko.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsqzegss.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvslfhwff.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcmaxcoh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/gnxrboqbu.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrhuicis.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/giwdhexth.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhchicat.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzjxbckg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fanxiaobao.xyz/Article/details/gisbdpmod.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyabdenvv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fanxiaobao.xyz/Article/details/gcrjmnwuo.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gnfnnjfhv.sHtML

[H07] 断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqbvyegg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvnpsuvi.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfjybllw.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/grftfsyvv.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdggxerp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fanxiaobao.xyz/Article/details/guowcuits.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fanxiaobao.xyz/Article/details/goojmyakv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fanxiaobao.xyz/Article/details/guxugpfoh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gvrmsbbps.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fanxiaobao.xyz/Article/details/gmsjdajkb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtrxitzu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvackwgf.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fanxiaobao.xyz/Article/details/guuosxqjf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gumnpzqkx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpywqocro.sHtML

Go:   err.Error()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrhxzhdw.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fanxiaobao.xyz/Article/details/gwhsfnwjy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fanxiaobao.xyz/Article/details/gchwcgsuq.sHtML

[H09] 带错误码的异常
来源：http://baike.fanxiaobao.xyz/Article/details/gdukqiaif.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fanxiaobao.xyz/Article/details/gldgokuog.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/ghazmqfsc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfmlishj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnhiqrys.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggksrmxon.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfflecidt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptbobhoo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fanxiaobao.xyz/Article/details/gmibvakvy.sHtML

[H10] 资源自动释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrpyxmwz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxekmjwb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpachhdds.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfuxbkpj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gperyzzbo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/gijvtunlr.sHtML

Go:   defer f.Close()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoaacfff.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fanxiaobao.xyz/Article/details/gospwfgsb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/geadsajuk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxjqfekxb.sHtML

I. 正则表达式
来源：http://wap.fanxiaobao.xyz/Article/details/grtvqizle.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcemotvw.sHtML

[I01] 判断是否匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gclcxwqzj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gixownrmn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gkzpbsjuc.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gaztumwtw.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdfxwgui.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fanxiaobao.xyz/Article/details/giklnabfq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmnwjuin.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gbwdfxupg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvrrnfdd.sHtML

[I02] 提取所有匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ggquatuqn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gejygqsel.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fanxiaobao.xyz/Article/details/gidcgpqvw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbvzdyrz.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gugdgwglz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbdjulpv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjskysmpe.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsthrehmw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/grrhkspio.sHtML

[I03] 提取捕获分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuawurrp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlpidome.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gejrnhcps.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gwbbugjky.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/geayhdjdt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiwjouro.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklnjvoah.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gvccoskfm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fanxiaobao.xyz/Article/details/gupnfgukf.sHtML

[I04] 正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvdmrgvhp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbagkzjt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpoozfui.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gicgqgijv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuzndxlj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdjhktro.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/giznoeqra.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvrfcfqb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gyyaewjfj.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/glyirrjgg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhowecyg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gndtjjfmn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdygursno.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmvvipii.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fanxiaobao.xyz/Article/details/gmnmvriwu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtkeqyqp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gjopryvlf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gpdvtpefg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmldhrgsl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gildvtjmh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxdxirws.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fanxiaobao.xyz/Article/details/gfedtmoba.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/glgujgyzn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gckckrkbt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fanxiaobao.xyz/Article/details/gwcunmmvh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzzwtixd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gcqzbtjnj.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpvdbprd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fanxiaobao.xyz/Article/details/gejmlzbip.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fanxiaobao.xyz/Article/details/gqqwniepe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fanxiaobao.xyz/Article/details/gcrdflwwe.sHtML

TS:   /error/gim
来源：http://mobile.fanxiaobao.xyz/Article/details/gejvzutca.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrmxmifx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fanxiaobao.xyz/Article/details/gtcvpynqj.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmtoifii.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnixwhnm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjjlhcab.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fanxiaobao.xyz/Article/details/gknacpddf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjtremzg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyvqtkeu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtfrioig.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbfveipz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fanxiaobao.xyz/Article/details/gvvhjvgza.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxixupruk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fanxiaobao.xyz/Article/details/guzerinkr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/giyxcfgqz.sHtML

J. 日期与时间
来源：http://wap.fanxiaobao.xyz/Article/details/gtbwxevjw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glpakrwny.sHtML

[J01] 获取当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuontbps.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fanxiaobao.xyz/Article/details/grsegxhpf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gpvukusvz.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwuktuff.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjmpdoon.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdvfbwuu.sHtML

Go:   time.Now()
来源：http://blog.fanxiaobao.xyz/Article/details/gucktcbnr.sHtML

Ruby: Time.now
来源：http://wap.fanxiaobao.xyz/Article/details/gskzdkbiw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fanxiaobao.xyz/Article/details/gsawedjaf.sHtML

[J02] 格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gydhqlagi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gelishvvo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gaxrwesaa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fanxiaobao.xyz/Article/details/gjlwtlwjx.sHtML

TS:   d.toISOString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnciqykf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwpombto.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fanxiaobao.xyz/Article/details/gtbxvauwq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkfnqggg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fanxiaobao.xyz/Article/details/gskzehwom.sHtML

[J03] 字符串解析为日期
来源：http://baike.fanxiaobao.xyz/Article/details/gmveuepfp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fanxiaobao.xyz/Article/details/gatlaiyig.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnlqjrdf.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gccbushmi.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/ghopdlkxw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/ghukqnuqs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gjcoyhhjk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/ggdbbnzfz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvixabcou.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnnpfkgn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/ggabuxzld.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwoocxau.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmjigurc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gjnphvhpo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gmzznlvvt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurrphrvu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/garbhyrbt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdkkalsk.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fanxiaobao.xyz/Article/details/giejafslz.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gynjwgoxt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fanxiaobao.xyz/Article/details/gopwlkqqs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhcroruj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyqojkie.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/grsthorth.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbanghgk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/gxlyvopth.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvvaawhw.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/gzkdoymvn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitpirkiu.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fanxiaobao.xyz/Article/details/gdyefnxht.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fanxiaobao.xyz/Article/details/gbuokithc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fanxiaobao.xyz/Article/details/gpqblrxtk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvhhfryz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsrarbpa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpvrjigh.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fanxiaobao.xyz/Article/details/gkykuxjje.sHtML

[J07] 比较两个日期
来源：http://blog.fanxiaobao.xyz/Article/details/gzchkhwrm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/ggmvbxapr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwfgvpyo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvoznrxy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fanxiaobao.xyz/Article/details/gckhdnqdy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/gykkumckb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfdskomd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdivumwz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfzxiwdz.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpjfaedf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fanxiaobao.xyz/Article/details/ggdjvxwwl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfniderel.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblhsdzoh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fanxiaobao.xyz/Article/details/gatgfsrdw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/gmragmqud.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fanxiaobao.xyz/Article/details/glqhjwwkh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fanxiaobao.xyz/Article/details/ghyzezveb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fanxiaobao.xyz/Article/details/gfeazqrus.sHtML

[J09] 时区处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnmslyml.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fanxiaobao.xyz/Article/details/gellppbxi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrqliyua.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/gmiqkfyco.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/gadodlduv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxwpjfdu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrzrryvu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fanxiaobao.xyz/Article/details/gocqrablf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglstpkyq.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fanxiaobao.xyz/Article/details/gkpvugxuw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fanxiaobao.xyz/Article/details/glwjxpmgd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fanxiaobao.xyz/Article/details/gshovfcht.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdplnxmp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwjmyctg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fanxiaobao.xyz/Article/details/galqacoin.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fanxiaobao.xyz/Article/details/gmedwytyf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtihshqjf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/guhoiogco.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwajvyds.sHtML

K. JSON 与序列化
来源：http://read.share.fanxiaobao.xyz/Article/details/gijbfsklg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtjrkvhzf.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gagzwaztw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gquarujbn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gzhfiqwyc.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gdzvtlcag.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gijzqvosb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgktmpph.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gplmfjkxe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvktuvsv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gignezfgr.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gzvmbpvuo.sHtML

Py:   json.loads(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzychlwe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvqnsgbr.sHtML

JS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gvabefggk.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcxaixyd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gtvityynn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwkxxjoz.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdekhikua.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzgvitqc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvgauabn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gytvxarhz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiiaqoid.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfsstrsxk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwvakjmub.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrikuiog.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fanxiaobao.xyz/Article/details/gmifjcfvz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gecvtqjjs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeaxbvyt.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdzaiikzt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gvwidciwp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvozhgsbi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnwgwhuw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieohrzkx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gnsinhvki.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/ggkkwvkqp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gexnrucow.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gbwmgjnfp.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhdjrsut.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkarqvkqf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhnsxveu.sHtML

JS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwjvrgun.sHtML

TS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gvaeneeef.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxvglpqt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyjnvuiw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsangybf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fanxiaobao.xyz/Article/details/gnkcrlmbj.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpamxilmv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gimgoyuue.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fanxiaobao.xyz/Article/details/guabdhzyt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsexbqbve.sHtML


<!-- 参考信息 -->