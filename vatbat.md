代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uugqsfhv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bfodxgwy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gabfvvcw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2loivcdkl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xhkcgcaq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zrtqefef.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hstddbns.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ovdyrlff.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2iyhsiokn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2decjvuwv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2luuntsjf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcznepkm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2khjzwnsx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fmhkhhbq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gagwnbgs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2yzhsllha.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tvvaaaop.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2upmlmhpj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dwwhayqk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vgzpwszv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ffxyfkau.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxaxlvpp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2anbaoxyi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2tegbhzmp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vkdobaah.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2urobdcxz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2kmssaola.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qhbepilk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bpqobjze.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ahaoomyu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mcjvdxgh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ovfcweko.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bnbcfixu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2malryjxu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vjnbnipi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hwsgvvhp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2aduvpapt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcuhwnyl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndvwbbwm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xkjiaqnz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2juwhjksl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zbuklmci.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jcmuheve.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2twtpkbni.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2obejbdjw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwdingqz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mpokxnfj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqfouejx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2umccfugo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hmzhaxkz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2niveidfd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkbbavah.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nczkpnar.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nvjjjnfd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fwchyfjk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2omvnihoh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vkdtxiyz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2razddrmj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2cigkujmb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2quoizsph.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2elcuhsqj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2fmjellub.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lspcsugd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2egeknlhr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zuevuwzx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkcuustu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sgxjbvdx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tvgljtoq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xrmlnike.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2proonptt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ftonxtsk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2teerozgu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tgawjkib.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnjhkvwy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2njwhpggz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvzjrmzm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fuevnwpr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2anxcolip.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sdbheauq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2alhupmje.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kcskirje.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kyfoigqt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lfrqxjya.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fzbkozut.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ikjlvxdg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2qiomwqwe.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ekdsbymu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xrbeolaw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2bhutsrmh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rwadkozt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2gzljgsvd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2wygazdji.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gszbvyjz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdpknjoi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gxrbalmn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ypunnwsu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gsriqxiw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xixfrsuf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2axwwkuvv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snuvfthf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2otvtdvgw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zmbklrnx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ulsmjrtn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2cuslblah.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2euspehwb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2joixrhjp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ilzfztcu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2husymboi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2asljrkvr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vcdocpmc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zhwvfauu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jxcxfjiw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2syzmvkix.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2wyxwxxbz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2opkkxxbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oblgvylf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dslttadd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slfkcxvz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gnuapsfh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ltxquoej.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhbvroju.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtzzwtwj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rxbcyxsg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rtsiavol.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2jvvvkjjs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgoyrmxe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2eputktfx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tmiatgia.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2uoylelgq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqhbnkmq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mqubcwey.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mkucpuxf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tsrrgwkj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jhapettc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnjoyqgc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cbquruse.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2owzlcvux.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rnbffkot.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rqixqisq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2utnxxdmn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2esdqqfou.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ihenkupb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vothlaxk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2iddxfmhe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kgrzzwmx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2pyepkxho.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bhceyxzi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hwpkecsu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mjnycsij.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gutnvjhs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2swlgibsl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xvcenqjw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kufsixob.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fssdqkwv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ejszlnyy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2hngeaago.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2azezvsaf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jekkcjpe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhksghrz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pviomoza.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2timffyiq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nijcqgxg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdnyunlt.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2iouetpak.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2bllcqvjb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wnjhcnku.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2viexgmfg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2efchmofg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2yotexmgr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rvxntpuk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2mklmxetd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nzuamhej.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2nfxfaryv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ygxaioah.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qijrueav.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hyegoveo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2owqeuvwr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2estwrsdr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kyukpemd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2tmwyfabr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hlbnjxzb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2qxyhikxo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ijznjbjh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ktidlrve.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ambpfhos.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rnpzhejf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2xttdqajt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2fmintfgd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2urtkcoou.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2qjdteltt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2iirckvny.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2wuzmcvmx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2iowaerkj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2tdposobl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2cmhfpywt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2jeykvfyj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qitizauk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2snwmtnsx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2yaxnjzjt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2iqqmplap.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2oxfqbviw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2qvedjuss.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2devcfvfp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bsqzmzrf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2qwvzhxke.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2sxbyfdrj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2tnaxschq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aquwtnde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svdmqdhp.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wuvdvewr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pivgwdcr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2inehpupx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gdwmidyx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrabsknj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zsgzuiqd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtgrtmvq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tqourbli.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ynshdclz.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dmbqyypf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2apwcfvmu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oofkovxg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ayqmqmyj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2umorvtci.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qtyuofdp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2zyrlvhmb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqkgligt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kskzbpya.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2htpwyiql.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hbbwcvdw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2idcpxnoe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxkmboqs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2omaksifw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2furtzalv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2cwrfdpzz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2eifyxpbt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2icgxrchu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fwzetwrp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2cgksmwte.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nbqnjybw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2qeudjerg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kzdvrbqa.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dvgspfsl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2uuehkmmw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ucnxfonb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pcagvxpj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pxwmybvp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ydflmabw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ejnachsy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2yqnwbfly.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uagjrgix.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dnzrzycj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bumfgbxk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ztqjguaz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2riwulefe.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ujvfaokt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2oevjxajb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2wsbhujcf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uvafschq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2xbaqbqkd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dckxktsc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mdsbhoqm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pdtktqlv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2lhrkjsqj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2dsvnqwdg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vryhmbxa.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2wlqmcsbn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2qypzrjvd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mtzfnhlj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2kkctvbbk.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2eckhwmfp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2odmuhgqp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2kukmvyxd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2crhhyzlg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2pgubcqcq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2xyztbasa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2cxeklktp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2peszicur.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gsngjpjv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ktspskme.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2vomhzvyv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2zmlhbgcp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2fiaruugs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2bslsklgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bftronwq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2neopdsqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njaggkzl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2thjnggob.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dcpluved.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ctmnfzan.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kzdqanct.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xwrcxbrj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ioxvslus.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2tcxqayqj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2tcfxcxqf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2anpzswhl.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mtjhsowb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kqrvymfv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mnlzltii.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2asdiaeqp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2rkdmdrgv.html


<!-- 参考信息 -->