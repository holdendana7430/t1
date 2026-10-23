代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pgismniq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tehalaye.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbiqemll.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bdopvrgu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3uglnegeo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vsjlthmk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yhdzbmkr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ramntver.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wvknsebo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhozczas.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3emeysbym.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tumzbhjd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rijnldgv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3srvamjyq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fpaqkdop.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qxafisrz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ndfizhsl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jogqjdrp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ixaouvra.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3mtyxhzci.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3gygbjbzu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pgrgfbqi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xrowhbnn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bfiinoxc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ypyadmsx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fmcjxntx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vryzmfss.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bktufyfz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qcwxjavh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mxcbmelj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aljzypft.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dqdjkxmt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ejxabsdi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3asfvzikh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fpdugsxn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltjxoiwb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3paxuoszo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kuhvahhu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hqfkbkht.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwpdqcsz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dwrukacd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3gphmxorw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rhgatafo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jlmvrbth.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3htdcegsr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3cvmjbsbb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zeuuiylu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hghaxbyj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3prxsydvc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xqxndwjn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3htxuzqcz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3inrutced.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eeanrqty.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3exjehnmf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3atbtsdip.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dybqymll.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bcdfrctj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3yppllbhw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3safwcwcv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qfbcxacg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvyptntu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dmkpgfnj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iikwnfjc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3barziegk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3znmrjrkf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jntnmcxw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qeaiwste.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3pqfoazgr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3eoneuhec.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vbtyiguc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dxpadixm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nemmsyfw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nhhlbbsw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3wfvzhvnc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lnstwlmp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3boojegsw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3shozzrtg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wfslydzi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3orerqhce.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jphpilrp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3umoqkeho.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3sfjlimuc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mxnexriy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nvwkpsee.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3kqetpypr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dwybbcjk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3whmthydm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qithbwht.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jjkjihux.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qiabbkqr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hdvoplvo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3yinhzckh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3sospfdhw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qckxwlva.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kyhjabek.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3spexiqyz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3rzwipiis.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dxyksjzs.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qzkcdnzm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3twrtwvkw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3onzqwckz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3sskojcms.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lpnbsvad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpbaufed.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zzoihxqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpmkucom.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zailgldz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jkkiordc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rngvchty.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3svdyxzxa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lyeoqpxt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3teefehzo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tsxkdtqk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bdmajiiy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbaiqosb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ovmurhnl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vvwyvjmy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3glfkxspw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uncoagvx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hvdrweeq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kggoujbk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gngvfawx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3dtprfikz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3voobcczk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wcdfbjwx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3tlamgufh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ndvvjvtu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xxyhliwm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xevrvyyr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kmzspnxj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3onzfvnot.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qrzyazhe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pldckpvq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3koodsdeo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3gdkijqbx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qhgqlvqz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3yeacdlxj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3meussgdt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjnuhcgv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pctsnovb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3owkukabn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymzpbjbi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jpiaveqb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3tngwlpmg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rwiwxqkz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hgeatbsb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wownglsc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lqtdscjg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3nhsdkods.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3nfyizstc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fralooqg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3dittgczt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hmeoiaue.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lprjtigz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pzcilqqs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rgaayrrc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3guvqcfhg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3vguvrhup.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3cxkdkxax.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rlkoazdk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3inamgnlq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3atellire.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bgwaitiv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3szkstujm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3stknoxuc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3wbiddquc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3nnkjyvwz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jibrjlxy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ldgzvosp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3laalvwqr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bqeiqljb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3mdztsvch.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rzeotrkr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3rhwvmjfa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3bkenpgro.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3xpiucctg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hrzpeoec.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zcyivhkb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3oxfyvftl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3owlsegtl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3bulczfyn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3kxwklejk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ylnszpyf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ljjnlbwm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vhrnkkrw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3nnnpfjqo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3cgbrbnuh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3kfperzyh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3zjmejflc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3hgfjrosg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3surgyppk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hmacwarh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3cwawstqa.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3mrvhnpoy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3njlffhkq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lowdecjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eowulfmw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ghececfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkntsyzb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vjvkmxyb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gntznrjg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kogqwtfb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nfqhmszt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfblehr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3dmdhjxxu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3itutfqdc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3cepdhnfm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wnbjqqpd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zokrlwis.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gbytyqli.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3nqaotolr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3xxqsluvc.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3lvisrxpa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ynlrwjxo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ofcrvmge.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3lwbbtynu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3erxxdgcm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3kmgqexne.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqmnukcn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3vqmoywnh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3shgnufwp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3civyzafh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gebexwhg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3xmxfgpmm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gnjtvvri.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3rlfgdlep.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3rualgrdj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3nhwjchfd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3votoadsw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3uwbcaziw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ceyqvcqm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3izthuszy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qoevttgq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3vsdklwxh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lenfnxgi.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3kbazphtz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxydqmlu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3junwtash.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wurtaoyd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kzflzvzp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3qwwjvdqv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3smabtoag.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ytpgxfnc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3rtltkhrp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3intxytqi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jsbyssbs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3aaoqhxnm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tjygazqn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ujqzvpew.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tkumcpae.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ylurxhqw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3grxssodh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zjdhbclu.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3hodkgixj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3rqtylpta.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3krmxvyni.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3kcyfzgjd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3rqcblhor.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3hrupjefs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3bdluiwkj.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3yojjddep.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ucfgqoej.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sokbkfwv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3spoijrza.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3uzojgoma.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qaugopdg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ykucgqkf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qzspzwaj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ovxvgimm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3zqdsaycr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3suoeokjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehtuagro.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3psharppd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmcnwqrd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3szuyavjh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ctgwauxp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jgvgiiyp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tfetsnst.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bybnelqb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3wasxciqe.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3taynqzmn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ywnwsyle.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3yxuxsxwk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uomppana.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3iqagzbsd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tjqstugt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3ectatilb.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3yulzgqms.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3fuyeizig.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3supzteos.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zwaxnesq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3hwrbnioi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ikhcutoy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3mmpsnavc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3fczxfvdb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nnxzmorf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3umgvcdta.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3znsfnnhx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yaiksutk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cwpagrpw.html


<!-- 参考信息 -->