代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3elfrooxi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3sgdphsdd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3agxhzlrr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eeutmfnj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vqxencmy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jbnrfnln.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jiaddyyb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztecohnr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfsupczt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tebguaqg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3blddfabu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3lsoyensw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3njuzwhrm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3fzqunhhh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3twnsemle.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zumrtkqa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3arilwtui.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hggqvryr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fvpeqexq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pgekmauq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ullinphl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qczocywv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3dzjszkws.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rzkfmapm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gvsnxlcj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3unabgzka.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmaqgdnx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rhlynxod.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fhhlqscy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3pldmpocd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3diprmjks.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3azlwhgad.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vehqzajj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3iecqpgre.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gsufymrf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbovsld.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxdvdhou.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wwxjgstg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3afelynoa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxllcclx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3nkfezgdk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bmcxxsbg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mnppvckh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fsllslaj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xapbxhpw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3oynqsoes.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zuvloqyx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pzufffxa.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mmjvpcnl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mjzwhvfy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kkznobti.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gitxacxe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jcpxeenn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbarkhyi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dfktrvgd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ovtlrbfz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qklkvhnd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ktzvsaci.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3znuywbiy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3idoakfaw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bihivjvp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekqasghx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tsywnfsx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqvjtnho.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3imvhrfun.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3prjwomos.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pacbotcx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3yrvarntx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3afajczug.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qihughky.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fjffovxe.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kodcdowy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ujemvgeh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jwjalwbf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3djcznmzy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mqbbntxu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fgnwbycc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3bldkjfsi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jijrrylh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3cfjiwqfw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3odyfixot.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hirzdkwa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3rhvjatim.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uyjosmep.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bcizrbmm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vevtnuix.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3uvwhcdxh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nomybuev.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3batwhubg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3favreyax.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3uxjrcqir.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3zdwuvpgq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3uexyrjlp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3stytiqtt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hhzsqvxm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qqeswrzc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rcxhnchd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vrdibrhg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ylydjjcd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kbruzozp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3kxggvqwa.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3adhmvkbu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3drgyiusb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tiwkslmq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3otqbpnit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlqwcvds.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3vdxcsiho.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qusgikjv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3skwrcnyr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsayktom.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lddgehkj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3glrpdubw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tfyuzftg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jhntytlb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dntjssbs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dzaznbyk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3efeagavi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hanyrdbn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zwwiapoo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldsqbrwf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovyrgmxa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3yjoigmaq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3kjkwdfcb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdxjuhkb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3aedpenuo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3amlqlbjb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ezgwvuzx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rusdkoxg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zmphqsep.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wmbhdfhb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lxjllemr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ngczaysi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iicbknyw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ppnrekuq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3qcuhkwsl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bdcgfzfq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lyycanyu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cszmhwsi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbumpyte.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pulsdzgw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3skbnxaoc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxazlzfy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vjbmqbfu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zutmtcbu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3uyzmerju.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvbtkcsb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3posjzwrl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncjycpkk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3kwwwcdyx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bfkeloov.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3pygiixuf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3tpbhkmdm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3jryktpbs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yxziyskn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yzyknxdw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gkqajbha.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhnzmzq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3afowiaia.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhpibfxe.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3unylzkov.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3pesmwhds.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3uefrzlpl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mmfyahbp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pdbqtopa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xgcancxi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xoazvefw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3nenuylxh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nzmjvrka.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ojjunvlp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3eshinghh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hbdbtspu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3lfgntbsv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3qviuihnk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dkulhxar.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dbmhsngn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ffnsxwbh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3oseteydf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3pirhnycg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3idrhjmrr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3qerbtwke.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xsjbjzro.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3bizckour.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3zoqxplao.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3acsjtziz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3fdghlptx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3imhrhnjh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3xurabybf.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3pdgffwem.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3lkgsjzgh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rwbaejps.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dsisnhqg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3czwiofby.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3dfpwvyog.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3mgbdxmus.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3bjiysapz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bpcclnby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afitnxrv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aerxqcwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsfntaro.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3vitjqemj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ljnlrotr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rpexjaue.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3btawjewg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jawaqeag.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3nzmqgmxx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3scldmkwc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ttwbsjci.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jwlocmhr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kjihmfdv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3naqxrnhs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cpgldksw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ghfckhdq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3inxnocth.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pyihwpde.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3scpvezgf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3clxsmwlo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dkkpdkxp.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3nyfkevac.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3lfdskycn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vtvelgze.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3htplmgss.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3gltfoyix.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eawjtout.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3txcjdcbg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3akailxcu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3xjrwfrzt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ihoyhirh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3krrnpmnx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fvtjhfvx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vfciihoh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rdudhxyz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3cstsdhqr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3youdggnn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3jjgivclb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3owumiauf.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ozjlioii.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyylhsyd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iilhogsa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3salakpju.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3crmdxauz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3lfaztwzq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3svlucexw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3aoqsdgcv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3farfynjc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ztsgzbqd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3oqdyqvvj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3qgbykqda.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zcguowwn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3lmfgdvbw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gyzjfbgk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3qeloeflg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3fhniovrj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ujezcpvl.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ccddoaij.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3xefpitpi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wuivibgk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3gqsagvjk.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3pcdkbxuz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3wlwnhmjb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3yeagdsth.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3flessicw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3sjwmxjqu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3lhxcgwit.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3cbmpkqsq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3yjdalllm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3obiewakn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dqqqnvlj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3vyjvsotb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3hzucbxad.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3dhqfavud.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3poxoqkqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeijlmcf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3gwhlxgqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lggcaspm.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bgtyvbjl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3uxrynngt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3cuepzlov.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rsuodwmc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3jcepsiol.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3drcvvwxe.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3pddprrnt.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3zlvvocro.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3qthtyanp.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fsljutan.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3nrfgullb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3mfluwelk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3zdeaiskr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3vuqybhtw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3dvucjdtj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3njqlbjcd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rjnkdccb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ihpeilzs.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3zcbcziyc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3fudchybg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3invwlgla.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wuvziryb.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vavfprhs.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zhfregmq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3byrxvsqk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xslskjsb.html


<!-- 参考信息 -->