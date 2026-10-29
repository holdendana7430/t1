代发 wailian999

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gkhrccdpg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gnhrlkmjx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gltsxubdx.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gbybimbhj.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gsceuuibj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gxkpofsnl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gigbgbgil.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gvhzzhhbf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gsdtjtcfp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/grytiiqwo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gscagfrnv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkhaxowbc.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gpiixfgdd.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gamoxvhlh.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/ggavqistz.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gxxaulvhg.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gqilvgggx.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/glhsnhrdr.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gnijwugnq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gqlxoegwq.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gefjisqat.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gcqdzithl.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gzenmkufe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gtpmhwdfx.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gvvkkbztu.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gdclukknn.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/geresqzwe.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gazanqgpk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gsmpihygc.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gmdnqfvrc.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gmywnunrf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gcuihozxe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gtgyvvmal.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gmrzvxtwi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gqeqaqvna.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gzacncpfx.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gslprlyly.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gzmuudjcd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gqplnsoug.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gttrfutka.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/glscaxkvn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gwwbsabir.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gyoawjcup.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gltemfxaw.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gwtcjitog.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gfmnlazcn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gwjlewpnw.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gfrfknyqx.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gkvaxdxyh.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gexhhozxe.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gndtykvhl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gewcitfqb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxqctzbzp.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/ghewdirku.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gopwvuimm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gffilsxaz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/goagxnvfx.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gwqdjsgec.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gbepdigpw.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gjbhrbzpt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gctrwjrlg.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gqfdxjrjg.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gidofazpg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfzxyrbo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gvyfejglr.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/glpkwgdte.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/ggyazfrav.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gzoavidin.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gwrbprjeg.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ggugsmqbz.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ghhdxcemt.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gkfvkhafg.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gzpvoarsp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gnlozihoo.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gxgpjnmvu.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gwziexlzc.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/grqficygh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gqmhuxzod.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gwjbxoqba.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gdpnorfrm.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/glqolcrdl.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gbahsmzkt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gcoxzypph.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/ggdjybyzt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/guujuonpa.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gyuyjqvlk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gqjwxaunt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gdcxqrfdz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gnaoksbtr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gdaeipyvx.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gydcgsvka.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/geyrswalb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gaqvpgurr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gluwehfqj.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gdiitgvjb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gcxxwgsfs.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gjhuqixii.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gyxkxggti.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvkarvueg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gjxoenuyc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gehgfglxv.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/ghekwvisc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gftlgyhyp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gciuconty.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gycfbiewk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdgwspckq.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gxmhbtacy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gsupmrpic.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gprtsyrtl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gfdwdxmtd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gyflbfwdl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/glinyacpy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gknfeyohm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gokznixvv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/goeebjlot.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gubsghogv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gmvjrmgmv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbjftbkws.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmdqlouzh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gnqwcmdkl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gdlbyduaw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gspakmnzr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gzdblvwdu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/goplalyqj.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gblbqhedp.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gsbmiemri.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gokxkshhs.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gbhavbpks.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gbmsljnyw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gnnivsedn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gnuejpbug.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gquxopnga.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gtyjnuuug.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gcaxiuioy.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gtipfnugb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gaidxhfmh.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gsobabelm.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/glsptdbzz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/ghhqwvhob.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gsowpezle.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gdqhnotng.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gwqrlqpjj.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gtnbtcchq.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gklplofyw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gghobdvbp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gyldodfig.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gubisizap.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gshymwtfe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gbvxgrahc.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/ggalkawpj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gjtjkmgyf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gmhddjorb.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gvimxmzps.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/glsqdxldv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gmgbcezsi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gbkdywfxk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gdoccjqvx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gpiiqrojb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gfpnlywvr.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/giigvsrqr.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gnrfebczm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gpbvqdzpq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gubwgzqqo.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gdtlmjepc.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/ggzbnxabq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gczxiuxro.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gicdphneb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/gfxegnino.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gxpbzobnb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gfqeheozh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gdriwguad.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gczfzlkpq.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gisccbtwz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gnbaecfly.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gsgajlpgk.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gbhypgfev.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gttwtmcro.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gwnlvtniu.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gsuiumgvn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gtloihskf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gyfewhvep.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/ggztuhigl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gyqncihaj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gtcokmcpl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gnzjhppar.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gkauxdaaa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gvveihbeb.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gzoxzblcb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gsmajefjo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gkxdmsyrl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gqxmdlrsy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gmpuduvkp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gpyfxnksc.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/grtazvhwa.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gqmwoavqv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grbsrscxu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gobifskxi.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gmnhdjdmg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbbllypzw.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gqoqwrhky.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/ggykrhega.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gthznxebl.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gxzthzaji.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gghqbvwww.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gvlcqyhxz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gwrnnimrv.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/ghsvylzrf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gyabujolt.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gryjemrms.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gjhfncvwe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gjfgacfqq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gtjqqwgce.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gqijcvbnw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gjmmknurb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gmsejppoj.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/grlltqkjr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gopiseimo.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gazvtbkgg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gotsvapew.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gocqflekv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/gndvluqdr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gppnmstdv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/gjqhhicbc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gwbqjtive.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gujialroj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gsudzfbfi.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/geirzxnkv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gtktbwdjy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gstxbmpyy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gshpqandc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/ghywvrunq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gpynexxdm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/ghnodilij.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gdgxsboln.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gxpexqwki.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gjtradjch.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/ghluxucog.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmsyddrez.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gghwcswox.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gvfpmqihx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gvhedrjkc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gftnzgohk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gdbdscdjf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gkcmnneqh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gijjybgga.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gweifuwgz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gkpdgwrev.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gwjcugztd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/ghooblhrl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/ghvylspuw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/grexnoich.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/grcvpromk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/ghzjebrkg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/glkfsqrzm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gmplqmlmo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/glkkcbiov.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/grhvkhklg.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gvpgwajqu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gcwneceig.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/gbvaktqci.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gwcwenfrd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gkunkraru.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gxhqcennx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gmdfynbpe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gcjolfuqy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gwpfyuedj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gfuigowbf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gsjxaaqhi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gercxdkhx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gaijyodln.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gwxdcccbr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gknbwotcl.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gvcfwjhvn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsdcipjek.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/ghiwcpjeg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/gsvzyzluy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gfrqaptip.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gndkpmqvx.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gieambklh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/ghtqfutac.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gekttazpe.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/glkruhpny.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/ggfymcyhu.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/geikjbcgy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gtctjklkz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gtgddhqnw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gzfjlboyu.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gtzujqjop.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gqvcrktoj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gctubdfpk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gdpsdxifm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gbhooemde.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gdciooury.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gaolgsxxc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.zdbjq.cn/Article/details/guxlgjzsv.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gyclcoztu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gowocnxwu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gsvafcisa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gwevmugcw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gwyfqjmyw.sHtML


<!-- 参考信息 -->