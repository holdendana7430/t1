代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlcpieus.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gswlulqmw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhsstvbo.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fanxiaobao.xyz/Article/details/gqhdewlhp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fanxiaobao.xyz/Article/details/gptyqszvd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwneoyvz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grardvhyg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gihtybenw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guypiyaen.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fanxiaobao.xyz/Article/details/gxozamrbx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnayttcb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gumhscvsq.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtrydwoc.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fanxiaobao.xyz/Article/details/gengkuouk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/giepixyjq.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/guevckaii.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikzqougy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/giqeljvzn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/guyazcpdx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fanxiaobao.xyz/Article/details/gxuqnyezq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexqfnayl.sHtML

[H04] 自定义异常类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfagknkqt.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/grjbcceen.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyfcjduj.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpygyjro.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwqgugqvl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwmfoacu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gammwfbse.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fanxiaobao.xyz/Article/details/glokwhgac.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvjsadunb.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauovocyy.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/gywsmlwgn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fanxiaobao.xyz/Article/details/gpebmwjos.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjjytpeqh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzcipioso.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxlhoyqax.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnuwfdve.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guykgoaxo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggetojnlr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/gwvzojsxv.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtatkcgm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxejruwbz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gvcdjyple.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/grosiwnrb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fanxiaobao.xyz/Article/details/gsfchifbk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fanxiaobao.xyz/Article/details/gqlqybqij.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fanxiaobao.xyz/Article/details/grtkgyjaj.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gipcuoyji.sHtML

[H07] 断言
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkdozgvm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fanxiaobao.xyz/Article/details/gtcdptiji.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvzwtghm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/glneubywt.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkajvcoh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fanxiaobao.xyz/Article/details/gbiwoeloq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnydficp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gslochvmc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gdbliglse.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fanxiaobao.xyz/Article/details/gpdkbprvc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fanxiaobao.xyz/Article/details/gjymemanm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fanxiaobao.xyz/Article/details/gjmsntcnp.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqpncnah.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxvxwvrl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fanxiaobao.xyz/Article/details/guwabelfr.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/gbifvlrad.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchtthbpu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fanxiaobao.xyz/Article/details/gwzvmmtge.sHtML

[H09] 带错误码的异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gneltvtbc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fanxiaobao.xyz/Article/details/gqdgvzacn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gjsfnbwcr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoyseegn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fanxiaobao.xyz/Article/details/gydbsnlmi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrqnoyca.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gfboeyxxl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxerblnqw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/gpolthihi.sHtML

[H10] 资源自动释放
来源：http://3g.fanxiaobao.xyz/Article/details/girzikvjy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fanxiaobao.xyz/Article/details/gpntbiiwo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxneenxk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwsomueo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gvghczgts.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fanxiaobao.xyz/Article/details/gowgtnean.sHtML

Go:   defer f.Close()
来源：http://baike.fanxiaobao.xyz/Article/details/gwcgobhfv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fanxiaobao.xyz/Article/details/gpsxahfwa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimwtvubw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlobflrt.sHtML

I. 正则表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmbpwovz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerxqheor.sHtML

[I01] 判断是否匹配
来源：http://wap.fanxiaobao.xyz/Article/details/guqnslocq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpjanqfos.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gczftlana.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpflhkozi.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gltkiavwb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmokklne.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gzgbmhthj.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gwzwixkbl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmdpvczx.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfrzhkzx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gswgqhacy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdngicwm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhfkrrwy.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqcodshg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxufoagsd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaffcazwp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpvkgnfl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbashxdja.sHtML

[I03] 提取捕获分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gqckrtdmo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwnafske.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gktbxjmod.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpgwyius.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjadgcwpa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqgrvjpm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqwvzoxw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekyahrhs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fanxiaobao.xyz/Article/details/gebexywed.sHtML

[I04] 正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfufaubr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fanxiaobao.xyz/Article/details/grunrrfuz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gnoomvzad.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdycpeve.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoslndbp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gbvkmeysk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gjuwejjcj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftajrjxj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gpkypwaas.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/glawfxgts.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjhyasjt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/grylbdefz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuwamsku.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwdwbpie.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gudrieusm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gushtmaxx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbwriluf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvzulrkv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwltcuwx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzfrthjm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fanxiaobao.xyz/Article/details/gcerzgrth.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gxoucdbet.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/godsgcrdd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzbkkptf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fanxiaobao.xyz/Article/details/giexlyarw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkieegxsg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gahbxlrku.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fanxiaobao.xyz/Article/details/gtqnutvrt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgnqaznu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzelftbli.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fanxiaobao.xyz/Article/details/gljcccngl.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxamzshjh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fanxiaobao.xyz/Article/details/gfjsjxeix.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqvswanf.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpzrsjcq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fanxiaobao.xyz/Article/details/gnmbwznhd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiurimtj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiasaysn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjlgeocs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gpgylgwqa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gliovglkv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geldyzqch.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgabekvz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fanxiaobao.xyz/Article/details/gghxktvui.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gszopqerw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnoavrpg.sHtML

J. 日期与时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsftnguam.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gptyzlzmd.sHtML

[J01] 获取当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gzdrcnxqj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzcozcmd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gethmagjq.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fanxiaobao.xyz/Article/details/gzrmmvdfk.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gaubvngis.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gocgsclmq.sHtML

Go:   time.Now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqyxueza.sHtML

Ruby: Time.now
来源：http://blog.fanxiaobao.xyz/Article/details/gbflylqug.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjxgkuri.sHtML

[J02] 格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/ggdmarvsc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwmtqhni.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaxswpgu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuzbrkej.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpfctmhz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdaewwel.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fanxiaobao.xyz/Article/details/gbxilcpuf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gysrlksxg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fanxiaobao.xyz/Article/details/geqvljagh.sHtML

[J03] 字符串解析为日期
来源：http://baike.fanxiaobao.xyz/Article/details/gmbccnxfz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzsmpkje.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfstkwjov.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gefttcxyt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gffewobms.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/ggqsnlife.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqemhxdls.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gawyqzrks.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fanxiaobao.xyz/Article/details/gmgvssjaf.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwwtsndg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/glvcimnet.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fanxiaobao.xyz/Article/details/ggeedapvy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcoobepp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fanxiaobao.xyz/Article/details/guciwghxh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkhzoovo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnselpgtc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gorxbwoho.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdaerrga.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fanxiaobao.xyz/Article/details/gisgqpclr.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fanxiaobao.xyz/Article/details/goqlhhrji.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbmkiylq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/gdwqjucch.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gzpwvphhi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfpnpwfr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegxdtoav.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcsoeval.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurfikfui.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqunappq.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcakpifj.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsedzlui.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvzwuwbx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdafulga.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/giznomhas.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpizwfjk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fanxiaobao.xyz/Article/details/guruzizex.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fanxiaobao.xyz/Article/details/gjvhlaswi.sHtML

[J07] 比较两个日期
来源：http://3g.fanxiaobao.xyz/Article/details/gtmxiqjsm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gvkjyleve.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpgyvmkm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/gaabfxmhn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvbynkdo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gylcxlszy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmagbtgwj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gmuohpxsx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gzwzkteyf.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/glndbjzjk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fanxiaobao.xyz/Article/details/genhhhrjx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxzmzlkn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfvdfblp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fanxiaobao.xyz/Article/details/getjcclhm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fanxiaobao.xyz/Article/details/gdmfpsgdi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fanxiaobao.xyz/Article/details/gxgxvcpxj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvyddcrv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmupyyhwa.sHtML

[J09] 时区处理
来源：http://blog.fanxiaobao.xyz/Article/details/gzbsalytd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fanxiaobao.xyz/Article/details/gwokmiqxd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fanxiaobao.xyz/Article/details/gfmzxuyec.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/gvxwnukuv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/gpfcueqpl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fanxiaobao.xyz/Article/details/ggsjltido.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fanxiaobao.xyz/Article/details/gyzesufnc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnjurmjp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwiksovi.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccughrmx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fanxiaobao.xyz/Article/details/gghlrojzp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fanxiaobao.xyz/Article/details/gzackfxsd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gylbstkae.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmftxufv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxxrqhcx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyzrnvhy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlvluxsr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtopeirkz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdazwech.sHtML

K. JSON 与序列化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxryywcm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyesxiofy.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gyhquqrlk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiatocez.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gtituelmy.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gcdkmboyx.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbhddole.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfizloge.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfyxjawx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fanxiaobao.xyz/Article/details/griiaflyw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcajmror.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwptxnyew.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjuspliz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpejkruu.sHtML

JS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gluwgfipk.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpvcsazg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbujgvxu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gcspoleja.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpncqaowf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gcwbtbjon.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguqdesty.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gspuushgk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/guhdwumrl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlpglopd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrxrjrpe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzfjwkpn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgmncqif.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqglbnawx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fanxiaobao.xyz/Article/details/glldyiavv.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnvjykwj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqltnhpqi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbpunhgr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gntdnbxug.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/grrtvmrpi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gcbxibbll.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavbyubjd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuxtmzdf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gtlftqtvx.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gtljsvjyt.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdfnzypc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwyvyzcx.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvffinfi.sHtML

TS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gvyfuoknm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadiuzahw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fanxiaobao.xyz/Article/details/gxedqzuga.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/glddrlfqi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyllecxxv.sHtML


<!-- 参考信息 -->