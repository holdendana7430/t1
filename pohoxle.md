代发 wailian999

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gsxeezeld.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmrqcgs.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/ggpwjtsqd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/glcluqtur.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gybdbqpuo.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gjuaoarwq.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/guchubcfk.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gosttjvjt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/giabyjblt.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gpnzzrutq.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gqceczhtl.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gmdvzjpyi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gkahjjljf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gqfqfkfxe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gczbohvlg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbpgnopz.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/galzpeuym.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gvysyquia.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/guyexsrmj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gswgltbxi.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gchregzuo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gvevnivtn.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gwielpzlm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gldzbxrbb.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gdsfcpklr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gpgllxrgs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/ghnhbthfi.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/giukhvaul.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gsachopkj.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/guhkqpuqs.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/glwinbbve.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gmndvjfed.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gombxpuqq.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gwmqpabhd.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gecyvesgt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/galgkrfzx.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/givmgctof.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gqunbfgtd.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/ghmgxhawp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gvjbultya.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gzfgbfyze.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gnwiaggeo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnnpjzcsv.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gojmpmcgw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gfczwymtc.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gvvfqxfmz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gyahbjciu.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gqcbboqld.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/guihbwycc.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gtwgcmdnv.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gmlencndi.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gtsrxassg.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/guncfpton.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gscnxszms.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/goqqehdmj.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gextneloj.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gdmhokgrp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gzgljfldg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/ggwmpjllr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gjolibhcw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gbalkwjnj.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gzjgxgluc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gzvuugvts.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gdhqfnktj.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gvzdiuceq.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gogkbapwv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gejyvwndp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gzjvqtfxl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gvvjvwvlw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/ghzlbfysz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gxdmdvcju.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gtbbzlewf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/grwfdgweh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gyqjcjqpc.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gdmbvietz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gvygymphh.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gnkkubnnq.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gdjnuuzgz.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gguupjboz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gpepgmjzw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gcfcriszu.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gjjzgmsbw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/grpcazkgg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gustlckeo.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gojnvvixv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsuzkaoyd.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gorgavnck.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gzxqexldc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gpjgiwffk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/geicltxwp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/goansiscd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gquwgkoam.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gzuwftntk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gpireuspy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gdmjyatjh.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gfvyfqgqh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gpafodfak.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gtxiehacb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grxhzplni.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grlxtunkv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/glpzplmrr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/goqbptibz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/glxzvzwih.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmoqotwrl.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gliiosvxd.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gkkqfjsun.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmfioqrhd.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gtnjxejla.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gjhdocfbl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gnjutivlm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gxnzyahah.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gfzofaeic.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbdkzogcp.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gfeyvvpnz.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gzkkrixix.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gmbomhutc.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gayadlnqu.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gpysfkewv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/grqgovpgz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gijksmyfv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gyehupxcd.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gtvyaskdi.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gbjjmufdc.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gdauezmga.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/genvwryvo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gvsygidzm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gqwcapeaj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/grsnyhhvr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gqghpfyrv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gbpocqqen.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gwioczrfs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gvtrbczaz.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/glbannnhv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gasmnqhun.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gydohaqnz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/ggekmznsm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gnlgbwfie.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/glhchottz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gyibqvpam.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gnrirysal.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gzxstqxzl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gnhgwbmvh.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/geglastkw.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gxjpmtabw.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/guwetsdys.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gcfynbyte.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gudkanidu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gnlqpkpmu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzwywriq.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gdjqrmhyj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gfgpayxwx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gbwqciwmq.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gwyygmtrw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gsiquqyux.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gckaqjqhu.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/guorbaagy.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gnjoodnfx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gaqorrykj.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gmxtwdsrg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gdlgkjeug.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gvwtrxmke.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gwzvxtzir.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gglgsxarf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/glbyoqhmi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/ggimmqxkj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gxlstaifr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gewhueejq.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gknfvkjfx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gycoovxco.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gxrgbvdca.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gxyxhdhtw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gpdetcdxj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gvhblleaj.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gsypotpjy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gqugwrbbx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkavsatzl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaontenjd.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gfrhffyda.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtaosracl.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/ggjlgacjh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gwgkqxvju.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gioiejtly.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gdoneoeyp.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/guihmsnjd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/grkzdfwcf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/ghybfrfdq.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gnvvsmnix.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/ggnksjxgd.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gbbezjapz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gjaxyvpmc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gxjraccrc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gikniokvu.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gsgwmrkfp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gtvzxfpfz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gelklkqac.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/ggogxkyhb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gdfqubojg.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/grsjixltz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gditolzmr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gcztqewjk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gwjvthefa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/grgfneotm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gzlzppogm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gvpaipvhx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gbimyybyd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gsepljwos.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gcfltcydz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/ggvtpgvad.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gxssqxohe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gntcbmuox.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gjtodwhpy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/glpfsatdb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gyerbelzj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/grrygzthh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/ghsvmjdxr.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gvszccnvt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gckdgvqls.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gdtswdjno.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gulhgnbkf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gmcqzonkj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/ggsrygedi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/geixwllbu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/glxokrhbe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fehbvm.com/Article/details/gwejtqfcg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gwflghojs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gyjlrpamr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/grgwyulyl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gbuitszft.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/golyjpatv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/ghcxseoam.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/guqqzqfyb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/glyxozqym.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gxrjhunmt.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gulhkhqvu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/gdmuwcggu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gssqytouo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gcspmbthd.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gnctmyrxk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gkczrqahi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gngumfycg.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gxexosacy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gvevuvcki.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/giulqtxdf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gahprgrmt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gnpzspomy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/ggmzovqbi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gziixiurf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gijnslqis.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/grmzedicu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gehckizow.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gnrgmnoej.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glkcnyghb.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gcxhmvliz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkxqtatlc.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/ggiatyglj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/glaldfzcs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gdkhowunz.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/ghefbbfft.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gjfnzqqkm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.hesvh.cn/Article/details/ghidmcrkx.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/ggqehfoqh.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/ghrhtqwgl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gvjkgejmv.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/guateqjal.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gnfpbkvdv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gjbvgrmei.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/gjakcknsv.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gvoqherix.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gchgdbzmy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gewlamuar.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/grprjmbcx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gphqlqdkw.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/ggooduztu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gmpfhfzoy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gaajrgjrk.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/geckyutpx.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gbfjlihgd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/guxlibadv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gtgumgkyy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gsodhrrxq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gfrejlmwd.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gyoxhfppv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gazkluaox.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gnnnfdeex.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gscymofks.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gmanpwjjz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gblienkkv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfdwgpmil.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gupztofvv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gsarrxtgm.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gefablcek.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gltevtfep.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gkyslgrna.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gyapalokx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gfhgqhuin.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gopagzvif.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gayywewjo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gwhguqpfy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/goalghufr.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gnsgqfoib.sHtML


<!-- 参考信息 -->