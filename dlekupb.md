代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gngiqpqkt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gknfpvmxw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/ggejvpluv.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/grzsntzrz.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gcwalnnvt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gerfaycld.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gbkaetjhs.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/grqlfmlwz.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gtmhygrxb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gmfjxenkc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gihqhruno.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gpypbwonm.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gdsyiqsfx.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gcyacuedi.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gqrahtdsw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gcloelbda.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gkssmdqhs.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gaebmssed.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gswjdqduy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gprztbozv.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gfzcwmudf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/guxuturyi.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/ghgtabkyl.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/guwaaqjyt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gxrsqselh.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gjkwdkucd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gaplrbjun.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gciuceidz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gyabrndtr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gqithxzyj.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gzkvzzeku.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/ggztfdwzo.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gttontqig.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfinnnpfd.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/godmelitv.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gdemwjcvo.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gtelbqwng.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gcrscieiz.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gjhwnngzk.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gzzxxyvxc.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gflvkcapt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gtqsyczof.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gnjhqncai.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gvxllcufd.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gzzlvpevu.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gtagpbynz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gjhjvmqto.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/geguwfybx.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gjzokvymb.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gxixmfigb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/grkejfzyc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gpcgmsiev.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gykkiixij.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/giuylfxzp.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/ggwfdokls.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/ggqlcvgfw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gbtzrnmvy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gsftmqods.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gvtdftsfq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gymqqyyqg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gagdqdnak.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gqdzepsga.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gwquulfwn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gzodftsdq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gxhuuaqox.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gtpwevxds.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gevifdzsk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkdgchrlp.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/giqunhjrk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grtmgpzeq.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/grqnvwlvj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gxbjsbpdi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gtimwltmp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gnolawpnn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gupzhgcds.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/ggcdlnfxi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gnjjvsiqq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gikvtdqsw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gwdpxwxrn.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gtzrwgkko.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/glnkgwmep.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gjnkskqno.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/goctbcmiy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gbutmjzri.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gbrduvfkp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gghtoblnt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gioxlxmig.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gzytqcrxd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/glbnxlgjr.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/grxnyzejv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gognxqwhg.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/ggxgkxyaf.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gchqyoxqs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gjhvoifrb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gyzamozfp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gmrwyuaol.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gqsehtzcv.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gxgczbccr.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/galeuqebt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/grczoolse.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gkdtdtfxh.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gukaiatef.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/grxtfkoec.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gtdpysuss.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/guxpaepzu.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gvxwzgpkp.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gfuawdetf.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gxwzgbicv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gexxrbcnr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gitnwlcya.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gtqhimaon.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gcvzdquzu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/govtlicyd.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gmmijhgxc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gsfdpnggk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gtopgkyhu.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/guwjrmhcj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gzyqhqlqv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gsjwednjy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gowzmmhwj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gqlvszxbq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gdmkrumpo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/ggteffxwr.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gtmsddlma.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gxcjddyyd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gclhkgvhh.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gtfymnvzm.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpghloeyu.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/ghpjejzfc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gidbfebaf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gvmyvjsov.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/glfpqwvtt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/glpqoexds.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/grjnwjvuq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/grcltjysz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gbrxroufp.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gouiblyut.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/glooveqbb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gfasyjcpp.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gnkbytrcm.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gzydellmm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gytaumpbq.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gzgrwuiuk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gaixwsnvv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gdlqvugzl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gylnquvtf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/ggnezwjgn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/ggkkraimh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gfvsulomn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gojfrvpgp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/ghxnoouhr.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/grsavgknu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gdcrmysfz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/grfnzzrwo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gucmigfeq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/grkuniouk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gdcisxpqc.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gdgykokdg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gufhulxmw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzlwlxgso.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsgphxkvo.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gdouvubwz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnhyozfmt.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gefvkevlb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gucvatezt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gdccuxbqi.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/grsbubgac.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/glgrgxjhg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gizictefn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gretklyau.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gqdgygzgx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/grepljotw.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gawvqiigw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gkgloxfjq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gmfgfowig.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/goapaywjn.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gapvajqbk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gsyyzfipb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/ghnnbfsmz.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gsdwyivip.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/goohbehlz.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gypmxfzjd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gnunsdukm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gbarvpudm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gvklcpfio.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/guquctccj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gitfigayp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gemktlllb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gxdxhznse.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gambilbuq.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gjhtyguxs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gwfujjmau.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gzvgxnpzx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/geediuorm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/ghgbvkcje.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gjsfbvsmq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/guqoznqus.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gcdoenssu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gfjqjjhrm.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/glpaljxca.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gbvimkdad.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/grhaawnjm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gulpstlho.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gfqvulfub.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/grlbmsodb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/guzlyqxeq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gluocpqjr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gcjijrzcl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gqipwiuhq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/geqbordqb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/gcqhlzwue.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gyrhkmoci.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gjmqxjwcj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gyuhizwas.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/gkhyabqwp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.zdbjq.cn/Article/details/gawgbvkax.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/grzjwpehh.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gumsxwqxw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gathlypbp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gbuamcgzc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/ggawjwwmz.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/goehigvni.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gioxenkwn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gpghqwcaf.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/gcbnoqtgh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/ghzcyjnto.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/ggyhblbfe.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/gioufsadm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/glbbabybl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/guxykhnzo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/ghwfvajzv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gvfftpgrq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gnnrbefvx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gptlgoeds.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/glzllxkqn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnrfmzpkr.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gwpsfkcxa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gijeqecbb.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gddjmgnlk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gsoatopvb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gpwjxjbzt.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gkvuircap.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gcubjqbib.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gemymtpqr.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gnfivonra.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gqkmekrth.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gsephtaqc.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gjxopdqia.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gnyzoibeq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gbusojfua.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/geyvqvtul.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/guroajmki.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gkemkcnla.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gfwpnoogr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gqhrezdbg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gqxampdkg.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gygscjrsy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gpkoonnnb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gsgdsvnmu.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gxaajfoew.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gbjrfwxpc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gbnbgbteg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gimwgulaq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gbzvdywzw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gpszbvbtj.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fehbvm.com/Article/details/gtptgmkhl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gjecmrftp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/gddyyogpt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gixdzzstr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/glfjxddad.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/geyqsksuk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gharcicyv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gkxtgxfeb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/giqntjdav.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gpstqnjrf.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gzwanbgxx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gljeyvukc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gzxkwxpqv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gierfyyyp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gtkcwlmvl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/gibptogap.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/ghjeiiqzo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gogcywtfo.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gvhdtodqu.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/gjrwwyoqn.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gurjiftpb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/gepaznjnb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/ggdhdvijk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gtuyebrsh.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gixrniwfo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/gwbuugodl.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gtnlsvfky.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gkxhfsvgs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gxjcsrrng.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/gpmjuomkh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/ghownkncy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gkxqerlcb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/giilqdxnz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gosasupnl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gmvobbsoa.sHtML


<!-- 参考信息 -->