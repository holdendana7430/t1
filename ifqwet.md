代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qyazfutj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ynvlrtcm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qmyaneyy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rnirplpq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gpjcvmpt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wpyspcoa.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2juloufev.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpudmbdd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2juerrxtd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lbnrerkx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tlibjluk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ckhkxuol.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2oanmearg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nhrnezdy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ycwwkspx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogwsalif.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dceacjzl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dutbhtth.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vhjfzoel.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zcyifdqw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cbpltkhr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2crhewqxx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2kivhlspf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rkoxpbuo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jknzbgnm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dnhngvtr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sobwslyw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2sjsaveua.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rgqxoerh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hbzzxquj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lakfpero.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2abmmjvsq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtrlcnch.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkmplwad.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2imlbzogi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwgybccm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qifkusmb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ldtguwau.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xeamlacn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2rvthrcvo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2fyiznkfa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpcbxjwf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nrehchxn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2uilslvss.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ohmqnuaf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qppgbjhx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ltmgfjsz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sidsgdsy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uptxllpb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jtsytibc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wshirbnf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2uhcgtptz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ktxqxkik.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fuyrcrqh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cgaawpjg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2opxpqoyj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2kpvwxouf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nvghmbqx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lgjdlbic.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uevxuybc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gukqyhec.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnviucfl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfafujjp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mscmtvpu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2uajtwqfg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yuzlhtga.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vgadzqpn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qcekuabi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwcclghd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ywdcapak.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2prkalqoc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wimxfhts.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dfbqzmjf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lgegswyb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kbwemdpd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fpyyfezn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wpcagrve.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ptbwasdw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tyrpjvin.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bqayiufs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pvozdses.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2rsuytsmt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tvmeuawr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2zvxqwtsv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2zmftqmai.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2oxxuwkyk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2madeqart.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ziiwxxgd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qafxrimw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zujjajwk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2nrcgojpj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2axxonlyn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2imaoqkjc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2awlbmzvf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2szdaoqei.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2knrfgizj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2aegnqzsm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zihkglzi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vswvcwlg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2tkzrpxho.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2nueuxubd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jenfnlyp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2wjisyuxk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tksttwok.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2onopbhhm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ghwvqhni.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rssdhxwx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dovwgint.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bbjvmjsr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xtkpqqnu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2kuqbpihh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlplxrni.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2uuudgwcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlhoabor.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2yzpihkaw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bicoevwa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjyfqjqb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tcxqlbup.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2osueouhj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctwzvosg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2emvkaaqm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2yvpmjgrx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2htclgwpb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2yfelnzef.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2qhwyinkq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dugxxzvs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iczqunfc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fbqaxsqv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pajglgxh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2hinjadow.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2alputrir.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qqmulkdt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jthuwpde.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2hpgdhgtk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cmvidkrh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qzxmkpwq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2axsvdhwj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nauofjvq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gddwpqwb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wuujcfjy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mbobawsb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2efjvpjmf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dstaofwt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhalwxkt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2geiajwtc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbmokfya.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2smhpenxe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wodzssdg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jbvgmcgs.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lzuaeumh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2zvqmtnwr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2vklszydi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2mhihcqxs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vodblqgj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2peijaqae.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2tadpbxqh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2dtkfhpxa.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2prhezaoq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwbocpfr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2hjyhluro.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2oqjhsbgx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xefbwuzp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2svwaishn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tmfhrvkq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lgwohsza.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2jjwwycig.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2moqizset.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2opsfklra.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2yycunvlb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2aruvbveq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cdfqwmgz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ydvhrowv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wgexsezm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2cwhtugco.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2vjhxwnjf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gkuovzro.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mtdjxwuq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2kaomjwdj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2nvzpoogf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2cuzdqumo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2srrgzzqf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vdcqfsgo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2zzlieppl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2mkagfzhh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jaqteoom.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ncjjpyyj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2riiztinu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2mfroegbo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gsxytfrl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ouwefgzi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdjthem.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2indrzexo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2bxagrifw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2tikzymtj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ldzaesdg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2lpplwzek.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2cjhptinv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2fxbbbjct.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xhkglsrd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ewiiebny.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2topzgkeq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dtujktbn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2hddgrsox.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qvbymlin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxohuork.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2deptiftq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hweyqriy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2arjecrir.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gstydkrm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2phwtjjgc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vcdbcdvl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2edixwrsp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2zoaykmqc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jkwokhhs.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mcmocsup.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zmnljenw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vcxwxldf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymsgdvlg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tfmsjlif.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2qljuueon.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2llbpugzg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2pbpwzymu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rpnnsmrx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zpfmmifu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fglaftyw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2oreicwzs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zkieevmv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bpmwzkuz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mnfrmhxr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2freakcbq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cqqqpdah.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2nikpjaqn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2fuxayppc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ppiavnru.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2smyxtzdm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqirkujg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sofxnant.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2llnfzhzj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xrcaewqj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ebmgjllt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cqeippcf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wgxaclqn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2gosmyahu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2kjvaovxv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzctobz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2soxxeruw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ezrkllve.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zxnvuvzr.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2ailbxhmc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zfutibcb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ozmkoglu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2suehrxxa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2xqbktwap.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mwslxmkc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2qjrzpiyh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2abavagtv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rjzvszqp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hrigbdxm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2anuvjmmj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2mxnuxdbu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bebyjdgb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2etkyhzjh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgggsug.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2pcsgdvwg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2hrfnonmm.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2cboivqoo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvivvkx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2gjyzeurw.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2vpdeqctk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2lprowtak.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2tzgiybbn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2hfnzafhe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2shxtlbbr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2rxwabnsc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zfaeusgu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2kkvwuqzo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ptirsmgf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dwymyfal.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2wbespiyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvzybdun.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2jtmqhdix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jghrjopj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ovjsgvdv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2pxlrwgng.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2xogyvfiq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2vyatrqlz.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2esjgoiph.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2rlvtrnme.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2nqcrmkis.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2gocolgvw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2frhnuncs.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kzwheuoj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ajzojscu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hoxqayfr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2vrmqhtbp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2lsdmfbag.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2rmcicows.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2jbjqdpov.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wbcnjewa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ovudnckt.html


<!-- 参考信息 -->