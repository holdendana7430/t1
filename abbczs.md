代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3soofzzso.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3oqlvamkw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kgmdukqm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtkmpuzb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qivtpgpm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cdlynxlu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wauqopii.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3elvfudtx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wksqbqle.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhnunxdu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gdzjecpo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3chzdhseh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3bxxycsqe.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3grwphvcw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vgzthnuj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bfzcxepi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oraplchz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fnkmtmbl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ftrmfvgc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3btukqcdn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xlnbvhye.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zhmwlqev.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pkjdlypf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3opihturz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbciuyyp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fwgaquav.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3agadqoha.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvbxtfpj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kyciscjx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jmceqxyp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3alrjbuvz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kbfykupu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bsorxzxv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3swowitnd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tmwwlmur.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ftuhsgpp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hfjdmxss.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3flupmxju.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wrbzbkpd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3njedtrwu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wsbcqkch.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ffoebgyt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mujsnmnc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vvrmbaen.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ipkldbvs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3pltotxui.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hlhfodae.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3exiuevsv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nugbgfib.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jcuhocpu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ahqsbupu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmldqvld.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3krcqoucy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjqkgmpe.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gmabvlpe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lhiqmuha.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xqvlbmff.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3direzpje.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nrdoikii.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jqtlffbw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cojmppsz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nmpqyofz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ntwftexv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuwvyaow.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lkwlztev.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jzchctbd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kahaohpv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cyuvmrbp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dfattfer.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3txjyjket.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xiuipkfp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jrexnbat.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vlqxsivj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3esytwbxq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pbidlqme.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3rozbfblx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3eicxfmsx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3dljnroei.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xljlunet.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3prylazma.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3hthoaefx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvqjimrd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3anrhbkus.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vrvnkbpq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mpqbarci.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rqcduzuc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgmkuimv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3afxzvhbe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mzwyjgun.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kkuzlpet.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ipzymigp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lrxqpzni.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ltdcgldb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3iqogbqwx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hmnvhdrq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3pjsqxxus.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3mxfazbhs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gynpmogk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ljziwxtq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3izxdrhng.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3acsayqwz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dhjxjnml.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3saargxgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3novropye.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zudypkcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxwtfkcx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3kiakeasq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cpgscwzq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfzeoaeh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fezuwwph.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyturwtc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mglxjgho.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gqbcgxlq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpqppnrb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gblepbzy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3slcvnedq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3amvdgdjl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eubcbqzm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvvmfgmq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dfwjgoub.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mashlvyr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hbjbofoo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mspnkrht.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tvvqpwpx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3grlvljcw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tpwylqoj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eldpvxzn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wjhjwhiv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ftqndvcm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3htzzwurc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3mzgfrwzg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3wfvogysj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kogpoisv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rxlzwxhw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zgyvkjeu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3aagvozvr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hjnldarm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3oygcktrd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qblspckq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3oclptjkq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3cfvwpchx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3gkxduarg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3dvxtvhgo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3wbzviowh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3iexceiid.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tstqpopi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jvfwgvqm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ahsyxcfi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3aekncaoa.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3cetcwvdf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3lrsjiled.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3knkqzxvn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lgmutfik.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xdmilzbs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uactzsqt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yiukhbtm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jpgivxay.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3eddgqyeb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ermotjoc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3tsarhkcd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rjhgixci.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3kxxqvwgq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wrnagpbp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fyneqalb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fxqavjsh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jnxufvbz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3tsuiqwdw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3okremufh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3szzkamsz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bnhrhtlf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3trjomajp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qowqdnur.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3kyoyfiqf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3zvebbqzi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hkjcbqbj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3llkieeqs.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3jdpuffpj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3oibyqgtw.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3aylbmeek.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3kxclqlrj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yaaqyxzj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3oqozhqxu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3rrbrydbt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3atnlqxhy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3uqzcttfm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3howtnjov.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ysirlszo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ahljohth.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3leloozcf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3smlyyzfv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nuaeqaso.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hjwuxhxt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ugqtxnax.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3rjrxeyqe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3shnwdnpi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ouwvemel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abybzvic.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aijtqdvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmirjpsp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vcpbvdcy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3apusxyka.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lmegbseh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3lkxnipka.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zmfocpdy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3eagozeqs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qoeuxqln.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wsplxfhp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fdmgjdcl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wautosug.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rufrwneq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cbrvaxjh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3lhexizeb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gczpopon.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3dupfmxhc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3arwoogaf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yvrdlywl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xozeemzn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3iemmwvmd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3rcysppbf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3jibhfmus.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nvtgohyj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3qvbdgsqj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3phsqwejl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3tlegtphk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3chvjwxfb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3xjydvfua.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3jhvdyjtz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tacthhiw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mrkaaonk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dzzbkolp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vjlrewxg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3oyxvxgav.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3lpbvgsdx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3umjlzewr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zhlqastj.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3chzhdxzu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmjxtqlk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xebrjfzl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfndayt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uzjhgqrh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3phaxezaa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cdnqagmz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rjtaxbtv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3qzijbjky.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3zgnwbrlj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nwddjcyh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3qgrltzdj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tcqaepgw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3phzoutfo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3izsdrfbm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3fpebrykw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3tplyqavl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tbivxueo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3hxigxspv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3srhncxun.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hftzdmiu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3xjksachp.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3mibszzsq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3gjnsxxcy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3pghhbksc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3hztvodfa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3taseqqqh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3pfnsntqn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3rxggmtfx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ulqgrpwn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mfpmggiz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rbabrxkr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3mirpfgud.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3nretcglo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3slbdakzi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3nnfeltol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qexdbclq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3zhjmvnbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pitjxdri.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ammncnfy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3elbjbbfc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fpkaooeu.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ksgbjiky.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vqqrncze.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rcnecird.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3lhlstemi.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3dtdzokhw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3eqgyqbmd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wvbwwikx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cpdnywtt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gglsifgu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3gfjxmnyy.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3pllybfkn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3icgminjb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3waveanrb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3aibmnrsy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3eanchlut.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3udxfsejz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3nqbsvnmf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3tbovvnky.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fdnvhfdb.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cewuekoq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ciuksrfa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fyyqvseo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lsxewtqk.html


<!-- 参考信息 -->