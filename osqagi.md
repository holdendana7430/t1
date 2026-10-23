代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfssxypw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3lpkyulen.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3usxwgmft.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3iqoeitrk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rrpzcrme.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ftgqmvod.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3clecbuki.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvfkwjgr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhhuluji.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xgbaebdc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jahdqapw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jgvrrygc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3deryaojm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tpghyrin.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3jvfthivl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cwsjbhmv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uoubxych.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qwltolum.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tufnscth.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bimltvyz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3mipxfnym.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nkzswbgq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3hgqfrdou.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cgtkupol.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yowkuryz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3phibmacx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3esypypnk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rlcykebj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vqfpjwjw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3dwwztmbm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zbwuibys.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pquodyry.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ugsiifyd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3glgvkaom.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ncizbkzx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmsltgft.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kxstxwso.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ceqalmdv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3lkbbejoz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lmltmjap.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cjibubaf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rxfldncs.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yhceofyt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3yfufwlim.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tvjsxhmb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vwyjvela.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hgqkbrih.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rrwcxpwk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3sjgflama.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rroihntz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dshhzvea.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nbcthsam.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3peqceaac.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vpkeidrz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uhyvvdrk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yyrglton.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3szesneba.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhwfyhhp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ewirskyf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3docmagmd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ohnfyimb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3reuzvvsu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvdxuoex.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ejmhdspd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qbtauozw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3szxsqhus.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zwikpmcj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ltklyvoz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3snqrjvbp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bvmhmoik.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3avjieltn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vlyoarfd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ufhuoanf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3iohekafx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3fgtcadyl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gckjglic.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gyijwiyf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gnayktct.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ilfsomeu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rebwxosp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3thskvezy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwffztpu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3fzolrknv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3eoqtoznr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3hzemosex.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3byxffyfj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3goaiswze.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvpnpdos.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3gfbybcck.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgyxtpjw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lukkuops.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dtykmwux.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ouzpozbs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hklqyrfz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ohzhfmpe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3hlurxqtp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ezzsljon.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zgiziboe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lodzosgn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3uvimgcqp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ctcufdae.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hflxvqnh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zkzdlene.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpoglpec.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nofnzcqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnntjrff.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bahjrfyv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3krjereub.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3erwygmwi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ozejibrf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3utqgdvvq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrfzotbq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qgfziukh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rsqhfssr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jizfxhix.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3gwazxcfw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3fkhbjdky.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cbfxxvvq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypmjwdyu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ucnsdotd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3urqnfqwj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3yxytfnvf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kqscvkdy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eawxscyz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bvpashyf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3eaygvatp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yyomcxbi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rrhxeclj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pelhaykc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ibqlteoc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3uceinrnt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zucdynbc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gsxogwcy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3wxldvwqh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3djcpxmno.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3txnoqhkw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nehhmbhp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qeaqudlf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvgierrx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pvtinjuc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wuolmopd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3drrkjkdw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3cpdfepej.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3cvxnirrj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3wxkexber.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3waaclrbh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdobwhlo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3imspelzo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3yexlgxmd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3oumorgxn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3oivvwnox.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3oiwhmfvy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3mjdnifjt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3miavilum.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bjrsnpjt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pyllfpdn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3nigzlxzx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3bkmrscle.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3aeucgggz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3adjgjjqg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3zsglieru.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fznsreev.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ulxibaoj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3adxjajtl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lmxphsjl.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zymdqtem.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kmxigetp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3xmyxgfob.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3svwkqjjg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ceniufoq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3iodymxct.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3nkinufxv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wkkbvpze.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3uqtbrtvf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dmylrolv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bpekrpxi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3zwglvyzo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xiqdzdez.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cuwzgebj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3qufgojfp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jyodvcff.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vsknjmye.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3kswjmbkf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3uqaakvdj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jrejboed.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3slogrhhk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3qkloofyb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3jbkvufal.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3sskjekwi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ysrejygq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rewggpek.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mczowaug.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3iltjfshp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ftkglcqr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3zrjbfjmg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ccjcbmpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kimfiwbs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ygizissi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dquxspwl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3iqahxgpz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pomdpyvg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uyomqirr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3wmesqmwg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ukdhpexu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3gdrkbmds.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkjvcadb.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xffvmqgr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ceoybtuw.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3egewefjr.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbztfnjg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3usrxffub.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3xxlpbdnx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3qdimldhb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3gdbtwvmp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rccckzep.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xyqxwyum.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3awyfigzb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3kvoeyxnp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3txycczgw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3bxnbvwod.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kktimvho.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tymtvcrn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ewxjypxl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3jauwjvaw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3aigbbwyd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3blkbeved.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ejppbrif.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3pzjjidxf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uuvodmfy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zyefqfpg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xmthpezs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zcuskyhn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hlyggcgm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3heainqvl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hlzpbojf.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3wservvqt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aklxhobk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lkldegye.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3yenhhlnt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kadwgvsg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3nhaoqtsk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cgkxkcax.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3srhrylda.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3jvrloqei.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3vkpzknab.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3blwwmknm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3dkndqflr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3srwdosbc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3fppfkwnf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xksgekzz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3vxszbxri.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3nvwfesks.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pdyrbxna.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3kvgnixuh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3shjxssga.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3iudjdcea.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3lmxtyodu.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3qzpymyoy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3sgljurbd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3alugaokd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3yrioaekj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3wpylmmjh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3vxerugsz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3zkslaahf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gpqadavz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3roiykdbi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3cwcvaxwr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qgpnsolu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ualplnwg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3jdnxfdvh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3wpwcvvzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csvuisvk.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3hefiwnru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odnqgmwc.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3cvbweibg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3wfezbwvy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nwawvoib.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3lwolxyvi.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3shhavefq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tfzqpaua.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3fklkjrsj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3hflnnemq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3zkidoaqt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3uvsjyxfy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cuqmeosw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3cunnfzlq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3rxbrrgps.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3vfczvwax.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3uorwehux.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3dtvaonsa.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3deegmyxj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3yvjhqwzl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3fyqxrwuu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3nngswtiz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3njibadql.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nwmgrunj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gvbtfxph.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uvboiilp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3awlqqjyt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3edgzlkpv.html


<!-- 参考信息 -->