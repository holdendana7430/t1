代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yoqsjylt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lngiozmd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jgjznnjg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ywhuhoid.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2choihrkd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2esdtlivh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezzjunqt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ljmuqvlz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rihmwzea.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rxqmanoa.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zqlfrqlj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tormvcsl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zsanhctn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2uuspxdzx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zmshiozf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2psczhmda.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sfwwdysu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mlyguase.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2cvpsnzrs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2udmhithh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xnsjmsbl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zhtmuhtd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nrvpbwoe.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ljworkaa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2orksxccv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pycjblvy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cnzyhkof.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hadkrvxe.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ilcyjwdg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2fmnxnolk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xippbkbw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bozjzsuq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2awmbqiad.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzywgmba.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrzwoxed.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2cofukhdb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tknglleq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fjefkcwe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dzovalhs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2vpvbykkb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2fvxxnxxh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlecrhht.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2owlqdnyl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqkxclzb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hqtqubby.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pwnfoymy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zjkvrqxr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqqumhuc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uulqybep.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2eedoloes.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lncokmdh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mndokmis.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qjnaqypz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2crqdkszh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ijaeinvd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dmntdfrg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2yiaeytep.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ghyiqxwy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2diupjnym.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uriyxbkb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oschzdky.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kdrgiwiq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uczgremk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kuhcobty.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vatwyffv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfgoswoz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tvnqbjqa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dgdxvpdm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2klvagbwj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mpuzutzw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mttjynst.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppoiebgf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ihahczzv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zevbgmyf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2twhmukja.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2frkekmcs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fpiasdpp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hjtaoetv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2azjpaywg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wnvapbyg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lqgbtski.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2echapcyf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pakxgmpf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dnoslvnc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jvsjnhsy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jporishi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jcftfehr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pbxlrdii.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xffdmqpr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2syebkarq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rrcznlim.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dbmqyxps.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2oljhexsd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2oeiiqisj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vovqojsb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lafvqonh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jqtzgbju.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cozpglze.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ijwyaish.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qrcufglb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xrptwbag.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vpgwxesx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2doigudbo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2omhtgelu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2puacucbl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vddwwnrj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tgfzzhlt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2uofieffb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2btmwglew.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jxspjgxq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nhrwoxay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efkhakkt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2anlqcbpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmnogyor.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xydnbdbl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2enhzibcc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnsxivfo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcxzrlfl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbsozrel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dvghmoli.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2imuqajoz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2gmntyxcb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2skehqxvx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kudedywt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fckpuqlc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xbrjjclb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hojdkjsg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2amskxgmc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fxgfviwl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2fkbddiio.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xahrznqz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bpdqfedi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2horztmng.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2sbnghtne.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2chjoiicq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wglfvgbh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2onscjqnp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2atoeuaks.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jqbxxzdv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ccvbaymm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zdjwcjwl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2cfmyizxq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2oiviivnk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zygjfxyv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhhklmid.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ghhvxmit.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hskaqdla.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tuuhzozj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vujrvizi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2gituhwrm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2dztwfkxa.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ncpdqenh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2mleethow.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yyngagpb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ptuqwpsj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqrbgsmt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2jhpcsmet.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2miqpkuex.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2onxouwyw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fixjqobx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2jgihnwgq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rnivayao.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2frgwakny.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ksflmscy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2nddycjoy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2dafisyze.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2biicgyev.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kbayrstq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2mbfpfbuf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vnszwvhm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iucvpsjs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mbxmolcs.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bcnnoefb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xjyvcfjb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2waexkgzk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ydwfrclw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wpetyjmo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pxofpuhj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2zdpgtbkf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ivoacsoj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cwkuaxuc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uiqpufds.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2teigwooy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2zyevwuce.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2yacfzqbr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2rnwtayyz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2mzotoglu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2bucrobcq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2nosaathp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2xuskepnv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2npquhhmb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zwcjhrky.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2borcuxlf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bdylzxwx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ghbczact.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2gqukdven.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2stpdqarf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2unlxraoy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hwkzzdqf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cfdbsikq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2yuwyqaqy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ovvjpmuu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2semcnilk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dyocaqtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cshkpffq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2snyrsmni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkrfccjw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vzkeyaeq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fkkquzjt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vpnsgggr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zvpzeywk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvcacktg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2gkbdujoy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2fquaqcay.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mebhumok.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lnhyttwp.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2kyxddvrk.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cydvcyqa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2egteglcg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2rrpjbova.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ipswsdnx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kccjvccn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2npmfeyvt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ghwgqqix.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dpvidsnb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ibpmzcyt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hbicjhfj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2waavyabs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2phixiuhd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mhfrfpms.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2somxotyr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zrlojcbx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2qypdyfsa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2jktehdbl.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kafjntio.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpyoteod.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2azklorsc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tswgvowh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lbrehoss.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fkrcoedx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uiveuqvn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2nxwkspvm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2odtjkhvj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2junmmtum.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mknvwlrd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gagiwxgr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tkgzsjbg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kcfnuhhj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2epexwazu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbwruchr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hykszxzw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2tmjageou.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2zwgkkudy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uuukpecj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2bpmnmyxc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2beivwmzn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hvfgcven.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fxkkhcnt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2bdwxbsyr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2upsygetx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qiqgxfkj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2cjyklmlv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2xjqjkbax.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ssoupbzr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2doslocnd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2kmokysvn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2oxjkwiie.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmzufzj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2wrlxaxfu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2alqxptpp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rfbrxojb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2zhzboyzn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2cednpats.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qpnisxdn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2narrpgpf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2grnznsdp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2weancqig.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2nglovidk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ruthyyjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuxzkrnc.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2mbapoyjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxfkfxdc.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2fpicxquw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2shedoyir.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zjxmouvx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ehinzido.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xgvyheya.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2zmwpskkm.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2fnhnctil.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2loddkchv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ujdkwnbv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gmsczjdx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ffutvswr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dhmlutku.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2pwqkcqwm.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ldmqqjrk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xuhokdrh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2uiqbxmuq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2buzcsytl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ywzwjlge.html


<!-- 参考信息 -->