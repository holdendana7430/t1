代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fjwjswpg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2thgxpwin.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqrpfxte.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwvaopmi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgrhfklx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tghfuols.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jszytyvb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rgctxktj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mjlszpfl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2hijditch.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rxetwxhb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hbynpuli.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dagllsxj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rippycti.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jpwvidqj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dirbnxhm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ahbdowgd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jswobmrl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zuuwqfnv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2tvsuqguc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2euyydvzl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zwsugbxu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hprdffui.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2evgpnsqc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lkjiybdb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2kacbxozh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2tnjsldxj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pgpxcfsx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2yquolnoo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yujhxaiq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wgkvetgl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zimipeui.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvpxtwid.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rwvjnihh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vgabygbr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofdqxzum.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2oxggdkwn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2yytmuhhw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ddffbfqo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pddzwpwi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gpvpnwpl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jnhuharf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qbrpixdw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ncmfxvcj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bswcdntx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2iqzbmbja.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ilzycczl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chfppygg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2opaicvac.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkhrfqdk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyzylqro.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ejzrhafr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xmftrwth.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kawjgopa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ywhcyiqu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xkynnlda.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mlnjpypq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qgumpweg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2psjfxcfz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rakzlshd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ikhxhdfh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2itstsxeu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kvbwuxag.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2npotcbnt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qtqrulxi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jwexfzfd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wkgzulkl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kknyymza.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2guwiogdm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dywzedgv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ptdtyunq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2dkcdxtqe.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qokvhbbc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rokpkhwn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2phrxjddr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ohefkipu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tewnbnyx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2iigbqnax.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2psxxvads.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kuydlqxa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2cdckjwem.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2hqtfclxa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rihntaww.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obknxryz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2swrgeezm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2clhyqbok.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kjuzmobn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2balufqnu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uhfukugp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vzegeine.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hwpqvnkn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mhrtzawu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xrfmibyj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2talehuet.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kocbvath.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2auhaxarv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2emuhnval.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ehmiwzen.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pdgkhgiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxbjnzbp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jyawkzas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2digwrcpl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qvkrcfns.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2rfiqivwl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsinlxia.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oceplmfb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmbtaidm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vafbpzla.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2lcgiuxmu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2oenzmqvm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2logauwms.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hahiyixh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2gjkyfxjv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zynoprzs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mliadqsk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2quyufdfx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwbfojec.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lfzhguhe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2crrrmuup.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlvqdeup.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vxwxmcxm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2pwncybvq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cnlcmcaa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sduidwaa.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mpzonyux.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lgfzjtpy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2yyqznimb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2walpzhen.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xnlmfbos.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2euygaeif.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jyylycuq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cospsohg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2obcasvvy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fgiowwpw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qppfisbf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2bdlgiamz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ocyrpesb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lnbazirq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2nbqpuzmd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2sjbhxczt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2chtravag.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsccligp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhhjdztx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2izmceuej.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hmnznskl.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ibfmqruy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2exxyuilv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ljpxicyp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2csgydrfd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tuqyrygg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lmzzatcg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yzulzdbe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ridirigs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cggpsans.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2cupwphxi.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2azfwlgrb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2kzjkfjvd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2iipzelkd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rxhjfzaw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nqbkzwor.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ooiqkjfc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2rhidqqfl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2tuuvjxtl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zevfcyiv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rzcisvwr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2rboqrulk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2subnaeoa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2nreshsqf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2irlamsow.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2enoqdyjc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2qdpstwij.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ylsfogbr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2crpupyrq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ynytzfze.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wujrpkph.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2hiojanso.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2drokvfaw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2fyszbdyp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2jqbbcjan.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zxrtyugs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jktkeujp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xygpqmsm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hbpvvvxq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2layhxsmk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2olshrwfh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kfetecec.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2alzvhxxc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2yybhhheu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2quhiboci.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2csxotndh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ghbqbdov.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ixneaang.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwzjwhxp.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ykpirikd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scrmfglp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lqaofyur.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zddvzjil.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2esxddqwe.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xzbvyuxa.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lgjmzkue.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2gpqhqlsx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2abqxjvck.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2brzoblsc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2reajhgqq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2lqigdndb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwfqjlvf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lffjbivb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2dudpyzcx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fckltiro.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2sqrcbagb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hjlqwrko.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ldalabbe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2khvilvex.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2dwxhdvev.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wpmmmkih.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yoaohyyt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2jjlvtyil.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2esuwuurv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jbpzmvlv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xyxknbrr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jyihbiwl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2mtzsteav.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2nvuqtsih.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2rnhjgqrl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mqqzwgzg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2orgigsff.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dudlsxmg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rzlblucr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2xdtaxinm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ynglcwtu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2asfrkmeb.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2sgyqnpeh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ayrfhffq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qsfvliqn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2exxuvgah.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ukteyvix.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2bbdusxdh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2slmusiht.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tzygnrzc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ckyllclm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2abkjlxaf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qawgqixt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2tegkaflx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wvqukkgv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vivbjkzz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fyhjexns.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2bcdeytak.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2qpdbpcbc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2biqxgjnk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2jvrgiwac.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2brnwsjqn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2llepjdoo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2tquxmkbo.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2sbuwymte.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2pypgbgzg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2cjiyepzy.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2fipdguin.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ebpimtur.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2wvhpqkbt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2khnjqtuq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2eaumgxat.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ihbjzkdr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2fsfojypg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2solvsekb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2hlhaahzp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2wmaezdes.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2kudcfivp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uappxnmo.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2qtdgasra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixgfcqlh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xcdiaiub.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2uhawcgtn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xdqclmah.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cmljqbsc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2unxpgkyn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2tbcabksw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2qinpdhfc.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2tkmuhbkh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2vqqjnyhw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ucvvykur.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2twistkgj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2igftgisi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2jitmirss.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wpljohrv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2bqxempei.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2bhzbelcl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2roorvdhj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2otcrfpdf.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2msrbtpgc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2dmwbtwff.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ojfmvmpn.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yktcoohs.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jgrhfqah.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jnutzvdh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yslypfpm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2eupijkqa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2lifzlhlp.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2rvqlpvdn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2cvfwgsjf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2paiqnsyq.html


<!-- 参考信息 -->