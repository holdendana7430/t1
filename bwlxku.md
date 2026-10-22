代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ixuybdrl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wnvsoeza.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vgogdmoi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2udsuddkv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2egliqbca.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wuokfecg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2watvnqix.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpfjjuac.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2stjklvzh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2phgjwidu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pddmiclk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uoucwhij.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lulcyzdh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2siabqsmi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xumleuwo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2aiawvkdd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2snnoabkq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2aheejezi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2eneupthw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ojvohalv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xlysrjql.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mebhwyuv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jiaxjxhl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pswcxzdo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2nocnlqpa.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wujyvvjj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2whrqoivl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qkblopyn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrqrzcag.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2icccbgzz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2iaxcdyzf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvalepyy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yaeaivry.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dixluttj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kspumnkk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bqsdnkdx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ndnuxtej.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rntsllkc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2tzyrqhja.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2cbbdtvrf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wjbrpitx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2yycfguyb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ynzsxikw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2upjctaky.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hjadeudr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fwrounlu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zqrbsgyw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gsahgjss.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2annxelje.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2faguntfo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pqsgbakt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eyehctax.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vkiagsif.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cjlplqvn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xzxmzxua.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2llvhtejc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2odfnfmti.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqxmvxit.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nqvicyus.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ocjcgmcw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2eebvuyzm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cdjkjnfv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2avchfuct.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vcutpfho.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzglmzwn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2stfuryfa.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dlpwumqq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lkvbfufo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kjwujegv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2blvbikhc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gcataxck.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhkeatau.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2znwlcutb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2apszwgdo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wbixnnam.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gyhefjfc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qxldbmgq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wmzbarwk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rtplbyor.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2znbesfge.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pqzhmgah.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2nqjfsscj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2guqwgunn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qmphrzrl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ynjzjlbz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2sgdzgaft.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kwwzrtcs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ovgtpptj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gfifrezr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2smzypgcb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzibeyab.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ggiyqxdu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rjkagxbj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sxlgiogo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rflvzorm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nwtgyleg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2solacidr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rahtxdpg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2flqamind.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gdfwkmwh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2dorztwpw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjfpnlq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kfwflpbf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lwjoqswh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jtxvhgdm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2vpekpmcv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rkuzeqkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kypfriqe.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pdvzfrom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xelmszla.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qcirifsz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2glhmbwlc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lexdizhd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nrxkvvuh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yajdlybe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2bgpwgddo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2hgehceem.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2rvwfekat.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2rbosumbj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2kfceluft.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2qxqxaglh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yufmereo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ucbwnhsw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdzzlnsn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uobalwoe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2dtmikcts.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2rhdknprm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qswdajif.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ogdpxdsk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qcrxawjp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sfcuycmo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zlzshiru.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2immqokcq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lfdbbvlz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2pswdtiox.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ftjyifuw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gowjtngh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hjdkokio.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kvmbspuv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jxbdthgw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hwexwxst.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ooyehhlp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fykjprev.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xotmrsob.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zoatnhat.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2cucsuhot.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2hbuxmkwl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2eduazjhq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2uqqolqnc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfgpurns.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ykpahitu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rlcsensm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2uiggmzdf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2czdtxdts.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2soioznof.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2fdbinkcr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qurvacik.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pscmplrz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xcnpyyoy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uwexcaup.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bmyabism.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pimtpsaw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2szygcbmc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lnztxzsm.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2wzqrrlyf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fboupbeg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cmxgpkni.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rzrsbylq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lasybfey.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jxhchtel.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ogtorufp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kviixwjv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qcljqtil.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ekceogto.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2paksysnl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yeqaviku.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2vsvuoybo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2cugyyncw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hoxthdpc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2hnpjiebf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2iiiswkss.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2tisvzyvm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2erhlfxnr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ozfupcxm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qbpmcslx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2pzjtskio.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2clredura.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdmsqzyo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pyzbaxwi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ahsoymry.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2waxkuzwu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dreipefr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2qifjeaow.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2uaewaule.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2smnsmazw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jvfmjntr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2kxmpxqrd.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2znmbwsxy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2fhqgxjpm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gayijnpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwhamqap.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ghxeulje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsbucikl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jnzqcdgl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2magciqyj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wfejmsjq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pgyrlyap.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wwfimcmj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2kipzeqys.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2dzvemvse.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pngxnzxy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ybfwxxxw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eebuwtqm.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tawuhpkg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2qwwinqnm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2xgewrugm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jirlrrup.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ysuozyom.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lpmpeccv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lvlqfxxw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2koywhngy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2vibnfotb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ccypmfll.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bsjvqaus.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qqwobnom.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2cipafjlz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ncvrkgff.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zmbdolex.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ynuibjxq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2hburgiic.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bdimuerq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbmzptey.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tqglivha.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ookxguwy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mqpaprzq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ebqkjxij.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lemihxdb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2joktzdrx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yiouhybr.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eyrcpeew.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2pvuvnrmf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2haovkakm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2sctgbyxj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2apjlxlrj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rdeyichh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fwmdparo.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2clbkcmil.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2eymqyeww.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ccjycvoh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2dqupofum.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2bysuhdfg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2evfgcabm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ztadmfpe.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wfvuycqy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2qxlyisop.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2njpzvkdf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mjfjyqot.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2qxybcsqs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2mftktbpl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jsukxsnk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2cbgbflon.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2zvyklcpf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2pikwaitl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2hihnujcj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2kxviemiv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ioviqequ.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2lrlhrykf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2lkyvyggn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2nqsgpcfq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2negvonti.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rrmgwkpe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ivwqkhcv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2hxkxlmih.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2yxztvrwu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2yynekaqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhurogpi.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2vrgjkwau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvblohej.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2xoyrekou.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2vyrntadl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2uvdysqid.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jovlnkqt.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nsqtxosh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xdlgwady.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2xicipksu.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2lsaxjimd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2uraooaum.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dcfmpmkx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2glmabmcs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jhyoyzrk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2lrsdliyk.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2adljnmtj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2lifxmljf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2nwaaelyt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mmseents.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2vzzovhfv.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2naxgsdae.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ziaskpne.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2wdndfgne.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xamlyvgo.html


<!-- 参考信息 -->