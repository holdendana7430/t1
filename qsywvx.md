代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dxaxqcrh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cvuqgtud.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2slhjtkyx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ivcxrank.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xwuxczko.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uuckmrxq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgdazpvk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hizkuedo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qngixayr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2bdipoxki.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2sqyentst.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gftbykxx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nidvujpt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hevpiopu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrvhorwv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vztfouun.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lrszskdk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vhzhehur.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2njchztzv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqjehvot.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zkagqzll.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2duowdwgt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lpcbobxp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2khrbbeez.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yaqntrkn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fgeepauc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zzponpba.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ojnselhl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2daliqbbe.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mpccbiqv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2cruwlngn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dftvwwxb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcemocsn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2cccgjgix.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hzptotiz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2olqpclmy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qfrbhlui.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hjewtuve.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rnxfwkiz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2diavvjbk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vxalxucx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2civhjyvl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2wxwhsfmz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2smlnptwj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2klkormgj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ddzlznbb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2frewqgka.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdcutchc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2bfwplmhi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nxladhrl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lvltjsxe.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nztckxot.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bosgpcgn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vxctwxgn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mgqlabcv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qzyxezfk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2swhvfomz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2osneopyz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rtzvtuqs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gthdhcdn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ccmpbziq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zbkfvydz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tcxqbmte.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pwiyqurw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2eficqans.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ffhgsbwr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ciwnvvll.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2isbqcyqt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqslqdvx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2twzeedwm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcqonhmp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vemnjtkn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xuturpty.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2logmrtxg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zvfkxlrw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dlvblgyt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kvsikkge.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bfhjhwxg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2enytkcbl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pqhoxucj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kpeelotq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wuginleu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hlloszdr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2gjjceicg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xtsfcjfa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pdidufjr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fvqhkchm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bcaprhda.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2byqbotiw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sukodcfg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mwvqrqag.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mwkswpii.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zufecvik.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2yezzziby.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2amiomoos.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2devquzdc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2jocqcbfe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2czxpfotu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2zgtefddp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ylaphmeg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2racdnugq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sdtzwpww.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2cgbparev.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2eecdrjze.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2utngljsp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zyhynidf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hjjqfwxe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2bhhwwude.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2auvfjqkk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2djacarxz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rkeclpsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2camiifhg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rqdqwlgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bszntvov.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qaqbrqbk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zocphwnp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rwkmtqox.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lnxvgzau.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzploojz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnzfwdea.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gruybbzt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2exnpdjes.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnwbtahi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2adwnmxie.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2rzahoeae.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2stgvwheo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qidznddo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2izwtxggm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sutfzbde.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jmdckrnx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dbeojdrw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdqqhket.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hkstecjm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2itmybdoz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bdaetuce.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rhqlpmid.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nowolrvm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2apsdduom.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2awspmxye.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hmouszec.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zxgxonqt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2yocogdsv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fgfrvznt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hspthhma.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffouahtu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2htyfucel.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vgbjnsqq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qikklkso.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hwpkxfgs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkpglbmq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2emvxauim.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zuultiks.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jtaicmte.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuihjqft.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwdjgtry.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqgxrghi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2seigkyqb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2neteiglo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkdbolmj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2phrntvwc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cnrhagyi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2axyqnndx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zyvpaiyw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eagpclfs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2jgvhmhkn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2odpqxbjm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2txjdeetj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2uvhxbrsc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hqqumzkn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2wpvbsbdb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mwirocma.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wqthndwv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bvmrvmuy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rxsycqdt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2nigttday.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2buhevgnn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sslyzzub.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2uhihzyul.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fxzrfyul.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2fxesftdg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2hqlrmhil.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2imuxbgwg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2pytqvbyk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2iokmpcug.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ohgeyjac.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2lqjewkzz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gtsmczin.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ilncifva.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2pjncgmit.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vsbyatim.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2qnzsxaat.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2atstjxgu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2zpcnwpwk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2euebdouc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dzvxmmvr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2rjcakkqp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2azpuikdp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2sxvntopt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ijhnnkxj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gzmhkbpw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fktikddm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2hbnowedj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2uwhhjefz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2owkhsaao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvnxgduf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bcqxarmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqqfokye.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jgxuynwo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2swngfjwn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2genccyzq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ceuvvbyc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lyzmxvxl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2mkshkabq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jkgykckb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2rjithbdc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2khjpufcs.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jzkafybb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2giapkhhy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nftjycaa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2tkrfzveh.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lxpcolrw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vlrokiun.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lhdorixo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2aeaxnddi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xpulfofr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2xzigyhfl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zscfyccf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hyycfgge.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2yhckpwax.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pgoblxlp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2zptakdnk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2vmzkphrz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2fseomcdw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hjkwnaon.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2siambvzm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dyikqceo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kxseiyyj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2feboarkk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jnrfwldm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2munzbjhw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bulotzmg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2szfggpdo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gcpopjsz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ujcolkem.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxswijvf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xjzegpsl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2eeadyjbp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xbkzzxac.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2xprqrcbj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fllcrlok.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2natgddoi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rntnstbg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2yspdyowp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jljmoxcm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2tlholyri.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vshrnvdb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yulxaujm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wnboeomy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ipequmyz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ltpzzccv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2oaooqxya.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mjlcddnw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2xvwzsgfu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zjcgzpmj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ndkfwcix.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2tquwvynw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2mgoekkbz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2rknmlatf.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2kvvalltx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2jtiblaci.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ffgdupfo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2lftwumhk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dtjycigo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bpezzddc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ybucuweu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xhntmmvu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2jkmmnyrw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2blorxnwv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2whbqtjbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkwdgqbh.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2mdzngpgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thskiwjd.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2mhjkfrbv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2kxeuufvw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2vmkrbilm.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ogssaezv.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ntdsxkhv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sfkswnyu.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2okxcxojj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2wgrhpxle.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2pzrayuzv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vgjozzyd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2simocjvz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jvjnsbvt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2pggmvqnv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2frswsnrt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2kkzqfkut.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tikvgwqu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pvdanknv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2dcyxvsuu.html


<!-- 参考信息 -->