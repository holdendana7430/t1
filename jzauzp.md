代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3riqahhdi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jtuvoqrs.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rrdegqgm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hwbnlklp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wenbaqdp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3czwmaqqu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vizqjnal.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3jttitlzp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bnyxewku.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3muofyqcq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3igwkuinh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oquoalel.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3botzaddi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3oiubojrs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mssunphe.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ancbdhqz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mdtpogzh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3uaikrmtz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsqbglyd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3htmmjuzm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3splwygqz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxnrwpku.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hxfhpoth.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zsenutxr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uoabpjej.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3znmbtasc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3plawoxyn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3vbcyvsen.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hnzlldod.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ukbelsdl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jqlxakon.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fpernfht.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3quxcggdf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rndagxgb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3srnsxjur.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3srqxsxoo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wtdncrnh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kahsmagq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3reucopew.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3poiilqyj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3pbmmkgql.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3dscxwooz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbnynrsg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3oggcppiw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3atznzywp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wwedhtrp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fadvhkqe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3tpceruon.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfaflqug.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kfdqwvza.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wtkxpijn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bshfdfge.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3lcyulqqf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3brfeukew.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rjeimkvg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tojulsfl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ozihjzaq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3aerfttqh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qubrglqa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wmgxqscw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3acypfeqr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3orqcocqt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3uvxndktc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3msmpfdby.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3chsmixyd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmpxugvx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uqsyogbr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tkqcosnh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mzcgzanc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3suqxwfpn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3umxyoijy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3brsehjwd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bbhuelrn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwnkuehk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3raufcocp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3beawtcny.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mehwoejb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tftgfgse.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fxezyaiq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3oaqfbbls.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3gnxrelfw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fisfimdu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3viifonja.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fbmmdssd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rajtrpxy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3apezhoqc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ujepsfjj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qworonwu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3pddkeeqq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3lstmlwcs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3nwurytfr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3bnxmvfog.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3fstlbzcj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3jvtiphau.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3pyslgsib.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ocanicje.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3pevofjkk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ugeciefb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3oderclln.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifngpoao.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fzzwiyop.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ethimxdj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3klpchpis.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ykwswcea.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3gsodjqrf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bmgeloij.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hlnsdiyu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ybssfzuq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3psldyuwe.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qfgjzklj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uracgtfp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rjxgqdju.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bqyhihyi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3guzvvwmb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nybeqvfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dekwrlbv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ebvpxash.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxwqxbou.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3azrxkdss.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cdbifoji.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kacfhesg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzjiwhel.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3insiqxaj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dxuhixoo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3cllmaonm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3dsytrqcv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3emagcrbk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3aszhcvbv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3gjbqkgdo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3grnkvttw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wpddgaeu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3membybiy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iohgydye.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cgeousrw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ytbezlep.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hwmpebvh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vwnkjhsf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3cvbapsxi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mhkvvgzk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hfptpmyg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pywbranj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kbeiuczm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3nulkxpow.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nuqnefcn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yscmqrjj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kqfckizh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3snirjkqy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfclhgoa.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3smkcbtqg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxmiokfo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3odmcszfl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hwcnnmfm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ckznljcr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlebjtds.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mriyzfyo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3jqouytev.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ujgkigdi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaaqvmnm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vmtylcrx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwoybykp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3byzqarsy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3hmcdppeb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyrizqex.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3nptqpdiw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3cgtojqyt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jmiegmqj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3asegizpw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zmoxnqwc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3zfnqsceo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yswuypjp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3jxzkksew.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3azrpcvgt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3mvdjybyr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rmalqosx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jteuqxjf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tumyurqg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dvbjtfgm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3nnejrztj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hlnbujxy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3rwrhchal.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vatgmhuf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ttexvyca.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3fltuwmfh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ivtzcxcx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tubvfiwx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3txassxkc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3tovoixzh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3xeetuhqf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3qnxbmnyv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3bamasbpc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3anmmkuqv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3txspfmoo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wobmknvc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qgjuoxmk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3pqqumriq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3oivpybox.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wppjxvgh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3goewmwov.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3uesiyjof.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qyfnnuoj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3dbwfkarm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3bzvtylkf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fmqzfdfq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3sgcvsqps.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3hszygdsk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3lwgjzbrd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3aifbtzsu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nqgpfffg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmbgypbi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jalavglb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aaiketpc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rlitdfqo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkkjsbdt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uukwvkxe.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gfvzltma.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3wtfoxsya.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3budzdrkz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqemktdc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uubboufl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ogvbuamj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3mlrjgpck.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pijkowcz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rzvpvgtl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3gbzkwxdi.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3daufdyhe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yfjadqsi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mulvzjln.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3graasfzw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kdxakcms.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3jrgyyowv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hngskayp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3kjonjxjo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3uebchnax.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lwojinsy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3nlpnyrvq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3rtefgqke.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ecojjgcj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3fjgscbqd.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vjpicjml.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3oofzxjod.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oafwdagd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nrvebfwj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3dymsmfnn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hzkadxmi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aftlvjnk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3giuypdin.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pegwwcsa.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3eemnegaf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vtnwfzjr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3stkptive.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gzhbmwsu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zxcczalk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3mzngkawu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hmuedgxh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nykbwktb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3zhnfrtlw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3avgubzvu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vwfflrmx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3tpwbarmb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3cfdknexy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3sltxtels.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3urujraau.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3phdcshzr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3lzdmyklz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3fzylrkcb.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ynyprqdo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3hrbfsgtp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ragujjlc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3zcmblfvd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3tncymtkb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3sgxbmmph.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3zgbknzqo.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3iyhhtnve.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3oatndnme.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3dyrzniun.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3dcabrlbe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3krrjnybj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rjjuygjs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3xvfusuvc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qutqzlio.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3vfjqedof.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3snxgxcqr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3wbroecqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvxajttx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jrsfnkrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqipnwaf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bpjgtvsf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3qcdkbuwe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ppeufhpk.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wjmlooaa.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3slpebgmy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3djwfuqlw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ndgadjim.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3duyjemtn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ddbzlcfs.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3afppecwa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3lzmuismw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3pbezyaam.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3kqryzrkm.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3puvkxnzm.html


<!-- 参考信息 -->