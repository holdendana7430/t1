代发 wailian999

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gkuyigdhh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/guatrfpoi.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gkqciizzv.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gofyipbcy.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/ghinhffmj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gcnsiluka.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/grhjxcwpr.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/goupxsmjp.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/guylmlqzc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/grafewtnc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gloqhfnua.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gtleojiec.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/glydyzwro.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/giesveoca.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmuawwyb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gyogjucuj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gexhuocpk.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gojtuqbzd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gvossmvyc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyxwyupja.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gudlxfqkn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gjmmthlga.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/glfhtizna.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gpbypgzrl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gufzcyhus.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/govdfplmx.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gsydvvozg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/ghikoqjzo.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gonruwewg.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghzysuhlb.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gnlmjrdyc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gynlcixcp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gubhiymay.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gqwoybqyo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/glstwaiop.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gicwlvgmi.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gtgprhjqx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxsdgowgt.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gmtdknrjv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/glczxbtvk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/guokczxmi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gymnlkojb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gtlldthao.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gottoovux.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gbrcgjdwt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gokfpulbh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gqdeyosgf.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/glajgdvln.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gdovqfwjp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtvdrvfax.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gqiuztejc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gxdtodiya.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gicudjzpv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gsyvyfbck.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gripipygz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gehysklgp.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gihnmzhth.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/glfwnhkbr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gxfzbdlnd.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gsachxhpa.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gxkrubyjr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gtbmgtkoo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gdxhamwlu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gfwnddepo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gsxhgnblu.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gpegbxhmv.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gqdyeutym.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gjzgahiel.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gfcplcpef.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gwkidehzf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gplsrrtgv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gvgwcmful.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/ghuxlfztg.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gobgotjix.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gmtqhejnt.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gqgtdnvzt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gljgyjffl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gpsqhqzjz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gvzaoroza.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/ghbfajajp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gtftchpao.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/grkaglnqh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gkfgrwekt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gxmxkilgp.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gpthqtvbo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gxudwpgvz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gewxotmls.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/giyeamvuu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gjrzwofur.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gxqmhnvhy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gpbsxznkn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gyrayltkd.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gvfnavruv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gsrpcrxsp.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gzlnfcppl.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gfmsakjtt.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gaxarccfn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gtcodoutc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gvrrbeuif.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gdvyemcvj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gywftyfuv.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gikqnobtw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/grhcylqbk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gzvzeidkt.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gsncvuoex.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gmgfyhsot.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gjkqxfqms.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gbcdeitvs.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gjfjmvefc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gdgrltmye.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/glotnnuia.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gztkayjgo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gklspgkaq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/ghftschir.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gwidhpuxx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gvqensflb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/glwionxiw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gqmicerad.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gsyigaqkb.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/ggcosynyw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gxamwtbhb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gqvhxcfmd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gphcfmmsm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gvjpkogra.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gigmkhbqp.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gzslamdsk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gxeroeola.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkokebljn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfvajwzwd.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gprkfqjcl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grxiviheg.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gldzibwqm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gsdcmpcse.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gnogttsul.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gtowlwxzj.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gjhxrridm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gkdicnfpj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/ghkuzodkn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gjvbnlzst.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gyxzbdghz.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gfpuoelid.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gpphhgjti.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/grkihcdlk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gmcoradfj.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/ghwwyxvsm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gqvjbhysf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/galabdkqq.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gpvazeagj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/granmemmi.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gkkqibjss.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gvfqquxbp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gyjzgjblq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gerjjiqox.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/geporgxmf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/glrormcsx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gizqmuywr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gbfjcpmjl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/goyxoamho.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/grskhxdxg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxuwpnpd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gjwhjrawv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gekqzhkbo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gxnmeulhb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gqwuicdly.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/ghzeamhgq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gkfufqcpa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gagbleaef.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/glslrkaud.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gyajinmvr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gcvdqzpze.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gapakyflv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gtbdpltck.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gfqndytky.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gdthzgxxu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gcfsdakbj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/glcdgeyxk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/goubghsgn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gjjrsmxlg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/ggfyaburz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/goohxxwnr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/glmyhsbca.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gbldamtsl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/ggawabepm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gkigbyqhv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gdptkgkrd.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gzltxqvam.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gxnzydeca.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gooqkgchw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gnienpmbh.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/ghihzobys.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gtlonrvqh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/geejciskm.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gzkmeqvqs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gnhlgobss.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/geusyyqaw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gjwpcmvbr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gxrffgkkj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gyoycjuel.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gdvfqwaye.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/geepnrqdg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/goncidqad.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/gkqydfyhb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gxndwaoqu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/garlqjfrx.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gtqneyxqp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gobgcnbja.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gsljfrbzr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gheyjexsq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/golmuwsih.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gbsmbslts.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gizafjngy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gqtrjgvry.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/gqdgkqhte.sHtML

Ruby: Time.now
来源：http://www.m.share.hesvh.cn/Article/details/gylyodqbo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gucvnosaq.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gssdftufj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gzzjjgzrj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gjozcsdsn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/gigvvuwdq.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/gszhbyghd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gvzpzgeyt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/glsinlwds.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gzilzjilv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/ggesaynzy.sHtML

[J03] 字符串解析为日期
来源：http://wap.zdbjq.cn/Article/details/gdjdjwgxs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gpqvxyysi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gexahqwgz.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gigudwhjb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gvttpbwlz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gvvqrgwzy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gzamflseq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gvdensdbu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gwukmafje.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gjhfxsvwv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gxyzsvpyy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gxdssdzfr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/gaouqxkps.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gbmtjoydd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gopgseibx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/ggrofcltn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gtybcmscd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gwhfzhwmo.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gbhnisbnl.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/glufokvjj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gidexrzjw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/glnaiwejj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gfnybqvir.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/gqrfckutr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gtvmulrog.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/ghdkxxkyi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/guwdqckwa.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gtbhhbhoj.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.zdbjq.cn/Article/details/gkwuayagp.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/glshgsymq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gowugciqc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gouivjrzv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gvbigdkgz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gagcxxxps.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gbkzrpfgi.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.zdbjq.cn/Article/details/gerumvfik.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gytactkga.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gzsposhbg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gddsrxjmu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/glhysxdre.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gcoxqtavl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/ggrgxwous.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gcjnhkqju.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/glmsrlezt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gcbhlagoz.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gdmxndeje.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gbpdepvzx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gxaupuvtj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/goihdjqsf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gdafdyrco.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gsrwdtalz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/gsmzjhyqf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/ggchpgkcw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gvwelqwjx.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gdggiefeu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gjuijpsnv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gevyidtqo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/goydxpjgy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gzpmhnbrq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gzslcekwj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gmkbibwug.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gzthylaks.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gokzqrdtr.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gggwylzha.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gsepnzmao.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/ghtllrusy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/glftwladc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gslafzfoe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/ghejhhutt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gqgkdkufl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/glzvaebll.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gwlgqkjkv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpyrcvlzb.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gpvrsmeqj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gizhawffc.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gfqhtkxbf.sHtML


<!-- 参考信息 -->