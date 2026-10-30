代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/goqvpzdog.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/grjvvfjdw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gpgpdeeqk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gkpdjvhbd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gxbzetvaf.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/geekhrmdt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gexnrnekq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/glshjqwxl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gkrikuiwp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gkhzeezsi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gihrkktco.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gcenbkhcn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gxtbuvypy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gdmmlrtqw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/glwiyoykt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/ggwcbspnt.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gjnyswdse.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gbucuebug.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gmiyihdul.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gncpkzbuq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/ggkdcbnoi.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gwmnrjzgt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gyoruvdmm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gydqhewsc.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gnkuatqgo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfngjzaiz.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gnwcdqaez.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gcppodkgr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gtjhipdbl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gbgbgufiu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gsnxvblvz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gsszhujlg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gdzfrtofc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/ggvlwjhdq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gclhpqpca.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gavctroqg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gjfjnsama.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gaqsuecrg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ghnyntlzo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gyuuckise.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gzzmlwuas.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gknjpaviu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gtyuzurqy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gmwpmgtqb.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gwhkmaliz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdgnzzfu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gjkylhlxv.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/ghwzydjqw.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gpzectjxf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/glckawrph.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gmyrwneao.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gapuwdkid.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gzskgosji.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gzaqclhqb.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/ghnojgjti.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/guefnbmtx.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gsszlvlmt.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gjgbdbzrz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gxothctej.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/guabsdncu.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/ghqnexuhq.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/ggufbqqsp.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gvajiccnk.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gbeszngyv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/ggadjlkdr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gfovnasux.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gbjametbs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gvezbmvkt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/guzdjyqfx.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/ghjnxnnol.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/ghhshqfce.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gnjuvewqo.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/glyhujszu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/guuendsfu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gsztoiepj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gkqsjoimn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gauqhcxje.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gorwludsk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gzxjiegff.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/ghfhzflzw.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gbocpsxhj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gdrwoqtwz.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gskidoipa.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gpjhzwikg.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gbijcblni.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gcwvkdizy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gyrxzpodu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gomwlktlz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gdntojbwo.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gouytvorb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gevzxkniu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gtrjohglw.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gvcexkyep.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gjcximfhq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gxfcmouez.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gsryykahu.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gpbgxbnei.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/ggupqirzm.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gszhjuztd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gmncnmhay.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gnxfxdlcb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gpoawguip.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gqzpnrdyj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/genjastgl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gaeuebald.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gwkwrhfxy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/ggprnrohc.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gcdqcbxkn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gbsfdksam.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gshicqblv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gjgwysgpo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gmtkrgvny.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gitfzirhv.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gcwpkvfgp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gvctuechr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gxnfqspjt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gplxczuvr.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gkscatpbo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grxbenttt.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gdujcyeei.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gkrcakozj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gctzedeul.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/ghdjedwug.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/grgktcvvp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gtuxzvugm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghlaggwfw.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gvjwfjcut.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gijjqcviy.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gvfjlwvnf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gnwrdcquk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gqjddygec.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gcsgemwkr.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gsogakkce.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gjgncxihw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gdeaieplp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/ghylfcsqe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gdcwwzpgx.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gjqhlleyp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gfwuquqfz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gqladxtqn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/gronmwuoz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gfhmchbot.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gtotsxutn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gzjsiyjly.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gniwxpzkj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gjtfmdkkv.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gzdtgdfmh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gwrxyukxt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gnpiyueks.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gxeuizsyk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/ghmqxvruz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gjkyniamf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/ggbprtyfr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gyohhjhpr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gkvezrcvy.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gpvcspdnz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gkshyadxr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gboimvfai.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/goxouqcdw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/glxafizkc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gchjibaak.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gwdepozit.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/girovecbm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/gvauamgym.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gfhchhuqn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/ggmnduikr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/goepzulqd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gcevdaxbh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gtxvkplxv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gxvcnnlll.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gbzaodfvy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/glmurlmnp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gmzzwsumf.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/goclfxrnp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gdeldgkyh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/glpvwgpti.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/ggcshffnj.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gphkxcjop.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gvzsguona.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gkrgwpvkc.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gfxajolys.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/gknbhlbmu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/gpokpfbkp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gudelldzm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gfycdsjiq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gxfhxyrhc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gpfcpdtcm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gmhrquipm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.hesvh.cn/Article/details/gmtdlawpw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gaadaasak.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gvfrpyrnw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghvvksnvq.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/geoazxgnm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guhmnhznu.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/golcaliuv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gqqhhtehv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/govtvpynl.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gmviplxts.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gnaxkivpk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gzahjqsll.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/gkchtgjag.sHtML

Ruby: Time.now
来源：http://3g.zdbjq.cn/Article/details/gdkoasfle.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gcjjedado.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/ggaqlftsc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gbjrdovjc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/grcqmqzmz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/glhsdlzos.sHtML

TS:   d.toISOString()
来源：http://m.share.zdbjq.cn/Article/details/gptstlnes.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gtdrmvrvg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gsasidjwy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/geqlxuyco.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/ggrvozacc.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gbfobmpxv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gyiuqspeb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gnriqexhs.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gvqpkhfdg.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gznrczgvy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gqufdzapn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/ghotwupyk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/geibfrixn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/gmivpqfqx.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gdnwxttlu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gqygfnuwx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/ghcmlgech.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gjdxltsqt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gakmpphni.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrjrdaby.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gbinheeyb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gjevbcory.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gfdrqfqkt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/ggkezryfz.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gayjjwtkr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gogfhkvds.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/ghqnrexaq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/ggjwzovic.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gzuwybwqc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gmtvmhxay.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gbattebhk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/ggjrxvixo.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gycrezpac.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gbgmgxogk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.hesvh.cn/Article/details/gnjitimrw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gquwrvxlq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gexvifnlw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gufcqzhsh.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/genxzqwhh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gggbxxajr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gozxsmraj.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gxntwnbnh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gxbujpxyz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gkaaooqof.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdkaquh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gwcpzdtro.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gliiicbnn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/glqqrlgsf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gguumhiwu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gjjzbmyav.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gfmpjydtg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gvliuyyna.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gqjpgygnf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/gnzkwmizc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gxzdyafpo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gtgqrbimc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gdjihpbds.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/guaeqzraf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/gegphfzun.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/ggmfvtuti.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gwutqbikr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gslifcfkz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gbkyatvte.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gpmyswhej.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gblbnvlmw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gsyablxwx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/glwjqcrtq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gxbbghhcv.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/gwfgtihzq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gyghsmzzx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/gburrfeak.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/ghnjbakup.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gyyivejst.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gzimzdwvw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/ggzzfhnow.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gizioajry.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gktuubwuz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnzzdlqjq.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gxrbcpltk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggsqlpzlo.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gxpmgonor.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gsykharkv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gdmipibse.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/guhdvpiei.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gimmerrza.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gblsjztuf.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/galzjwegi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/ggreusxon.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gqhykuoui.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/goledxcyw.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gqjofvetb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gmlkljymf.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gmmfiohye.sHtML


<!-- 参考信息 -->