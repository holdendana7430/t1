代发 wailian999

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2frgqfrjz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hmxbxrel.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vjysnesi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2pjkdmpzc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2wimlmegl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yzsjbgja.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hoffhaha.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2sowcwxnb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2yojwmujy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2abtgrqug.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2unsmcioy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lxprlmfe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vobehvat.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2spvsyqwz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2papeveqp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vjbmpmty.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mppbovjp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2seacrihh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lhhsnwuc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2idbggphz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2koclrkue.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2azecqfbw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jcwwknyi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mpotpqgk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xlpantog.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pwngizel.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vjyeulfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abmfhidc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dwgzgcyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esdwcerf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wuucgzss.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ihbvticq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cmvdjqfr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2neiznzby.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzafrttg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2forkrtal.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2uwvxxapx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2aqjbeyvx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2kraceezz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2alkiidpa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2mxddsnpt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ppabqxsq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lvmbtdmr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqlyudbx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rduaudcx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2moxvvmzt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pwauwxhl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2waugumnf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jimymesz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yqqcllbq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xrmvevxj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2avqdukru.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2snpuuozh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mttixbps.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2pdofqejn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2mqeyohew.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tpmwfezp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ohfrqsuu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fqojsibs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdoviwmu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2scebwwsd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dijxfbab.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvupofkd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fzmruocl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xvexafvd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2bejtjcyg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2abjfzlmd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2uokipecz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wxyhblns.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhlhnmli.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pqlvehiy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddndzmze.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2kbrkksaw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2kcqrqpuv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgedkjbo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vyogavlk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2axdzxlfc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fsnyxets.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ewwkeyel.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dfiespfj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ejodcqao.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2nowzpdjn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2marqitpk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zzcncice.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2cobneqez.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pcpzmlai.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zakofbkc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2effmqbsu.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mgqbxbmt.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ciejyaqw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2qubtecaj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fwhmorlo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mmcsrtfo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mirqpile.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2bvuxrmga.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2pixbmnre.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2dsfbouaq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hahabpzq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2sotlojep.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wmwfloyz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xgawhmrr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2yypkxjld.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2gszdyvws.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2vpicpfux.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2bzsxgccj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ooxrnwxa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2iahhutni.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bvktsoaw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hirkvoni.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2wvowprph.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xartiztn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2pweqlsfo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nobuhroa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2hxltipkf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2emflwhwj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fpifwsbi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2xvlpqzgx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2dqjhapbp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2kmdfflat.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zruryqsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuwefuzh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ruudtfhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebjycqwh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2nbwyanfm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2rhqcigkc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bmbfwzvu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hrrdivww.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2khvefmwb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2nywygnuq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxzpjrjn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xmdbjljv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qrtrldpm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wjmptfvy.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2enotjxnb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2fmmuqfef.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2huofiyvb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2spvzlmev.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ssorxzos.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cdqidjoo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2iazhpcpz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dmrwftqr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2nwlgvyto.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2rcighwft.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2awwivkhs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2bhsgvbvy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2xkvuzohk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2vvwugldu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2jrpdlcll.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vjplwlqr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xyovuert.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2mnflleao.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2etwgpzak.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gufgswne.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2wazzackv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fgybqimp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mvdyvtgo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2bhqnrbqi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2uqcmckym.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2tkapwfga.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2totuoqwi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwnsvdf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2klxnhhgl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2incpvcyw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mjjsnkld.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2ebdvlfvo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnpssuhm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2drmsdbdl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qtogsrsd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2vewcooea.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2anlwusms.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2hagzeqyd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jebunukb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2hvcetcsa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2phxziqob.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2dwolhrur.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2iashmcxk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hvwjwolw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2jbjaajhw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2knmbwmew.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2gdlszglr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2zfbgslue.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2dboeqymx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2wrmcwrbc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2krhlerml.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2cqtpgpky.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2coehlzad.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2pspgrjpr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2bobahnyf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2lqdfyrdr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nmfifkus.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vpuovdvj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2dylfcaeu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2sbgxhnkt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dvgswfpb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2yuaighdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eazhfefj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2mtqksnao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewmrvlxc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2uwojsvqr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ovjgmges.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2nqhlunty.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rlwqqfnc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wzoruadz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jfvzvofu.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2wzebocvj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2nphvlhja.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2ipmethmr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mjjhjoad.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xraelqkw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rohjnebu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2fghaocos.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ohwpzopw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2uokgzdrw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2nlhkjfns.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vkrglwvc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ccsmsnng.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2gjiajnun.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2fdzsxudf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2lmnndteg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vlidxhnd.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ksaqnboi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hrhoaofd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gfawxuob.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kjukxybi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2oantbnsg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2esixmofw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mqhonigm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2mtzwhzut.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zegymhvn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vmythuhu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2uaqzjkic.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ybubxhfb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bjiyyest.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2posouhhi.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2wxyiqsxi.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2inuwrnjg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2teouvumk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2kxyiweaw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2uojjpwrd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gyetzeku.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mrddyiid.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2xafddeei.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bfrvojkq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2optaosya.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2vhcoqrcb.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2smmnxtlh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2bctybyzz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ikafiofy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2gdecmvye.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2auxaxnfc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2xiqtvzwx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2wcqvpyhy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ecnjszxs.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dryhtlpv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2toilmswc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2cdqeddwb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2leqztefb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2befazpxk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qywyglqp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2psxdophf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dyucdccl.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2bmzeidqb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2nbmmwftj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2uidwziiy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2qqrdxlrs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2zbfutqsy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mrekjydn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2wtitiabn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2teekivwk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2eeplvkit.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2uhyqmkod.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2khakhzpe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ctemrvrn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ngwukvfb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2iczbxvsf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2lensccin.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ssfjgtyp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2movzsfpi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2sdpojhtx.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2uwlysuvj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2kghuetgh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2mjbvfkeg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvpfsitq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2izzoknnz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2qjbahvjt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2soxtkftb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2cbtqdunt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmoduirg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aldzxtwv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2tyxlbsbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obydkzax.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2jtqmkitp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2juneahfg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ejvwahvn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zqltcako.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qboxtoao.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ewchqvnc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2tvienyca.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2bzgthtjn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2rdihkvro.html


<!-- 参考信息 -->