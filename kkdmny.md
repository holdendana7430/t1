代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hmdqrvwa.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2oucvzbrp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nkwaqciz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ieqlpsus.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uumiyixk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2avzrinfv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2weieocyc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gxtuxdch.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sspuwezl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qfqhgrmm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ugkooptf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lmvktuqt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bzutzmaq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ahaoyuoe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2deigigqm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jeknplqs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hluahbwk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjfoctdk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tyqefpfy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jluqkldp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bkylnfqe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zdhrgfsj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vglifhig.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hrxxhpng.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yqvbksbr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hrqwpcms.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mxafezfg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zasjtklp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jgegkwxr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2snczwobj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mgjlpmoa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lrsmulgg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmrnnpzx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2eyntkcrg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgkbguln.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2dyuywgan.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wnopuqju.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gcrmccbc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2syirlyyt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2miaahmpo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wfymeill.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2chuwvkgg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lkpkymyb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgkfggck.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhxrfmia.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wdzrbkwc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mcwgpknv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmrvuyxu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vyaiobmr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2fllwfkft.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mmhsyzvc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2caginbfs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jkavkect.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2euqnpyog.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2whtwrgkz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zzodzcis.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rzopccpj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ghskeynq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2vyoypoyb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dibsczuw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2deeyapvs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcvzaihd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zchewjxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gxfsvsmy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xnivepbb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2znfxjkdp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ukdehtcv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aaixsehe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2slwgtefs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umwocgvb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaspsdty.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nmkflrwk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nrabvpoz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bgonkzzo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eefvfggh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2llrbpmap.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2npohfsyj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2geyacmeh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2adlamhgm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ienmbweh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mjycpzhc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yrhaexld.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2yobgowis.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uzbcqfyd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ndwoffkq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2brttfbhr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fcxwshbb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kkwfilst.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2epzbncde.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2psrclftb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2pwemepke.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bzgchqln.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nsbheuqd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fajswebf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fgdkkbtn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jyiezojw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lphejmrk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fvtlpwui.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2uvmqffqo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kvcnepjk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yckteijr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2drjzmczv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gycpdqhx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2rreggaqx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jdnytkbg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hzzwhtxp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wknihtqu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zycdyaxi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2smqsaxnr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2avwucsqr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cxofffoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnxaabiy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bygrpjgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpwvitzl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2eftnstpo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mblfhbzn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2spqjbyhi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2upaoyces.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdvxcwws.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uapkatzr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jwrtmhew.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2wzsfxhbw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2tsstavuv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2idojhzik.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2msvoybtx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2msgrbota.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgymtjcb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mhfkfwwc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qcjgrlwv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ycjiscpa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrywqzmr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2txelfuzd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xtnlhtwz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2yabraune.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fiafkivo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ymckettc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pcewvoki.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qolzgbsm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2huvxgkpq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dsgjllae.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lgrbhwyd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qegmhbqz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2mnyvvqav.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcfproqy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwatogbl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ggvwcilp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqscwpbk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2aopxxssn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mfbumshm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mprxlzzv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cgssjahz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zcubojrg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2yxtkfaby.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdescbqi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tihywnby.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rliyklnn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2tzslverg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nevdjmlb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2iamgmocr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2yufqyyer.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2nnphmqxl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rnvyuxlr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2detnjvdg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rxajhvhh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2fkjpjcpg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lvzsnqen.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ddzremxw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xertzmei.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2cegrgipx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uyljcuto.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2juprkyxc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fpyvtnpk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2myqdsfjo.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2lldlbavl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2sfawrvkf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zxvgxvwz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bcczqlyn.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nzffantb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2xvknfjau.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2uromoaid.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jzktrdqd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2auaqsuzf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hwrqzvhu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vpsikumv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2cdybypol.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ktmdpmko.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ahwuewkx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2wlibrlyr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dfhsfpuk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2fzlozzjc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2vvjhzcgs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfkcqffp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2nkypvntk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2elgtlrva.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2osgsppek.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2sbgcnhyu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nyvahmqw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2grxngawk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kxnvtlkr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ifyluiar.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ggodgqug.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2mpnvmaqe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2mrdbzrpr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ybxqhcjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucwylwmf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2jvxznvtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzydxcxi.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gahjyyqb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kkabzyqv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bdraftkv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qcnloicx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bnfrazof.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ilaxztqm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akimlmsf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2niauydga.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nvyjrkcx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hbvmwwnq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2maeecadp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2heajzmxl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ledqbdez.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dhkyuwar.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2crqfpccv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rjflyvwi.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2yqbuecbo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2liqcbpgb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2wohszmuk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2nqlheyzq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2khaanucv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mfkpzsqs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2cqgwggdn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2mputijgn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2pdsdnbbd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2nxjgjwdk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2evvkazrm.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ozwtyljq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2qunvxknj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zejnplwu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xnwhffhv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mrvajbej.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wqkrbgnl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2qprfoyzx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2agbfswgf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vrejfwce.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ibmxmdai.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2zkfqsove.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lgtwzdab.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2acpohfji.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zdacsobo.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2txlpyqrt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ociwntbe.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gkerwzyi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2lzvfjdyu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2zrdvhwbo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2trtddgts.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2jgpmzyno.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jaojccru.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2eqzcdlar.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ljnpodxh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2oelbnzmf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2vgjzaeqc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kdjpmjzy.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ytcngkpj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vuazipbz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2oyslukgw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2qsrxrmtf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2uctehjjg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ytipczkr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2pycexfxb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2kobhvdzs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2urwxsgid.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bxtthhbe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2txderomt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2orjomvpr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2chcyvsfc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2brnfwtht.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wbjhlflg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2dvzwnmng.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2vntppxxw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qnkvlzai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxelboqo.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2hknwtezd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcvfyvpk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2vhjyfdsl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ojuywauz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zgkqamoz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jegjwsjm.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pwtvdakc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ruziuuwq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ubiibnxz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2hgymnpha.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2wponcqmt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bwvvouvb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zwqrtdjo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2smhrqxrl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2rovbbspc.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2hsvkfohu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2osofzthg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2wmzcbbdn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lxkhlipr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ycgtwizn.html


<!-- 参考信息 -->