代发 wailian999

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qfeseakm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kmhebgrv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lcmizkot.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bhtpwxjl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qluhirzb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nxoiianf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bctihmll.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hnoezbid.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3choabkzc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bsguzist.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jjdqvbqt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlikrdna.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqpexnvu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zkesfswz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3iqhxmsvy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vzwlewjk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xurzqkxq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3phrkclba.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lsdlzkmd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ffdhulho.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ayvsjqao.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3psooehdx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ghhixtwy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jxtjetjy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zpraiaid.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3glififbi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nqzobayb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3coybdbly.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwlnqaat.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mnlijaie.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gouojknc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivimftzr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hwhwkmcf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3pkxdkttz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3gbpathkj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3cypsocjk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ifsyganj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xzdtnhxk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kiwqeonh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfgzsfkx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ttqoufix.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xtaihnwc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xmwfjnvh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmbwqzzq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3oheeblzi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ybuphkyx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qsrkelnp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ydtrutly.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uzcqjskd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ystmbtop.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gjtkfobk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zlgvfjbn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mnewxnqm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3lawpwbaq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ucjhemly.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zfffoxzh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irixrnpp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkolelzo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lshfnaxt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fnwoblno.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mjejzwqx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wnvsnlbe.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ijldtrmi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3erhfedjd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgbwhjdg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tuoptlen.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hdezljkw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfmzjrzj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rsrbcemi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mxtewnch.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3eseuxffw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3npwozbon.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qdgvphui.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lkiktxee.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vhjsyttl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dnvumjxp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xymjcevl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3fucywyev.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3eajenici.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kelvyldf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gjugkrca.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gnkggdgn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3cobnucrg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pddmwzzi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wxgpmsjd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnwppehm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3tqeezhna.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3slxbhkpb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3jqmzzkjc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lcsfmvgc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jfasntve.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvrvucao.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bznmodyc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hmjllihq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3iklwxfrr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ywzmvnvn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dipwnqht.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yjgirgvt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3yavdlbyh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ooeozhdn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hzgxledu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mfnwqeyy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wjbnlfoi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3drzapmrp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3xcllpnsw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3yywdjjdi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rntqreli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gghfrtuw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3pzcmmcal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utarihbj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3opvtwtkh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3iygbvbuf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3advvjmgj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxjleoja.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3coupjmjo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3modcrpjx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wjmbrtat.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vycbzqhe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwsaehlm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xiuevkgn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xcgdobgl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wjiwgabk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kopoorlo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kzijdhnp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bcnebuyr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ctqbmdjl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qbbcwzkv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cfqzpwdf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xqclltun.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3cunvucmm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pnjzmqul.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3szvhqoeu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qrtnezxv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qeoygifj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hlfaixam.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vltlhvqr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zmhxnzgf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3iqthmyqy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3xbmzmers.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ustbuqwq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuuicoyk.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rloicblb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gidgxwrq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3amwvdykv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bdyxqego.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3bfgyxgor.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jgyzrfat.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3lysjzlmq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3shogkfbr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dhceiqan.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rsyffrex.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lyapnwzj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxrhhfw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3dkcfsqts.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3mfgypjir.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3qtybkzae.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3myshikyu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3woabesng.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kiifxhww.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zgltkdho.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3btrvywxd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3kmsmfqhz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3azvklwhn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rpzjetou.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3jwxezofx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3bwtgszgr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xbafnnwt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qgyvmtwp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ybrffscd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3szaovbpu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3jymdegfi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gjrcptad.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uspxbkgr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tfcxjndv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3buajzile.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vwxfrrtg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3seqpuntk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cxpbeotq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3luyelmek.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3lhmphrbg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3wromuydz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3bdwlvvag.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3qojkmyfq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fmboylvz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tqpbliji.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3zisobkdv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3wxlqckif.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmmvzkzh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3cwppllin.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3hxzszkfl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vfzygzmb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3toyxrfnj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3muqdruwf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3jfahnmew.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hyoeggjt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jsyvmltq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3avvhsuze.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3gzwvhuew.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3mqyuszok.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uptrjzbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwthtdpr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3oqhmdjky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfwwxmds.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ehzumldd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3quxrhdsr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3csdeyjay.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zyxrleyv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uivyotvt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3nltmikeh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ettatnet.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3aiimxnew.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3sllppnyf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3chpkapsm.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dzcwqykv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3sfnokgvt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3kfroofyu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wqhctycv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3neotnaol.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3heuydroo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vbkmoxoa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vphdssfw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3zmqyjtyb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3dxbzdvet.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3yimfsixo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3pflenokx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dcwyxzwd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3jejljlfg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3tmuvqiuv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3floparws.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3keimnthv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3rxbiyfpv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3phcqpfir.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lbxtzyll.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bkhmymhu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3rgorvonv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gwiipskm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hoozvjdh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3vvgmvfsw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qzxllkih.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bzuqitif.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3qxtbfwmg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wgairpnp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gcvnzfqx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kjsfwbjl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3qfzealof.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cegzdgdv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fsrepjrv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3fvwtygam.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3qwhgczeh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wxrjuhwv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3wzzduuxk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3uzplgddx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3fkgoeoeh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ishhzauu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3cetdmyef.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3taeuujzi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3flnpawjl.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3dhpjtske.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3duqwvllr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3esuaquxo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3sthhmymo.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ddskschq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwkqxxi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3zqxcawcd.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3sqcnjasz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3jewiqvki.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3trsenwmz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3anwsjanj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3tszqwfeu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rudulcfi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3airdzfrx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3etfpdzjf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3catlmjxe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3dmewgeab.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lpznsapf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eydardyq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ptlkgjcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xllowexs.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3hnencixg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3lyhtxezy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3giesersn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tjasjjaf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rusvtcpy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3qdiemvxw.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3emucedpl.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ttjyvatg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3pivrprfq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ixmqsdnb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xhrljquw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3puzagqeu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3jbqikown.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3fjyeweta.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3rlzqpxbp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3yzyxhkmy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3exjjbkst.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3qiwrbalm.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3aynmknju.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ohmnmywl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3burgkluh.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bnemumcs.html


<!-- 参考信息 -->