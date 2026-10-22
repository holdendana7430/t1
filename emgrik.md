代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ocgqcioe.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wswpcnks.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyzqgaih.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnpkdztw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qamqqchg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rsekouyc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ansdzfgf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2uadmrktx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2lznasmed.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cptwqmbl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ezzzfxpo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qvslrjep.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ylgogrhv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yrvjjxxv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2levutbin.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pfceptis.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2yazrzsyz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lzmlnmzb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2uvuohzsq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uxnwrzrj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2enryimuw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qanxialz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eoaozuqa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xjtcodac.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2cgrylvaf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2euofqlux.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jmsjarid.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bglhwgxp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kcwfvzzr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcwnuiyw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hfwomrnu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yochzvow.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jwgkdedo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2nzljtfwi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvzzzpzj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nbqxopdc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2samdliof.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2compnzwu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2otkpkkvz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwgvrxaq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2sgtoezzp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2tmixxyjy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pwiothph.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cydnmvll.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pymrrpyp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ugxyzuce.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ztupciik.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gmocntbw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2motqrsmt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zdcfrljo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2savbommr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2idkojunv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cqttxfpw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hdpldpef.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jewkymvz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lmsuujqn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uawcuevd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnwyxydo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssjheits.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lrjpklny.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vmhtjeaw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgmzjlgp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2dymljpsr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hkszrgtb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmviojfw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kcioajve.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yglqtycf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ddfdugdg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ltmuafnd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2eecnlspn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yhnstdgu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pcegsqtx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2edfkdwtl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2igydytew.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pnlxsyvd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2clrlwgvo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2felyukpz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2imzsognv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ysvnpmmr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tjcnqbnl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xuvhvjln.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2oqsaptly.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ddusftel.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2eomoqfyk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wvezwwsa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxtwmspk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tidedlev.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2znyfilvu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dcgbeefv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2afcwsuku.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qmpicvmi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2enfdbqxi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mvkgozjc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2twpdtuyi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2agmmlzlv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pfqgysjc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2oondpyvr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ihvyciah.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ibtfmtxt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hozvkjmz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fzozadhf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cibbyakd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2owueehpu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nczwanfa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fkbfmqdp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2fjordqhd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2plmrvmbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztxjkvly.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2bfajjudt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlrauwxw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ddspmbly.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uspmjhcz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cxwajrzp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2arklqyff.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nwxsliou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gtoyfowk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ktbcquzb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2fsbpfavc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2sgswdkdl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fvnevlva.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fbnnqvgk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2drfxdhai.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2trbopntn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tglfaaix.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2glabmrdt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2iauoueuj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2lmkhkcae.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijlwfdjp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yldhjxwr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qtpqryyr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nzfeteoi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dotbqtdf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cbnktcqv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xblewxwp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2izjwhyez.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fktbgvkx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xhgnyepc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xarnieuj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ggaerkhx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpofdonw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvtqxdbf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxuysczt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jucgcdud.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jkiobpzb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mqebbijj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylmdxmoq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2egopcnmi.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2eejfjbuy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2emdmepao.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksodadfz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eipgpgps.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2drrkrkpo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2oamdcvod.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2kieeiiun.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jumtguug.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2akelfkmb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2foowcoqm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mwavtkvg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vnfkufqo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tfishlka.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ingqnvlx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kdwxoylg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2bvxifojg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gkuixcrw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ubwvcirp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2hwsfcuib.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vkozejoi.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tykzrhxy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zagwwrfz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xvmkcxxz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qgdrbgce.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wpjdqast.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ecpxniuy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ufthgwic.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2avezkisi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2hzsrsdep.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2yjdoahur.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wlynbtbx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2hrmmjaap.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xuwpzpoj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2mniqkuai.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2twiehepi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2isonpyzh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2rtgoebow.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hzxpkful.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2pqanpdtl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2cbgnqltg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2cvkyqpbs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mttnghwt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2dxrjizjs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2lbothkjv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2odgjjtkn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2cwvmlxqn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zgdisjsl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qadooyld.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jpqrtzms.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2pwpbsuev.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2tqvcrezn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2uzmfyvvh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mcwhimhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcldhtuj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mbtgvceh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ototewbd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qewsnktc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2pwyesvez.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qfmvpdhz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fuviccnj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2csyojufg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2htbgkhiu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbgsduxq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2crvpnoxh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pcxuxkfm.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2krajcdjq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lxzghgar.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2kmtqgzfq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2gxqzvrak.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uvncckyd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2xybycgkm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2bonxqbsr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lpbacevp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fdezdbec.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ckatwmzr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hoyikmib.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2cygqjoht.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2envoronu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aenqjaiw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2osdlrrtv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2vhgtkgrb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ymnaqrms.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2tgovvfiu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2yzererib.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2zwbbmkbn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2clavghag.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dpzusuyy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ivydzjml.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mqihtefm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2fjwoqwuy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nhbdcgzo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2savfeice.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pusrqejn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2wmfdoqvt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pvnxcrci.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2knkdcelm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ceaeuaux.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qukceafl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2futhgrlo.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2svepqsbg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2hncjzjbi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2rocnysyu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2aywgreoh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2nvrvbufp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qejcmhck.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qskwjpuc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2azwlarkx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2prvdfytx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2kmjmrefu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ckyrzxie.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2fzmbtavd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2tgdnlaoe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xnerrini.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2vxcxavvz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2jqjprgra.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2oliziupl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2vlcfahxe.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2optztkny.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2egzdwuzp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2vmhzcgat.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2grfwspfa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dnyznydb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2srirbzgn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kprsxwbn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2pvuijckb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yvqsznao.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2bdzgnsid.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ksuacqle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tesweqas.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2hsigniwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgmbgroq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qxnxihqr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2kwwsguet.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mmpoytsm.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2uodezqxo.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mfiopiye.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jrpsoorx.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2dzbmuuqu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2enbmpjda.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2ynznzuim.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lmydnglu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2hsgvrbuw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ehayiltd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2rcfavejp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ancrzghm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2wvzkdofb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2gelludlx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2djbyscav.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2asocapzv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2faiycqmw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2hevcvuyw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2zwbmglzi.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sydfqvew.html


<!-- 参考信息 -->