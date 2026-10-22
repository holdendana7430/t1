代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pfhdicfi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2totwjypp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vflqnjvl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zjczskgq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqksaruh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fxlrvufv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ycwenhqj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xnpadzpp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ubswdckv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hufioemk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rydbajhl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pfdvkpka.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2popgxgob.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yrwroydb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2frshuyvw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2pskclaao.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2smhocvwr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mgdkospx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fgkjwily.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2toynpbkd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nabgnhrv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uafytnmx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lhwzodfr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tydnnzya.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bfdddoip.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hstdknpn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bvpwfwji.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2qmowzwxq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2sbajrdug.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fdwasegt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuteobvy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qbssyzvb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vlirjkgg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ragwoazh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbtgdqic.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gsyfgdaj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ubiysyyn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hctcswmd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jgppvkrz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ztwzfsbi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2huskvivj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mjrnpnqs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2sdvowees.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2dwogornd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2odxhbhwa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2acaykdwa.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ijinamte.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2orkwisyx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kymceqwp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ytfpkksn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ffuybbex.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2clcasyft.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ngevlwdq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2plnrvtxk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hefktgfa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2emhgejwi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gxujdddd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbtcssaw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qntsnvwc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hbferccm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2sglsdiws.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pedhwlyk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ayacdwzi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2erilhhxz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lotklumd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nxllhwfd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jqhpyvwu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlegqzub.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wyfvnkhv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2byqgbooz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vnqxeyjh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ghudebcy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ykgzfhnm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nnpvzrqf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gczxmcfi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ooxmxqlo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ofujogmu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2lfinjvxd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2xmveexly.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2phldiqlw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fnihsqse.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ghwblsfu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2bbysmxmi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ofrcidsa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vfesnjzx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxjsfqro.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ytqcdixb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2eagiranh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ylfrgrtf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xitndicz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mmmystxv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gioimqny.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2awlmpcnr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2neaewsav.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vqqyowbd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yfetcudz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rwrkjaez.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2plwhecid.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lmbfjdup.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2omnwddye.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bfhadbik.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lfhdfyuo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nyridbkp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2txkfxcuy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2fzrdvssg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rzsvgjqs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2chiogawc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehiilqny.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pdxzsqvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afhgiljn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2hmdvfvfn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vooisrgy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2liqnypul.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2butqqnmc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kfocsbgt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2xrdudfyk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2asmoqkoh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qphvdquv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqpwjiqs.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xuoezvwb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ycltqkhh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrnxalmh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cvycxfbw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nngwewac.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzgjxqgg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ymmfcxdf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gudosupt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlmljydh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wccofeht.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vdxaybry.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lhsnoixr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dppjvsmv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2faeznkej.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hoghsonl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lnolmbce.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rjknulgz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mdeybkdr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kzhgdupp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xybgfhis.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cxbzpjpu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yzchqfcg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mabydwma.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2utbfedtc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tztubhlg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xvablnbu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ouiojbdc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2tftxjnkz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2dswbzplt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxwecswi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2swmjnfau.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ludrpvkp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziuiwfrb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2mcanvuiz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2smidzlzk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejezvgty.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2rzbgffza.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2rlquclkb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ainylgei.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cdejfeun.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xpyiczlt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2kocjharm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2dpritfni.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvhvjgau.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2sgqcevmx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2kfqkjufs.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fcsuuboe.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fverztco.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bhunkjwg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vaxawcll.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2gbloqtpc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mbjpdlvy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xnafcjte.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lqyhccwl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2jndazclh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2cupvmojd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2pnwxlpzk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ynupwvrv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ucdpguah.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2nkzzjuaw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ulwftbom.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xtrqwytj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2enfxzzsx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2zquxbvdt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2reakidfu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ndcvdfda.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2kcubrqom.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jzyrnqbw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgwmgaca.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zlruobrm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2fnevhgwr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xijcvhgr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xstkguia.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2fpbuqupt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2goynkxcq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ngjusydx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uudmlcgj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2shluknow.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2plpdzkkn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rkgvforj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hlwsibsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2giigewdn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xsuylldm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxinlzba.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2fflsrwag.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxtyyriq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vnxqiymz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2knqishns.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bmsoyzgt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2rkwupnad.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2oshmyfwa.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2exvpsbfe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vgdpqpsf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2uagqlrub.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxeyjsqj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2oxlugsld.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2lnpyazvp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2bwcvwuhl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2obqcibdk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2otvjynza.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2oogewvxo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zmeolngf.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2lslhhanm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2anbgmoxp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2emvxcehn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2jxkbufzi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2feqhyfrd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2mctdnbrb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2uyfugqpi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ltstpdin.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2racihukb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2svrakdzb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2flrxwqws.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2oivpzgxi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2obzcdzec.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2coxqyaux.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2caajwjbf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nnctzaxo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2uvgvivdn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sjeqhaxk.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2gsnyopll.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2zldhsdeo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xryoapak.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zibbofyt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bdqrlmmw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2sgwiofgv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kqlmvlft.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kahlbuxm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2fcdgwtnr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2aejluxov.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gqhprbes.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2thlhowua.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jkmjqnhl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2yswolekc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2lpqztnew.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2hphmmwxd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2uwkyxyuk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gnlwgvpe.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2nbcqwvgq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ohiyoscy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2spgjtbtd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2mhymhhyt.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2lwraazjr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2fhhqvlnm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2vniluxzs.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2rknxnrss.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2vgdiwnwr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2csottmsj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2edszpopy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2qemmeout.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ozcsnqzk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mnxqhzuv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2zfyiggrj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2tkddlcll.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2cojesykg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2otppfxfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csfyyong.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2vxggoziu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drxeseur.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2itqzkevz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2zshansuy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lgpwbknv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ivepnbqe.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2sjlgaino.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2imwgaplo.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2aaeqsofy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2uirrgyql.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2kmaxtinw.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vpmvntbt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fdbooqqo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ukguyfvl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2aywnppjr.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2clzxfuwu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2dfidfkgo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2cylkxoyw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2tzxmhehy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ohgijgxl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2aftmkxis.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ykvjhnui.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2srupftqf.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2unwdrcio.html


<!-- 参考信息 -->