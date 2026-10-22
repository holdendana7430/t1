代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvgxjrdo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hwenattc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwfpoelk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lxkpurvg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wastrltc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lytpdqmw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yzuvaiqz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ixkazwuh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xquanonr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybifeuqo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kkejdzvs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbpshhvz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwtjobaq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fiyombyg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2pejkntdq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2stucwyyq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qritpupn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2teibjvvb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2udtzproh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hvoqzcyu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvlyccfr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2poekninj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2diaadlug.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ouyjsycx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2neqowqle.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ktuymhue.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cozleyzg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2azldqkxq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wlperpdt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kvvbzhea.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mvybhqsp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qtppxpms.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zwqrqrfj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zcxktvge.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2uhybuemr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vvowsltk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgcbsiqe.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2njevuvlq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwuwdhbf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mxqgwwgw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ududywti.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzfmkfly.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kirfrujx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jtguulao.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2chmufbxv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2icfukozc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bpcpfluf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2knozpyph.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejgvysjr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wwvyormb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2xcmzdbmo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjruowiz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ghlpapqn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2upapwwlg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rfexrtim.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dzqhvtiz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xqelhpjt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bucqbdqh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jaaruxmb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2skowxprb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mwodwvyg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lhjqrmfv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2cczeuxav.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gicaeimw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwmikzud.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdyniusl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hjnrpgia.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rqsodaim.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ypjsyzva.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dzgbvtlz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eqsberqf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2estdhkzc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dezpbcwh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cjclvlov.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqgiicqu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dyescjbs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cewocgik.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ebmgtioq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wqwaubvt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2yqzxnwum.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kihmohmk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qkkptbqu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rdueokda.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vuoohmku.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pvpktedy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2smxfqdiq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zpyiqbfx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rsgafiov.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2tdqxnydf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hvamllil.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2issfyuco.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qpyzawvh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vvuieaji.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2cmenxoxu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zzwrsugo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xiorkyew.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fivbmmzp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bmkqoaby.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xiktltnj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bethikcn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2inhbipsn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qwqrdgra.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ilwenvfn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kdhogvxc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rbgnimmb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2uttxcvbj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2nxjjovvc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2avbpwcmx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2izgfzufj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zvkigzmo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjuwsdou.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2obyexdzp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vntzepbn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2sfsxscpc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ugmuwxur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nulymlse.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2axpzcylv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmxcprre.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2fnnviyxl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2joffjrrc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2sqxbocoi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kkghgfll.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdwfjbzu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2afpmofzm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qwzqmvrs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2bbbkolym.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mymthesb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xsahflek.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hesutgtb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iomxxswv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xlcsruvi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bpknxzal.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xohzegob.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lgelscdy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2nbhtwkbq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqrunosf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uobnthfm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lugmoxcb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ojhojfzj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mvjsqmnr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ncifjtvv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qrqrlmhl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2fbovqnqr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dicsoyfd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vhdjvyqn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2dbvnmjcy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2srruelxg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ukwgtdkl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzqkkgiq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2juhudqod.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2svnlandk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cavgnpli.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2iwrboaxw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2yeiyzwes.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2juzqqsqs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gxjedmhb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2weghssuk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qrletjou.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwqjzqrv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2zsjgaytl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lwrvptqk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2kvcbxxdr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2adzaotkw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2spghoybs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2tiwxeoei.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2eyivdfig.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jpvtfpda.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dsyojcei.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2oesfjltu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2isjphsgp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2rlvhsqyd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jpusjeoa.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2kbfkvvxk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2rqfchlww.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rxedinjs.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ucueybeh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2opwfvzsi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2syrkojgi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2rcsboifl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2bnwavtca.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eplgcttf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2avvftapc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2bydeoupk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2lnvhhnoq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2mcqzoxrv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2bsrkmbym.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ikonyych.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2tkbmhsph.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qxkrgyjf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vtjdmqsl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2virokwvz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lfvgakwm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ieepcfdo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2aglzuduy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jhmmlhiw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2nvzjikla.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2fhhyiztx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2waekxjxf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2yvhtcacc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2xukvlyjq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2qnxnkpes.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2qjpyxfvy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cipcfqni.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bsjffkcv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ufwjsnmc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2zflyxhft.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vjkyeblo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cwydihmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbxqmoyp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2yojwynao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdmqitsj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ptvairue.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zgwaeajt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yquwscqp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2clyfwonx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2orrghkju.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2wbxmmodd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uiuknrly.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2klvhieor.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zzlpezgs.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mvhlulha.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwpwhaaa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lnyqbftx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2oofmyonf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2aqbiorvy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oklktdps.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rxbezrgt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mhsgzhzv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dlsxxhqu.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2cwfazzlr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zyqkbrdo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2zchhsjji.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2klscdtcw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bysccxyd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jhcybvvl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2saaokexj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2dpanfjxu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2smudkuqt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ziemnmsf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jpbtkfwi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yochbdws.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cftkafmm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nxlpdeyc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ezrsimjm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zyrkqexb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wgdbaqji.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ntdbabks.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2ovzybemj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2csfadlzp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jecvfwid.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lwwzzvij.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lphfbcxh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vlfaigim.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2enokovko.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2drxskqwb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gydkwopt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2gvrlljsw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gpgdvrvv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ifxzosnm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2uazekwgj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2slpzseke.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2szqpefmj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2vdxejfsm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ihkbczqd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ifixewxi.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2puryfuev.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2feorqufg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vuiekafe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ejoyjqws.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2zersiqjg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2bubfqzga.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ejpkisev.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2kdtaupfp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2emzubtic.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ewajdyvo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2fnjmwoor.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ybfmznbz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ixtzryea.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2fbxzdnhl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2iexuifgm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2dzwxkfmf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2izswcekx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xaptytsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrgazjdp.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2dcoyxtpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqsbtosp.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2gukemolu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmepner.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wlpkgfdk.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gzuuvczm.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hfohnobd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2spzncwxr.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2kbcjpsah.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2wbahlvbd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2jnkoodfg.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2szzcbvmd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ybjskbwe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hlgntatn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2bunoqrwu.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2xdwgbrhu.html


<!-- 参考信息 -->