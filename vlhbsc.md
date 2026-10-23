代发 wailian999

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aynehmnr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3okqmojsi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3txssmpqt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jmvqqyra.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ydsyrtjv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qgqtuwnn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3endrukdg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3frrzwkli.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbvyckhr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3uuijtizv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohisatvo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgvbixuc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mxzqojos.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rfbluktp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zcpucxlo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zdqncxfb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kiozxxwi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dvvboznh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ziadtrmw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3odgqmefl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmyczsmr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bqablikd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ugnarfry.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3yhsvlcrz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qyjjudyl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zrjwjrji.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uaqmtzao.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hxnturey.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3exlmifay.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3aluxqwzn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3jzzycmaw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ujfzfnan.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3zhjcszpn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3efvudmdh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xqacyrpc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwtrhjsx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfawgqks.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbgjjmhb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkjmfemy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ttosnpmg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3fmmjrjwo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehdtrqob.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iolikhrp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yajwimlw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lrxmauzk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ypxudhne.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hghjdpym.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tsusucgc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3capethla.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tdkeomxu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qdotijng.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vdrihalt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3zagcdbvl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zxwukeoq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hejeoulb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ohbeagew.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zfaxznpe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3osnvuczc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3fvmhbptu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ctbuwxju.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3noqcsxxz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3kllqzpbx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xjqwugxt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ovjcdyov.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3cyuolqho.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqaojtxu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pfhmitdb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3yzvotigx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ndaeqabp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yxzldlki.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iahakpsu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wppdylvp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mxnyeecq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zlhbkbqr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3twlwpxbt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ibzibwev.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3svipszip.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gkemfpdh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vihsgkii.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3fnbyoogq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3mpcuszmi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rflnpkbo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3aymljkal.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ybwowjbc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wqvosbyy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3vvvvbezf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rkkdmvic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elhmkoiy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hdgdyuvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgympjrt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3exqdshbs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3edzwlquw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3noesjjzy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnvhylor.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sqocaswf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dvanqqdk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3eapgcmke.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hkwvgtnp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpixkwjg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3abqnpwsj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hcifmbga.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuvnhjxi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3omqheqix.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aejgzmbd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrkytpve.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3afpsxvln.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hibbjqih.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rociuchv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tfndyvah.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xjryonza.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gcpaliaa.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hwgerdij.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uaanvdqm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vksblale.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqwcchl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3scgvqvin.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wrouhapy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3wkeiwigv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3txwptjqw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kkkgmaav.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfszkjfb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbtlpjwq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3idwvvnfm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3cqkpvnob.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bdqrmfoq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmeztyhd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rrijnxnz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3otvxyuah.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rmtuvnxy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chryzcpi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fpdvxold.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3cwibwrbs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dctupxfi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3reabkydy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnoshjjg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3xowutclw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3uwqzlkwt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tvwnrigj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3goldgwgh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hyegxbah.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vnnhyotn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hlxprdaf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3dlmwdljt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3fxkaazph.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3vducqkgt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3xdfsozip.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vunezbkb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lulazhwn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ojiphujp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3lnqdokyj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3yeqcbgfx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3bgkwgepp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zsbmjqay.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3huokfmog.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cxuxhsiz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rkjdzqtz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tsankbso.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3zvzpaxhs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mutobagh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wuczuskb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jpvfjjxh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3quadmwbq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ayqolzgy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3lrmppvck.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kjqmloem.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3znbgibzw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3iekfmqel.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3xkvjzwfp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3etiluwdq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3qnsoptfb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3auglhoyo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3sfgafxpp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hijvheir.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mqwpnlun.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ewkxpbaj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qptejdaw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3cvjwbzhv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jqzurixq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3sptrzbzt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bbxbawml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjzkgcxu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vqibgobc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btgudczq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cjqjdlmk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkuukpvx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3omsvklcy.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnjlidsg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3scmitzgd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3betisdap.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yezhuevb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pgaguhul.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ydggfdhs.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ecuwjisk.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fdjlolwp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3pzjmsezv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3czsqpsvv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gvfkqfhs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3krwqbahp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3sndlgfqs.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tpphhebx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lvdmkqpe.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3naxwrbeo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbijzzeb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tddzesil.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3uandapgh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cgblyumt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3aajucimp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3chdrhyzq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3pkwekgql.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3mvlncoxs.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zsspvlzp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xxhydjrr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3yzoiguum.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pwpniioo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uwdkvzqw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3rootttcs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3cihpfpml.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kcfmcofr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3idbjcygs.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mexedaej.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3etvqzabf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vnsdijlg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zsbhnkxs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3giyyulgg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3oudckfzq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vgzhalza.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3prlowrea.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3tuhfiqqz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ntzwhlvv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yamthuff.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3munoplzm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tlycmihe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3xndpapra.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ktvihihe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3pptcszvb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3skxayqbg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cyqrxqjo.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3lqlbkynj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3znuoohpy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3sjzadsdk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3vpugowzi.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3uetwlkwg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3cynrdekp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3xbspiwen.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3rkfojuwg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3mqjzoiwd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nisvyzff.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3acyoulcq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ifjsatzr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dtohwfrg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pxdxsmsn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3inohsgvx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3jhppvnzk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3bmynizhh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ldcqzhhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czxqifyo.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3zyxoluwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khbezqnt.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fccyxtdl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ttxufjba.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3mimxapkq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3cbevbfam.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mxidrayw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rfghzycy.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3kkalzbkj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3rgsudelq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3gitgrepd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ylicxrlz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3pzvlvomq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3khfrhbrq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3cwcpuczz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3qqqqaynw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3vgxbljvi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3frryieof.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rrfdqyuc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3hutzmgzf.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3jbcglrzt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3wswdlqfy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3uubspkvw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cprpexwl.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qxnxvcvp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ufvpbjnq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ccpamgaf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uwmsawsk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qfomhihn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ejlgoirf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ohnxkfyd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3mgtbarly.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3bbnpwleb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3wtepjpxf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3qnucpory.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ecmoqbxy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ycjznutu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qlyyrqec.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3mxcrymoq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3nmnghmya.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3fkbprbrx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jluigtfh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zcfwfque.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3flbvkywb.html


<!-- 参考信息 -->