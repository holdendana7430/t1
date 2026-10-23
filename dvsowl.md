代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3whklpmaf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pphwbqxz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3iguzdndh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxuasrvh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3otrymewm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rwaxjvoi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jvgrvcsr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tipmgeln.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jwzjnuos.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuzthmjz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nvpquwii.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3itwtqlqj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3seodcskl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ptaeojgo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ljgqiyer.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3prryspdg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kzqpnmpu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xqzaurej.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qssolldg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ijzwwyyz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3nzjzrwcg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ehyzfrpu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fzdcseyw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hhzjdnxq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3omnnckyb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmkcglly.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ooifroaa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3reywbaru.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vldccsfi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3uxveyqmd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ohtngxzn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3cylyovfw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xujlruhi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttrqscma.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cvchycek.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjfaqaxt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcttbazb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3htfmmvwq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3eubcufad.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3drxcogsn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3scpjkvjo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zatuykkw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dezoomeg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fajilhds.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ixwmhybm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3uwscafau.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qgcjctcn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gdfaxnek.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dbyponca.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3lhnkekql.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qedawbtj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvlcnoom.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wzbittaa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zrdqmsvw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjfevzvk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xorltowc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wprljlty.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvzudwxw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3esgjskxz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xvdvbvmd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3umlymajg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmusawdp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xdfyeleg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usvtjezu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3auzyzqzc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ionvnyoa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lteteuyw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cbaoukfs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3usmgqvbl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dvqoqcxr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lwxdndzn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rnhewzdv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3irntfmcs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bzmdsuen.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wabscxvs.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gvklovqv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rdmwtodt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fqjmravj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3tsdbprjc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3fephnohx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vejydkwk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyufoion.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vmwfkgln.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mlgjdxvr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3klwpaxyd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ndkymjwm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3tgjhmxry.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amdoqmls.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3isckcrew.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aamekami.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hfvsbhbz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3crbhqvtf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vaootkue.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3akdejlyh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3mcnvzmqb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zozdshap.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3trioqvrm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mlbioaye.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kzdnzxgn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xrnktmgr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kgdiamln.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dldphwye.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zuqacplx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtsjohsf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jjgjunsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rddhxdeo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3aaerevot.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ipfzmodi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3laujloxp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pytlwylp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbpheuzq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hojuwexn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lmrsfzqv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3rkbzqmmx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtoqnafs.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3bvlgqigt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ueftxfsb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xsobikna.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpeijyys.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bjjrojbo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uinilihj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hbrmwvit.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3hminunvo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmhsvkzq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3engtzsym.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3pmuqhacm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gyvnnnca.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vsmgzgtk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ggwckbuw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3auihqesz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3fuxlpbuq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3yjatewad.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ulztnqjp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zgsovppm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zjotooyk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbfxkvlz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjasclgl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qypcrazu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3euthjvur.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3onivhirm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3swgxmdlq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3abcerple.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3grlaisau.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3pqdvemdb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3dqbttrqh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3okmnagwa.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkdjmcjz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ikevuxxp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuqfzyt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zxebxvxv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3gazigrvu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3sxnlhczy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3osxjfuvl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mqaquepp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hlmrrqbm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zmymhcpv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3clhavpsd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdfnkjp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3qaanlswl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3kvigdxhb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3esttxkjc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3akchogxv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bamofyuv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dwaalzvo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ejsiekgg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3uvfbnctv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lsuukibo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3izppccqo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ddgzwauw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ngurtwcn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kpadnugt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3fcrdpezs.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ixrriupu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ltfuxsuf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fughkyyu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3kdjcgicg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3srjepzyt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3pteyxhpb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3vcdsrpxu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3qkmnrixb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ifitbvtn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3grmpbwwb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhbgvfbf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3rnneduqz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3metquizp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3vorqfjzj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3dcmfnpxi.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ovavwlob.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3lzhijrwp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3oetioscw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3imzthbpf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3owescmft.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3dmmpuudk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3fvuadnba.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tdmdmhcg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pfllnsew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfxywsoc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dtsvtjvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxyzuqft.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3apkzjlqj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzfjura.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cqrpunnw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffnxzfwi.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gdcigmgu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ugsbjccj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebaqvklr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nvhpjase.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ifnrvjpp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pavceugv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gorxuqmo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cvgrzahu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3sxzqujnm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vpgxexuo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dxjuaxuz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ckozrbzg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bdvdgwgg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gbahydma.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3yuwqddtd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3yrisjull.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3yxxjfizi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wygfsvre.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3iivzxxhn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3viwsklmf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fvitagfj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3vjhgnqhk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3fjodnwsc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3evjaqqty.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zdkdktcd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ttjocigf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ljybfyjg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jcpkpvxz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dxsmfbfy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wbhawbai.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3foykkevl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3nsiadoda.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cfytqkbh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3oncvesbt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3teoecvgi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vwgiimwh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mazqjrno.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3natyrope.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zdxwrbam.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rxhkeqvq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3szosflib.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3pdhfuxsn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rugyjyhv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3sqmcftrf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aguhdttw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3unsnttax.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3olizeegl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3bcifbcsp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3fuasyhxm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lvesorjf.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3hunnjdnt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3gdzipqol.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qmacxhuk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3snezczef.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3vuwnriei.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3dwrxaqka.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ozzrnaxl.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3qxseirbq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3vvrvyqnd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3amsypxos.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jfasbudv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3rpxlljqu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lzjriemi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3yhrllbhx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3yxoamivi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ehvoddwh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3cwhfwveg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3nkslnubr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkseizou.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3lorzagce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmhtujtp.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3litgsugf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ksrdmfjb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3armsjlqj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3rxiwbtob.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zoquxnon.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dolmvyet.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3gprilpyg.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3rycsozaf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3xfiznptw.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pihqyvdl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3vhtpvnhg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3srlgknrt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3nrjppbfj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3xbemjelj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3kiwseupv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3wjkdomcb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rnjvnazy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3xnwlbrub.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3slljacwa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3gfwyzdhi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3dhsfsnyt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3almkzppf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wyrwxxoc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nopftiau.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kgywatux.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3byzjqcym.html


<!-- 参考信息 -->