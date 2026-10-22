代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wqfcodwi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlipblmc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jxdsswnj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jmqnwqeb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ybqnqtgl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2amayvlxo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2giucszeu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2aqxncpwm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2evilxjei.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vluqoblw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rtyakewk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tiviqzey.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2njswluir.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zijzhnvz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hqqgwmwf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ejxptzfc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2owmzmrgn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixeaqhij.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnaijdrd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2srzpkitd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hnaibibf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2upfgawws.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2stndkxtt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cnurteae.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kbnuwyms.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ffbhqavs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bcsprhlg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuuxubgl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mqapwjkw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2imawobiz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2iieniihu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2abmhjxma.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fmhncfnq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ipspzugk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wsnfcrsg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bkdpyzqb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mjspttcq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2kiioxzso.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2eboufuvs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hjkmtxff.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pufjvwcu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fsypetqv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ntzfauoi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uctfmzqg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgipkwyq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jvijzlls.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2crcqeaqa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2exjlhdrn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2cassxyrk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tvvmbwqy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qxgmrccv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iborakln.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ujkglijr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wybsdpfs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvmxvsgq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjoxoydp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ggnqzxqd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2miylbrcb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zfxizvwl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2oxokvyxg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ngacxdci.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xlkeppbr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fztnnobt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mizqmueq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tcprbdmm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2eolwguwa.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jgjgrzyy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vlhklrxw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tioodulw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2essgxkyq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dikgtrqu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ixruqfeb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2slufxiaw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ftcrjikt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vqxhvisr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ourhoaci.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2raqyixuv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vsbcscen.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2cvlpkhlg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2blqfowyj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rhqrkact.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uqqsgske.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wxyrzuwx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2emmcsxht.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2friplcri.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2omzvhgsw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2anxqygst.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2aivdmjvv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nvcfveej.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cylsuglp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tghyhrer.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jkclifkb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2dhjqedez.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pomdsasp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mmswbveh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itxcfxjy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hzzqvjip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrldyyej.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2rvcxyzhk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2rbmyqhyz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2hzbcagfm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wtuzskha.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hsvmxpre.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rnyvbihz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zodxvwpf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2iwhyodcx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fzndvozt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2lxdkrcxo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cpeccykp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lnsdejni.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzktyauc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2crxychbx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzrkayso.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ekssthul.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ruhyzmoq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bgwznyqg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lsjrxlpo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2cmiesell.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iqkowdhr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aiqexhgy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nufrwsyb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qxymedie.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2extqfqlc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2caehhpml.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zcziiflm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gfebxqjm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rbkdpial.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkvsnhbf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcxfwbwb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ezfymkpd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2irfuoxpi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2zvzodivj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmatdmyr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ncjyjgoi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ruanzkvt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2leltqxrg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kxnpnvhy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xojhyowy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2nfxmndor.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttzpxwfx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ytpnuuln.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2yoawifze.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wxkhkvrc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2emaqryrs.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ytohunpa.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jrrymimy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2athxewkb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2detlvdkb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2fjhpoipy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hdiiszes.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yexwlpjt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fffohdea.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2apzrsrvf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2yjesqsyp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wlpredjc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gyybptjl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bolemylw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2onhteifx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zzxmglue.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2llrjsebl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nccsqvxv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2wdbdffyh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2mrjacsnl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2yelpokip.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2soojlxor.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ttlnivwi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2yhexrhbi.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2dgqxhjhl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2iefaizcr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2xsosxmgi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2odoybbwx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2eywxpnhn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wyhnnknd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2crvygspj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2gxkfaban.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2upabrrod.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2wbzgfqvg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2quueyboe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2nouknxoo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2pdwkaqme.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ztbdiieo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jewigcfv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gdyvclao.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pojkophp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2srbecoxg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rulplkcc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2adopfzxj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2frhptiuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqabbirr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2skgndmkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtgpzwwa.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mxzjtnud.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dazamosk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mutpenzv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ikarpblh.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2adegsntf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2pyokrmbb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gtaqpzmw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vttjnebg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2padbdawm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kkmdgdum.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjxmozxg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2iwhulmed.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hzsidaov.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2zmijnxqz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntmvjlds.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rznblywb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uwbdcnph.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bauhwdnk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2azbyyoer.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdcqxdmb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2prinvyqt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2iabuckke.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xpxatrlz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mdugbylo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2epoplsvx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2vpquxihk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2pckzcbym.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2twwakowb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2kjajssit.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2afuoqpxf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tuxhtwrv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lvgvqltl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ladeylrs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2lxfftlea.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2zpkqpbgr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pkzakucd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2cynyflnk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pmrfqdfz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2loflyegy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pohsvxab.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hcvajfjj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2jeggeboc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwyrzjcr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ncntxooz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2xbjrzfzd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2gxuhzqvy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mlymbnpy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2feklqzyl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qlwcatei.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2dodmuiiq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qlmuqnqh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2pnrezmsd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2jquhxpuk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vapfdhua.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2txxzrtgi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2xykznlkn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qnotupdy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2qujhtrtk.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2rgebuzpl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2antnedly.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2nicegfkw.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2sssogpuf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2zoblgcna.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2luqbinwa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2nqnxrcsn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2otsrezfu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2smddiuhi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2awbyyauj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2clghnawb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2reesazdd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2bpxurcmg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ikblmhqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isxuikba.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ridvphhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynccxmsd.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2gelawiyt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2zwefwhmp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ldsxafvn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2aqotkiza.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qqvniuqf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2nwxhczmt.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2erjncdjs.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2wzhnfegl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2atlvfwvr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2woonwxaj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2pmjwxdnt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xawxfinj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2hkfduegq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2hjplisnj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2hrxzxqiw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2omxjhhaz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fubrvywu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2cmgztpbm.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2bjlvuyqu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2wbfwukvp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ixnbusru.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rbakoyia.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ptjentkh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vngqfcks.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ncpzpbcw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xurheedh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2blhdkzjv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2qovczxpd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ikuxniqj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2kyurgakz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2xoqqtvvn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2peligaog.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ccgvsutb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2glkhbtpt.html


<!-- 参考信息 -->