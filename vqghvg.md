代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2enabwddl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zauxmwaa.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uzzhvuev.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2nbboqvjv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rafzhuqg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmvhwtrg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2durqawxt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pyshzahj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufktewfy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ffkhgmol.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kduarjmj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2anaisqan.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kulqzjtj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2fitavcnc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2szejfysz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rebjxcsy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2snlfzrut.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jqpackvw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2iihjwlop.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rhhnzkyj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2acxiqzyy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2kddswsff.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mnzxcdxl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xqxkqajo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2arzbgygq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bftzhdgc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hykwpxyy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rpmayxdx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2knoeaibz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2igyztrbh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hyqdwatg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2aerxoaon.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2feujqekq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zagowivl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kggiigac.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ichpytbg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2aoefkfpa.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2luvorvqn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kujwmkmm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tpyihcif.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2tdyutcvq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2qbllxbfo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ppcggtpv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2peogtfho.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2afnboajc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bkxcjvuj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2htqpfmlt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zelmihpi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2cfiktoiz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2irbnemxd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2icbiylgs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dfdbglxz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cryklros.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yiixurnq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sjxehiqh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2whchtqqx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2utvzteeb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2udzowiee.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nzkbtagc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vojxtqac.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jmpvpuss.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2audnkbyq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpnipzmy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cquhsaam.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rnglzvyh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnlrslma.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2koonhkmu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gbrtnwfh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2msitklhi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bafdohlg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iovalmau.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qnuuhqug.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lbuexajw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ykqorcoa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2voxyjvxr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rqbxhnyr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yghibupa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rwbsdrgx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ijaptcdj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mwjxipmi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zrxidmwq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2czzoqhvo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zaxuuugr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2qkayxisb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2bmlxfsqh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2irpaydep.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2osulgruh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qarpbdap.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2agjdrgbu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2dlqrlmhm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mmqtyeni.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nioqfjny.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kqgsxwtz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jevracmw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ignssutl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmchiatb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pmzhhoep.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lsdixavt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ttvfczbz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2afpjbswp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lhygrufe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gtygatxg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vvtroawa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2uzpmcfpf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2aawekkim.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aupwdrxi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cqgzxiqw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tapyuvqg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bmidbzrs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2oqurzvax.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2srpzdgia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcgewnru.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2knlzjhdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2diiemndr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2hutgarkg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hvwmtzxu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdiudegv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qxqoihby.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wyinjdij.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsskkuvx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xhjqejui.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2giuytdoh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xiqdllxy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ehtpfkhd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2cquvecbs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xgduypku.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohqsunta.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cezlplwa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yuhvqive.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mlahunoe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2akjnfcrq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpiphubo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kkfmijof.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2iquskfnt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nhojbprb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iouuprrx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vouryhig.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nwwwifvs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2aecopzlj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pxnqqjll.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rgzfilsz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2cadswnkr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ueevbfcw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bvrwczla.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqjckaqw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bajxbcvi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2milhsupf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cyhnecis.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxbymaur.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2sskserbb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2akdqwqou.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qbzlmrzo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cyzamxym.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjdaxnrg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qijincxj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wutvawpq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vxhmtsxb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2bcaikied.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvbvhlpx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uadmpqrg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2uvvmmqom.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2skoprajf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2euvvajta.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sbvcxouy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ulzvkrgx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2yezijcik.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ulwtwrmj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2znewjkti.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2enhtmkys.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2jfiqftja.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zerrbsxd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gihuodir.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mqizztqv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fbsrkrnd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2nlcfyvrp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2upxvyboj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2byovvcyk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2madpqigb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2yjgtsnys.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2djpatyar.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jrgoenbg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkjqefh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2rovclgsz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2zbptmiqh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2auvhislp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2gbblpqdd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2aadabczv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jzmkegar.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tqgyioga.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2vcvwxbjt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2bitfeocy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2yioiqbfr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fbgitdwb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2axtbzcxh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rrktajjb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2kdcuhdfh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2icoubxly.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2oxqhxpqp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zxcnlgkc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lhlczzfj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ehsxyxae.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ntqcyvfc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qofdbpgu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pyuyveie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpfmkwxw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hgtmttin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygejosxz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vxpbehwp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vowdpzdp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kzkzgelq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vkcyekmg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ocnxyyab.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2dkbpubux.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2fstdfsur.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uspeuvew.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wxumzwkz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vyhrndun.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrywioyb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2dnkxambv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2lbcrsiwl.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2pdinkmfu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2iuqufnth.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gffjgojf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qaioeujl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qwxwnxpc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qmlsytqe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbndkoao.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2jywasklg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mreuanoh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2psrnjeil.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ncbybfvz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2flmdvjvk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zmvbtjlr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2apgpouzj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2nqvjlqpq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2zqqkebkk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2paiedqpm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kiadfxbg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lnflrqjb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2prfprcel.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ejnohlox.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2angwbygj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hgeqttwh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nutdooak.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2peqeqcfg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jphkpmxc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kpiiptko.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vrhslpkp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2itubsfyu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zqjyczgb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2iktklzpw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rfzscbks.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2wwteubhz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ltvztxbe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2rkqracmj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mkvndrze.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2rlurvqrp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2upidotaf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2egqglzru.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2chxeafhm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kwhkyxwh.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2aeiqfcyp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2lzivntqt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xolfbwhi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2cymupiaz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2wuvnrcts.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2fboozzkn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2izllooqg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ksrueicx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2tfvfojoq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2pzyyqdto.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2pxttypgw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wopkzcuj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qtmsizpr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2esejtmer.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2sxnktkkx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2cotvjgqt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2fxdmzidu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2yjyfshlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oltayjda.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ylbldezq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwysmnkg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2lidksvlt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2qpngpvzg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2papnlzey.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gopxeyey.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cjmbdbjn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2bjamcutk.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2uvpgwhyj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2bvwtwzbz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ykrckfgm.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gmfjhisb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2viwwnsjc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ludjbhzz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2pjcecwxt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2pplggdqh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xevovwkw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2qfkcifiw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pqdevnko.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2fjebikyn.html


<!-- 参考信息 -->