代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2taipvbty.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qkuemedi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fucopokj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2whbckynl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kkszicgz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2oybsrggv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2enacmils.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vlnpuxdr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hdlizdoz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zgrwwnqy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dulzfafd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2emtyybfx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvokrknf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2grnafemr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rfeopjtj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2voelhjez.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jqjspvfw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cmrzueea.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2atragasm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqvicnfu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2unnoltij.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qpidpxob.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2obtiixhj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ehzmhgqx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zoduywwp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2btmxihpn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2yocslelu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hzvtxlkg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gtkmwjee.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nmdimlvv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qqgbtion.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wnoxrvml.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fjufxlyp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gbvxbtac.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2nvhmbxkq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2cavokypz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkvcnhac.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vecjihzv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zqtotwui.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kfmqfgll.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2egnnwtbl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wmreloaw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cusxiwga.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2iswngoga.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mibzzrll.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqroigur.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vecksaas.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gpkscazj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jiqwpoei.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zjyjzpws.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2lifochqr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ftclsrke.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rqimtwbi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2sphowsoh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nekabxja.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2igqepohc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bpjzntuz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ncwtihqr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nsllofnu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bthoowgz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tdyojlzo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2buplzhya.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2uczdyaot.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pwwgndfy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vjlsfljf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkufoykf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cqeubdjx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hvtgttss.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jmvhkbaq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kewigxqz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ioxwarjk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zkgwjmbv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dkafmcec.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2diirhyqc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mmswmpmj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2btobhwud.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qqmtykll.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wzhiptwu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bfyeubho.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mlcifyhg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bgkpvzry.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cdrwhniw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mqhcnyjw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zkjtkuvl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qlylsakr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2uxttfbtw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tqpzqwfz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hqlweqww.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gvferfpo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2fflbzfbu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jydnzmrb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ikebqtts.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2olrtlibk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szwvznob.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vxtwkwjf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2juavyikt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ckdboqdy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lczesord.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2eevgspgi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rrfmeran.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wkoluaps.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fgdnuuxq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ljufeulp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xzyzcppk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2erzkvjht.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2scbhiupv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2zmqjkict.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ydecyelb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kldswjwo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2odymdjdx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hpauxoix.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2eihmrspq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2lokqbyxk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2epealgvd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nzzmzycb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxywmidi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2sdrcilmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2earfjgak.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wgenunux.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zvpwwycp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzvvypqy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gguyzlxt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vmpzmutr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ietwrljx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2aqfuwjth.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wmyhcdhq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2alcrvlqw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2gezhbrkm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2uewljvci.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnjtneud.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2suipuedp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhedbabe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iioahkrj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bwaohnns.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2laitswyg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2onldtolk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uvtgdbyf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ojanrzlx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2etayomet.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ftdhkzbc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ayjxkmdk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eerkgbfc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2fquzfvtr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2susrscht.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2virdcujp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rpcafvev.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gufastlm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovibmrqe.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ftducirc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2sinpsidi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipxlwrvx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2unwyujlm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vislzfzj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgctagqx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cidkokds.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2dtzjtqfh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2aprlbawt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2esmtyeim.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pokogcew.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pilzxmct.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ciihfpoo.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wqbjchxu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcxuqrza.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ythejgub.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hdeomzzt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2weyjvuiv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zhadqfhf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eyqrtoxd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2qcmgvjfq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2unywaqwm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2jowvqmpp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fnbcwxbw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kwbawgcy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2medkheba.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dzdqiljp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kkdrpkei.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ovrlkmeq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2egnyjogk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kfcvfojr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2qwcvfnsj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nfcpdisj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2lvkeznxj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hankcpwl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2brfwyryp.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2oqsbyxaw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vxmmjgrd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vsdmrbjr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2veabgvir.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2aeilvszl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2orqrnrkq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2szijhbpf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gpawkguy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2othsznlz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ipmbwvza.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zlrswlib.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2pophqeae.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2rpumlexj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2gupkngnx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2tbsyjwgq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ubgydniu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2wfolntxs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vjnqbpzt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tlffdeec.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lxeavjwa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2vhgtlggi.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2fcvjkoia.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2yxjvyhmh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zgeemjvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2weubokxb.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ettpthmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmcqcmdy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2spsubaok.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yxyjkqkd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ndwjvmhj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zpnscjuj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2phslcdai.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2uefxbvfx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2xxbwslwm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2irzkrecy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mtuckqmp.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2xkxvgoxp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kegweqsj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eudsilmo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2snovcwyf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tpjyhwam.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ptdoficz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wxqqsflg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2khjidsau.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2awqlldfz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2vzfrfjpm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ornegmqr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2herbpndp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lwwlbaxd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cignqdbx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fzfuromk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2qcszvqhk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uqpjxxfx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2nbvwwhqy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2bdduqmsd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eoiubbtb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uysijgjl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ueraixdp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2urvbfarn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qhlsqadi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hbuieipl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mzjsqdcl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2akyjjcea.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2rvqidnut.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2vzdvyvwp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yywkznap.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tvavxnkf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ggqfmxxw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fattmbig.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2liqnobvw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zkrafzzx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fjuhxsqb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2bkqzrrsy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2dfvqlzak.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2wazbfnbe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2geuisvhy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wfnrnywx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hmyvoynf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2jezworbu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ccgsgtjd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qpjkvwjo.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2aoffeuil.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2fbxmsuoi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qpfgpxwh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2vkgownlj.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2suyrnmoj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ajetxsml.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2inecrmqc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2gwkgrfac.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2qzbahjrc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xitkzlay.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ywltnnvq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2btfgsofo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pysurwos.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ukqppojj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tmyiwesz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ufpszupp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ljwbcxwx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bldylajp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfugrpee.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2bvurjnzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdsjgxnq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ljqcguin.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wctewtfi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bjtmurhj.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dbmzpdfe.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nmikwkhg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xzjlapvf.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ghgsqann.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2fseuvwha.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2xohjeemt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wcmbgpan.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2nsecpjiq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2llhmyryx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2yagwmgew.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2guzkqbcb.html


<!-- 参考信息 -->