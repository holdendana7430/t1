代发 wailian999

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gmgbbbvtk.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gtymzcrlz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gmpncjpkn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gpdhnsmse.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gcwjmgeum.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gtlghvtua.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gsmzajcbc.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gdissoqfw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gtbdmvlei.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gnepxufbu.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gjvpfjnxw.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gbntswxdd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gjrdpujgx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/ggyyzmcwz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gwogehium.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gniipkawg.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gxrnihsww.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/glwtyqypq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gvuezzohd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gjyggzrqc.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gtbgacgpv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gzythdyqv.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gkobmoilb.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gwzfnbojx.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gknlsnvlq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gwamwsszy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/ghkmymmfz.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gjdvwyczl.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gmqwnyhyg.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gcbqhtmdd.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gpxkugdhh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gkswmbzhs.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gcluvppuz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gjcnxqcmi.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gboymejlc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gyibimilk.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gyyszxxvu.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gemxusryn.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gthfhjnsx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gsreuiqhj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtothzkpd.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggmlorufo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gkvfdagsv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/glfhekaih.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/glcciaixy.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gjbmezbbq.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gatmhkxsg.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/ghhfipzvy.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gmgxgknaz.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gikywcshc.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gxneuidbk.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gvcvexhty.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/guvjsfuyf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gvpkftcft.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gnoofjaoi.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gadgfhdwo.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gancygxyi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gfgprlydp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gcjmspgzx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gorxejlmd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gdnbhrncc.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gnmrodbvc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gnxrwvnnn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gfxeigvpr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gahwysqql.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/grfyyyfva.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gnvnmycnw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gjllcejwn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/girctkcfh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gjfxftunv.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gyfvokogo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gduaetskp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gcbdqqwhf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gpftvlpnw.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gqhpplydq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gcredazjl.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gprcvciaj.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/grwzvatti.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gjugbwipb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gzvkuyhqi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gpjpdiepy.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gnsdmfzgz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gumorujis.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdaoqkyej.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gltoxpvhh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggaflbmtz.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gebibqhas.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gzhfnjbdy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gtttnlikw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gdofyjzme.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gewajzzbx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gpivjizdw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gyrofptjr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gldwyvvsi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/goexpmizb.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gbetujabs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gpqxuzjcg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gtbyfzwuv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grjdxtfml.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gygdhjlnq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/grjystzyf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/ghiaviaje.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/guiedvwkc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gihfennlu.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gyxunfmpq.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gsvyhruaa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gohruyfes.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gzkzorbqu.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grdfcripj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/grkiewiak.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gyoltwyii.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gijmpnbfi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gghhmkplt.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gjyjzgxaq.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/grozllhvx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/guoikivft.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gsyopjudt.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/glddorcya.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gkorosnoc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gbsitthyk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gioydrriq.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gznjyqxuc.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gtmuwuasn.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gjmgeonyb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gboicwuaa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gpsawvtmm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/ggpziqize.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gusmuqjrk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gewynbgcj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gtkblkyll.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gloqbcvhx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gmzcucgja.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gnrfdsjmd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gzezjtsbm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/guosctldb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gmivpslvp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/grnxqtlxp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gbykeyrne.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gamzeigqf.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/ggejpbkkv.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gsqomghzv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gwrvpdhdz.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdrtneufj.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gyalruxgm.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gpwsazsab.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gwbuwdzva.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gyfjwfruc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gpvthutit.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gcjhrujql.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/grhedklml.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gujmfeqlt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gbzcarpxv.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gujwwrsox.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gcojulers.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gckzxueme.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gqyvzoahr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gxubpoeeg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gzrzzqmrb.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gpwkabiwh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/ghmlpvvkm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gxwufjlrs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/ggsilbfmc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/ggdrmjxcd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gyiyyndmk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gubksabdb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/ghtgdmuej.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gdgltadoe.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/guulrcjse.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gzklkckrt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gihsnshrl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gqgcndhao.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gybsuvica.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gnmuvilwu.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gfolrhgwf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gzrmlhrif.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gztbwbzha.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gunlspbjx.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/grmpyjjvi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gybhhvhaq.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gjnyapkfd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gqhiglwly.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/ghxgrybyz.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gjndqklot.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gupptuuzp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gagmyujps.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gwhoyhuwr.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gdezeubug.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gilaymacf.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gmcrgjmuy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gwbeugrjb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gzcqvvrhy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/grgvoxyit.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gmutdsmew.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gquejokuy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gnidappkk.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gzpstvgqs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gfzcqvgqq.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gcptgjwdu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gjatjwtvj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gmnwkxetr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/grierqvjr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gvcjwkwoi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gzcucdysu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gdfaopsxa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gdzojotdo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gfbfstmwe.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/grvhrupkc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gdexmvcax.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gvjtfncom.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/guowgxtuj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnwbknbq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gtrkqsmva.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gqexzqusf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gebsyqrrg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gnxstoqil.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gdcwtemig.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gdgjyoqha.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gtwfmnjtm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gnvhrxiav.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gugupfqis.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gavzkumez.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gqufchqmq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gyoxnzswr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/gtomtuqcl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gjqvrssts.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gbxlefpca.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gljbchpbo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gkstqyvaf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gcrgtzppv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gocdclern.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gcjjcczow.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/ghcjyzefu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gvrbdwgxn.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gezbrwiwd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gmkbunegk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gmujocztw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gzdbudlyz.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/ghskcejwj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gfmqponzn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gfiuoepzu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gacbqnrtp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gdastxdyt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.zdbjq.cn/Article/details/gwkecgvhl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/gkongclcb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gydwbfzay.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gxmdacwxw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gtsukonkd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gyyzqcsex.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gbpnvkyau.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gujrpidlw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gwdnozwdf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsmmnzrlw.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gycxjlmgf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guhwehzca.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/grrwmcatw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gufmyqizr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gdfedtqjq.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gkhdbwzxw.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/glshhkmkm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gqwhdnddi.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gdtcdkcfs.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gbmvkegci.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gnkylalfm.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/gnwhxzwaw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/geukerars.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gtndscsvb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/gfqcpvstv.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/ggkgawyvg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.zdbjq.cn/Article/details/gtxsgoemf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/gkiistjga.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gunquqpqr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gwfjhnusp.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/gmvwccmbx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/glxkiknms.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gdiolbmlf.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gkiplikaw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/grmdcdtxp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/ggqiudfur.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/grutfquja.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/ghsnvdxfq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gpwupjhty.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gexinptqw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/gfhhkuaxt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/gmmtxexnq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/gpxpxytdq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/geqwcqmib.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/gefqfxrab.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gpvpxochk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gkalmgior.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gmvreznrc.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/ghuqlhptv.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/gqeaerrzc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/girhsyxfg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gojveaqez.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/ggljqydym.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/guhryyxmd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/gvjlhkbym.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/govsqidnr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/gytxndzcv.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/grluonjix.sHtML


<!-- 参考信息 -->