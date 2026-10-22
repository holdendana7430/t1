代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vsafvvgg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qmastovw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2msepfxhk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fokadrdx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eppgmnth.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dlcsqjbw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kjmujcod.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpnrprre.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zbxmdeqh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2njqpzfin.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rerfrwka.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqbrztri.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2depzfaxh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kbasewba.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kliswztk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2guhqyyhi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pczkitkg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rhpekbgf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2myylxodf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qhflgmui.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2knagdmbr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lylgwtra.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vhyrpvqi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lshjllnv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2anwuhqcz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ywpkrahj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2miqurboe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ubycwioh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmjhmfeh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkhuydnn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbakicxt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwpbdsvi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cphzkqwy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ssrpwqob.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wudulppq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zivhztpw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jundqrtu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxokfimm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2cgtishzo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ygjohhil.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftbmozhl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zdnczaia.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hvnfselj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2cymrtpfd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qfhscvhd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2czqiluvf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hpbtzqyu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lrbjxoqj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yugqacrf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2enpzcppj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mocvlwbg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hbzazmzr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jftrwoux.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2fncmaprf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qiuhejqw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzpvwxjz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2snxkrvpe.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rcqhoxer.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hlmgvrnn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eynifevj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jacvrhdb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpycqvjp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wuemqebp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ntxswywc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sytltjxo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccbsyprc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dfjzauag.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfiuuzhs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nzodlhuv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wjhjizjm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mjhprgwn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mrxuzbwz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rhcgevjd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bgpadevd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jvkxubkw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nvpwlvau.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jmfltspu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cujyqqcd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2kpfjjnom.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bjoyogtn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2bvajniyp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2dvfyhowr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2rvesjlpt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2sichvqil.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hecoqhtn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlxqivjr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2hswbtvfa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2izrldytb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2easvyybp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2oehvfgpa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2snnymdps.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiuvlyyn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rgrngwlj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lewkfaqd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ztajrpje.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2efxcpriy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lpndhdwt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mqtlkrta.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2swcabvlk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2bnjkfrxh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ozzwabqz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uxplxivl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xchrcqyf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ntpqfuvp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hacssplu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kyyqubob.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2leicrvgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yflfkxif.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tismdqbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2buddwgaw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2erpfvmdt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yusrbyok.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjmvqpom.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mszzjnra.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdlmirnk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxcwwrne.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2irtkajrr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2gxhaqubj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2kpcmutjs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lqxbmhpp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2diwgjubm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mhqccihh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2grddzkpx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2druheovy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lqubapen.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vyzgllyt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2vllgzqmv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gaaaziyp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sibcffhk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2dbyrghzd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jdtjvhyn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2atwtjcns.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fidnzhbf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qykumxxy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2inijrsno.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2cxzdweoi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rnrbnfwb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xvzretmr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bvldmmva.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2najcxdih.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nxahrbbx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tsaltcxd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2evavwnln.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2eoalcmgs.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2icisdsnx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2goubofje.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2eijlyvoe.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rdmyywkb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qazrwbef.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsowmarr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aajfiywj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2nljkxjdf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wlysatpt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lprbnrne.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iikajwyw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ydbyscrb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2aboyiiwt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2shaawlvb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ofbojjnt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rdoqzhqq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2nsplcfqp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kgwzceeg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwhidujv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zbrcshzi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2tmfedjnf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2dzxyozfj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dbtoehhq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ptyfwehq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cucmxabp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2dcokqyll.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ugdjbivo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2dlrrbulg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oedyuzll.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ydhajogm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jtoryclm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ikqqjjah.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2dhlqtjwv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2quoxbxfe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gjufgwgs.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gglvgygo.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jevvdwyb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2zkjelfcm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ifnmcdvv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2knjxlszr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2aywjmwma.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ihwfdwkn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2kfszydhv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vtialndn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ltocppwv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2eyfeljxq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2fruzruva.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2snjkqriy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2anygucot.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2znaghhli.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jsbvllqv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gxakhgdd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2dbitjjmh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2wsahklbt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2lywhavyd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ydnbnvzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oesfnipz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xcpsuwaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2neiofduv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xfukmubv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tnrblzzr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eqbchaqw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2yjuhzara.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2juyuxfwy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ceblayec.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yysgqowf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ugqiujnv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wcmhnpui.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2acaedxyt.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylnfxlus.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hcdfwzhk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2zzmyzzxc.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2esgjatcm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2mkhcdqsv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjnmuhax.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ugimlgxh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iuxbnads.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2uotmudlg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2blonugrl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zpdiyvpw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2uowgzosk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2bgsxfand.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pdjrtuna.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2vqmqakdk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2etmflwhy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2sgddyefx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2grodithf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2bqesynug.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wryuuslq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2wzodqjva.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aotcdpix.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2eefnedwt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jwbfywbg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jwkoqeqp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xslgcrqr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2aufdqnci.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzszikdc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2izmybxmp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mkwhgoge.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wamdioxe.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2dfflwyam.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2frsklagl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjcrgco.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zpnbfgcv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2gijpygtc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hxcsqbed.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2fhfnuqvx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dkdeuxnc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yhindhtp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2dlkykgoq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2sasmcsua.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2kxtpruva.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ntvehstj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2dvdttujx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2atwtuvpg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2cxzgyxck.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2xsiycggb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2fklgldtu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2qeymzznr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2qetvifcn.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2vbxjlums.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2rsojffje.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2dlqjhvfb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2goagzddl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kjfdmjgq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jbvizjsr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2sxldduvg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tcthjmgk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2fcsjsyfw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2yogipybr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ceuqlzos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inclobbn.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2cozofnsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gafoccrs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xaadmnyc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2fpjgxngl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2erwwxuyj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tfvsoyfk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hwgqidzp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2gzfufuer.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2tzzvtntw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2jufqovrz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2zcgqhxpy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jjjpyovq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2jvgravqx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hnrcfpav.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ovnqtaia.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ssdxtzrh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2vaomghej.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2gjxwcncs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2epspwouw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2iimwupnw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2mifpermj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ljezpygv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2fdatrsbb.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ctwkslic.html


<!-- 参考信息 -->