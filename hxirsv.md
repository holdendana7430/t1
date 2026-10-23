代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oanunnec.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bxkuvsqf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3asggusql.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wnadqhox.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eoylwpsm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nyvidctk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ggvnhvtg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wytaleca.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hysdahyn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aulwuxob.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmigejeu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hojlqavl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3swjysbfr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3unqltzkk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmrqpwiy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwbquzda.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mayhtell.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3woxdstao.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3itjxlzvm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzflqvdn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lpwpyslk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3johjjfev.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3metdqmaq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3seggbtrr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jspkzsxm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jnlwcdze.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zjsojyjd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hclxievw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qqgczhnl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pojovwio.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pnmzuovj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yrfecgxg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dncczwxp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gbyzsrwh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xdtmrsqd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qdygzinh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3eziomaif.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfaxopwj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xhojevkq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fpsnrnbv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3othwymtk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cknnrtqi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjsroave.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3juvlasvi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tnmfbfxj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3uaqgbvij.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3oedbsjme.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ykscrknc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncznjyle.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3imjkqgav.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hcozkgev.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ownavrig.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ylosifsb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zmpcfapn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bgfhssai.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wmakojit.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3urankrmr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zseraqdo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3whqejcws.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kmnutuoo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gjsriepi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3uhlyowkf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3blxjvaax.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3osdrrmdr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cjsmdeot.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3damjthir.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itvgmtlt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xkzxllej.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wnyzydht.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3scipzwvc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3oiqxhbbs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ujubftlj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuvwtczm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pxctxfpi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obejrast.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cowhguvl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mwnovqee.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gcgxyijp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jftaachv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3nxofipdr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3pieoyfak.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3svonpurc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3flayhtzg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3htiojixd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aogkkgpk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jzhnzstm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dkneaijh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3afurrkme.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ikayglte.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rjrauety.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vlswqqgl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3goumojln.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qmwrkhya.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxjjgzcn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3lrxvvuez.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xlvnaflf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3cxynbiuj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fzbytdmk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lfxtjveu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jmnmacox.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ydxiibil.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nqbdykwd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fzdprvyf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3rdvkqotf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xlzacams.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kugjdzzf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wqcjxnbp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3pdhbhpvo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kbafuayu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dydtjvjf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3frzgwptk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yfoqxntu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ahktfllp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gulrumxp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fiyrznlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmnktvuy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tficimma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxkaeszv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zlvrqoja.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3sbdsbvzu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ympuqvhu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sqwlwcks.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhduzwyx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kehzhjdu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vkyjhikp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3irzoxesb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipkjarkf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3unqugwrk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wizyslya.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yhipgekq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3atydbubc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojkbhryh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtydkcvb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3btotjmwa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3nyngyyhn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bdsoitgt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wwhufxve.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3bbiejbwc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3naokarsf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tjjuaokk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3obsobwxl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jsokatex.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ttrplyni.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3alrhiojv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hxpyyrnq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwyrmqhc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3eiwhvrjc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rbohyncu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uizwunxa.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3enabulwu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lwfqmurv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3xiyjwuvx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3grfrtiyt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3oilaerpi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3prjbsskf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ebkbarws.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ybpayuyv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ymzexkyw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zirttyyf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3vlnxdoll.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3rlbhrnuh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3rdxsvdut.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ksdjdibd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3sdjmdtuy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3bgydjnew.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lgipthvu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uikmfcjn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3myagrygo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3cypofdlv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zsqhylvp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3kbchvflw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3tdfxovhi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3zcqskpxg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ppteciys.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ckndeilp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iialxikd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3npdvwoei.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3lgirnjag.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3eeuixoia.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fvdjraoc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vhvpdtss.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3nacwpmnr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3kcdaqzxg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3gdrkqplr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3hahvyzgb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3yidmgyta.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dokystpc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3iauylkqy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3orajelzg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3djpgmcvo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3spinbhen.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3vbvslmdd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3oydyflsy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uvapmdlh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3kxzuolgw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrfehdfs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3afuvufvf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3rdsvnrjh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3aopkgdps.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3eyugcvah.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fwliiwru.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3klsdqcwn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tcdlxfsi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nxpovkfd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3zyfiaxjf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jxwnpdfn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3gtqhhwtd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xcslpqfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovwecflm.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3otpuwypt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rslrywjk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ilvqwzny.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3olkgvncn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tckozseq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3msvtktfo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pdnyxaoj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3enukqotw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3csintspn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wetcywdb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3trifwvce.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3irqdigpx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkxzgymz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lfdxoqwa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3pkttlqmp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3bsukviyc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hstrynxt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vuflfrhd.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mpidccmk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yfmwglit.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3eeghkmex.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3xfjnptlr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3fgwctxap.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hunjtrxk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sqcqtinc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gbxgciti.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3wxjmpehi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ylxuimku.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3zaukjclj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cxrxnfvj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3omkxfgny.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3miupynig.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ewwghdai.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mpzzuxdx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kdalbkax.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3esdcabid.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dgyjtmsy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3nxzwhmik.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3yakzfvoh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hytlrlim.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ugstkfuk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3oenhxcfp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nxjsbfli.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wftztbvi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cumrqynh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xlrziszi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3gjtrljcs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3joavwzmi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hdknpvzf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3vfaaydav.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3fqlordfk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tuqatszy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hgytiebc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3piufhocn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3sqwixkqa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3uscbtohk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3bhmgxcmu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ftntawar.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dnwurneb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3rtzlcxqp.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3qqjfzgvl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3xljtweta.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3blzakoet.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3bkhpybbh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3tkspgdgb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vjeptike.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3sjsrjnaj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ugcfunnd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3uoyddqxr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3epcxzhjs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3vwwsyjzt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3nebuqbkq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3vkjwocnx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3usnyxmsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypjnloul.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3cdhwpsqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcrqblnv.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3qbaxbitw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ofkcfpfr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jozrrpsm.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zlqpmafb.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gjevpvut.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3iykscuwp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3mgsbjuwr.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3itbfxjkh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3qfpzoumu.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3shmzmemm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qmzfjwbu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xzfcsoqt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ugcjfwsg.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3hedkiiqe.html


<!-- 参考信息 -->