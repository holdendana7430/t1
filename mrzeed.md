代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jcqxlyhx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ranwjqnj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3loeazifs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3foczoatm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zpiajgtm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzuoupim.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmqbikdn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lbzurpte.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfzprmaa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3bnuqvhax.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vfzjxdtd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gfuehmej.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3fhnwhrch.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3omwnbprb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3djbjfmtc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oolfhdcd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oxhuvhxg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ijnulefk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3yctoakvp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qpdjiqcd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3rrlvnybv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3awjcuhpt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wmjduydz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ikkahzzq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yvwcrkch.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pfpsdolx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xvqtxrck.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cskezsla.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lvxsvmbh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kopgbmsx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ukkcyino.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wiurinqy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3spsrzwip.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ionzghfx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3sggzinbm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tpizpobo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kfpyohcj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3eobxminv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvyrzhan.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kiihvjbu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3jwwirefn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqgesxpe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3teteymrl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jzarcjbr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qbjykcpx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ozyuxemv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xlgsrafb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohgaakdg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3surisrtu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qiwddzbe.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nrbaofqj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ovwltqds.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eytmvyyf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3btqndmxt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3mrayimph.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3crertzul.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3thtkvmcv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cuqwqarv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3fuiyoinp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyperfam.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxdsrlnx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjudkumc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3znsixaib.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vmdfyrdy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3nmioiann.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fflqyodc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ebyfxect.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wdigexym.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrywtzha.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rwknkxcy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jpllxxti.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3grdorfuf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fychyvng.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jyneubky.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ecdipglo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3duwlepde.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mkdmgtaf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kraofgzv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kgllurub.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iwdbjcjc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dujolwwd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dbfjorno.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3djpoasky.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qpdcjeew.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fopujzde.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3spyqzjcm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hwtjtepp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rovttser.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ebeutzye.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nlszleme.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ftznaymc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xfymzcet.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qzwejluu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3eagxukax.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3figtnxbc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vdnfcuoz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3moypzkep.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dredldku.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gruykbab.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3hmovhgpl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3lqjnfyoo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3thigdvib.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vydxxeco.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3igpczwlr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ratbggji.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hrqpyexi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fowszdvj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jfgfgzws.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3navpuyrc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3auhrvvok.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3adgvbvyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3woydfqcc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qjpjumsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvxwager.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mworiayo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wiwkslfp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3cxmceqrv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3usdevffc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fyccoigo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3emuscwfz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mdakrhog.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3stldrvyw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsbxcyap.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3pssuiiwr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3yrywaout.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tpnwqbkx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgzrqctq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrxkbbmv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpilxhgn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wszcelig.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3oehgwzxu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3faowabau.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3khwwslqx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3nhpppuqi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hppxznew.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gqkrqyfl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dvkhzfer.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fmahfbrx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3pvjchnyw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3fqfalvmb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3capioskf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3amingnbn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xbnstswm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vlvrnxvj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zuxbqlwy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hfkmfihg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mymaheib.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3qayxqkrk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3aenlxlwk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kziquirm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3wveicnzn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3nnkzjxgh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3uqhoatok.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pyfvozya.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ejzjvkdi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ghfpkaph.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qzyyikva.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ddwlpbhm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qpecwvez.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ekxoqzng.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3jpslfhac.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cofxwyxb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3awxlyxlj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3utlluscr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3uxkqdryg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3anwiqyty.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3icctkhww.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cmbghkov.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3fwuxfwkq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ejzqzeqn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3osobyfby.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wfhikitb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ulnletrd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rdarejdb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3uyqvgkev.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3jztvnwiq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vtfolomg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3qvaqgbut.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3mvgjbqzc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3lobwkwrj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3whdxspxn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3pxyspuqa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3iclzhafx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3bgubkpkk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jqvqmplp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3gsumfegn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3molarocm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3iaeuzbbw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3iobloojs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3cdjfhivm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lewohswr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tjiufvum.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3usvijnig.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3byxtezua.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3sqxjembv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3mnjnisrv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3lvqiwlbt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3vppppxrm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jopqgzwk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rkyedrpw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3nkzzpcfw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3eezfklhy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3wxngafaj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zneekvxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqqqpnqj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3zfcugyly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjftxjfo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3krcfmnig.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qidtpfdd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sejisjnz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zgsxubyh.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sweagumx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3rnvbiyay.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jiohxrgu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3amoitvfw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nnlkunhs.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3yzgnwejd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbyssqpx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tupzlcbd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kbrykjbv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wktogufu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ojvppkka.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhcowpuy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lecppnbd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3okpdfzsd.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3mechlych.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3jryiuidc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3peoapsyp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3hkvophmi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ifpvnpur.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3uvldjdio.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3kgvbninx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hqjelipt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3miiyzdas.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3byghdwkx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3cobxgauk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gdvegros.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3awemivgr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lflxhjqb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sdikmzuy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hzushrlw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3wvxqrkrz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ytoeobmk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3idpbmanc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ouhnojum.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yeloipbh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqdccbtx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3iusffobo.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3jqutewfc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kjnippgu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zjzycrpv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kojwownj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3iwwmtzzr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ztmbyvsj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ikbehruy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cztkhdlw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3uymtckbu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lttvjjxn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3hbhbhbwy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3bprbjuif.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dcdnqdpk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ubwrfctd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3uuatchgv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3sohezwxv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3sabguiku.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3jskahuse.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3clkipxck.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3acouycdm.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3vijgxcnt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3iclxudhs.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3eaqsyedc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3kefcfqll.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3twtlmrgf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ahbtufsf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3kwkgexhk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3emembrnv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3lszechmm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3vydjvdly.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3gegvzxsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oehidqsn.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ujjvjyld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atessiyi.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ducahhrq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ydjiphxg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3cedwxfrw.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3yfjoonku.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dgktopfx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3yasufdnh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3cotpuidt.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3owefihjm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3babkzscu.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lpkyiiqm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3khsvcszs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3zkiwzohm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3iveaudea.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3mpzbvhtf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3zqnmvkwv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3xsqbnkmw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yausnpue.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3gwthfajr.html


<!-- 参考信息 -->