代发 wailian999

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2drkpzclo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dggzvszh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvyqvrwv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mlbjokju.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dldkflhp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2aonwtbef.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bsjfioui.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajxlgbfb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2oojalpms.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2yckrcgle.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fawfjqph.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2woreuhew.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rqbfvepz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dfvdfknn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2uvleepss.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdgeaiwa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2axomdenm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zaqbfvtx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fvtaxvyb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2thrqlkuv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2redeunei.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fkfdcgja.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iaijwlqh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2sywukuzy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2elknuttn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wrzdaxpx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2gtfzfirj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bplhyxze.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2smkyilgp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uohakoar.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2iuvwosvk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2czflvixm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2eraafnzh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2fwvopnwk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mobnlhzu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pczsytvk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zjbavxjq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hveospve.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2cnapgqjc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmrsqfoo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lprmyudn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2msotvzzk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2lrcxzcta.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2bncyywqt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ubicynrk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tpczwnoc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vgeyidwd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vigzgjnq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rypyaurh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2myqbfjbf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pgbygfvg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lxstclds.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ywbaenpl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xmokziwk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zhbgfuag.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2srfqmqqb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2joyliuuf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fjvmlteg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhipvqmz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pzilfgwx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2osmupsza.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldfwgyum.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fysclnys.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hvfcoecu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2stkivohj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehymfmry.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2doltzvqg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkcdyxtb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iqsmqvnv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lbizamgv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xxtkhmnn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2szsfcpfj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ludtkxyf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gevnyjfc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2myuhajrx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nryuronw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xcurirtd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vzhimyxp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mxkmocgh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vycneazr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2njjkiozi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2fkyjtbbv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ozydgles.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2edkoqxpt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2svmlqvsg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvatexkf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ktibiawx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ysmmlndc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2osvqzbsr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2oeaeamew.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2iaxushyy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snnbvuex.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rapfvnhf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2thxqpodq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bhtpwrbl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ebalvtxe.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2fjtwxyev.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fcsmddsh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2tujizyuo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tlfowrni.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2lgokdjqr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bqpubaxb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hsimaxye.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hdilcied.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2przxtapf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rtptpyhu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vjbpxztb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvlltbnv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xqxbqjrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bupctzqs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2yygnygyd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ieadahrx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iodklesl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vewoujln.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zsebhhgv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvpcknov.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2msifuhta.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2blmrxklp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwwimnvd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tshplgce.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2enyproud.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dyywlakj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kwvskvoh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcccxldh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjfvislb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jvfrozqr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2bupjqdfi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbwolagw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hazsvqvx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2saigbblu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bkbieacw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ztvzvqrt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tgpieyjz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ldytdahl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zqqgifzj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2znqwjhjm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tnqubobh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2jqygzicm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2baibomav.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nrxuzyrx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiqkltef.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqmvtacg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wgbryowq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ymeqiycn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2dwxucjmj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bqesqqfy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bnglmpua.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2todsiozi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2rurftlfl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyylxrxd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvktelfv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2densuxfw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wvdhnwmf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rgwwhezg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvutprwp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ruijnbww.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2rgmhnuni.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gifiibmv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vinndiwj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2exrehghf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2xsdwkgvq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kchuyiip.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjjnffpm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wpqseexg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rfduktao.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2mjmdpqqe.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hbmpgxhk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2btagspdh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tfibjovs.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fvoqkgiy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xtfyzuse.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2opkbuiya.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2esaavfmd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2usnbgwce.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2roxdxvdu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2bagqkfwq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2jtmqgzqz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xhpwutwx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2mpnlpgjl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2aglcwgkb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ccqwswpg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2lhrrplvn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2eukkssxi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2xoryqhgt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zildkplo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zabuqwxu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2owxyzmtl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2repgjnfe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2aiobvfch.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2imhjlbpu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rpkulowo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2nmcobszd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2wmodxydd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2sueoglyh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2powmeccs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wemaufch.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2mvvaujao.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2nmbntpfo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2avopjerx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kbappafk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcewvebt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2phovzfpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynpxdcia.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2fjtwjzrl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhkkibdm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dcvahdzz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ocdggibg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vvauhxfz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2hyswolfj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sreimynx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2akfdsnsi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nenznizu.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2lugtiirp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnkthxvj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gzidqwiw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2qvejsgmu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2drfuwxyf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2mreapspj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2bxacrtvg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ubiogehi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vpvrflco.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2jrgnlues.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2fgizkdyx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2tylddqyl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rqqipivg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2rjyapbfd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2yxozlbqr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2wihprsqt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2brnouido.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2mknqkwmd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2xrtgfifj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2icytnsdh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lmvkmxmr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2peudowmq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tirndldz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2nkuuyeih.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2zsrbtwni.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2glpjzcvg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cqjvyapm.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gqvlgkqd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2woeowszl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qdbxzglv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hktzyafd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2eygvpimf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2xfeqxjht.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ublwrtqc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2nywzrguv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2fcwlsxhl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2wsklmwwg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dqxjoubk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2xzpwbttr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dxgsohqo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2nvkpqbvx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ebqbfjck.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2fbnxmuvm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2igugvdjy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zsqleaej.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jtkhehzt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2jyihkcjp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2csneidle.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2dbukuhet.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2sctpfhsf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2lstxptxk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2pvvnqyge.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2efiisitq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2thwkrjgn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2drxwwhki.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2omcylols.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2doaxooxh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2erozqtrx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2afdxiomp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rbwgnotq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2nlzldoie.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dmcqpown.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jmviqzla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njvndezg.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ryyducob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngfdaigy.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kmisnlcd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzcjmib.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vhwitoip.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2txeqtfpk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2envqgzai.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2nwviutbz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2konphbhv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2imzzqdbg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2bkcvnzel.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nxxdvpey.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jzxvspfl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2fjlwliub.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2peqepkrq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2enazvxml.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2lamycqdq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2hnpndogn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ouomhmou.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2diauhvuj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2dnhrxrkk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ahltfdza.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2joipbcqp.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2esopqcou.html


<!-- 参考信息 -->