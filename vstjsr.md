代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oespumdx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xdjkhukf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vfebofqp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2edcbphgn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gkswstst.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2contcfft.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2khrwjnul.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzleiltf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kskhsfrb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcmmrvnl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nifgrcef.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xfyfhhgc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2cgvbjorn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xvkdtwyn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hrflqazp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bnvsjpgi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2imyhblkd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rqmzyagt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wkprpqlt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2bkchxusp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2izctaiij.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hqidexfu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ngaqzams.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mxvwctno.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwwbmxsi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyrwtuew.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hipstsvj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2stugygob.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2otahnihu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zxvuhitd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjplqwel.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2aatbtcol.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2icsgthje.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlcevdrc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zpxfplee.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ckdhvcne.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjvzqsss.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xkmpceno.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2aglhlsfu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dyraktgw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hvoyboav.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bakuxrac.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tgcmkmpy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jkrkxyim.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hqgjluwh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pgpxbtty.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2fxlqaonh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mvsgvjgc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2jerrnuqz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wclaraea.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2stjkixpt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wxzddagq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2clccsrmz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2klyjnseo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvoqcfol.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gqryylmy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zytakhhq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2sqlkkbce.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jboztycp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2abyxawed.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bokrfbhg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cpslllfw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hodhvmhp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpfmduxi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vrajinfg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cthzpvxc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gvabhpzk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2duaszrvr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xsvybafd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2swkfiwmh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wkwdvsqj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2skzrvkhp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yegeyaxn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hdrdikgq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gunsacvr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zdfzysfy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qvowbgoe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kzntmikl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2eggrghft.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yoemhdeg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wdimrlsv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzvuimgn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hijafaqh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2uhfeianr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2aqymplim.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kicmnbes.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pqrygwfy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vbvpasms.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2jibilnya.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tpiknxgc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pbjlznnl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qgrojigg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hbpimwuv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ucmsghdz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2bwtzwmxg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2faejrxke.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jbmyjloy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kpoiaeht.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gbpxxwdz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pgzfqsab.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2byebaxng.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zlfvildf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cwxbzlng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvlwmtwp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kwhttjbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nulddxtg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dfmkrxhq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2dwdmivuj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qfhkhpab.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdctxcqf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2egfmkizm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2szeriszi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2txzhwfmb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jdczcwlh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqqnashd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tjchrhxs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2khnxvivy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2buyhlvqz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ismawfdo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2irpgiqsb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tizzatae.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rdjhlkgv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ozwbhcgp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtltmilo.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rmvjewmv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qizacfgz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hqkgearv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qibmgcyq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jqpfmpqr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pkhqztko.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mydnuafz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rflsigdt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nhvjldjl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2zekkzdex.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2kcnsgjrq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynicfnlh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndmgklde.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2erovawrs.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tdsmvwge.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2rmlqhpuu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2krehlyrw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkmuhqwz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xgojwpcl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cviuhfpf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jrqrbjqa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vjmrlrlh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wpvrgrfu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vucwwmdv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2givcrlgb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2eevwdjde.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2tytzxzaz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2owxpmsdv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2pmksbwek.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gtculvnn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bdbjubef.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ooruvzuj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2sdqoklui.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2lvzfuzez.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wpdbvepr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hlyuegyf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rlbkxvfk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2xijeantw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hkhviycu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dubbcmbh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hbatkgnf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xnmachbe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2pernqazi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2tvmeisaq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mhylairy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2inhopzfp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2belvyekj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2jhbrzolw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ijadsfyg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nslbmicw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dsirrhoa.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2faqevada.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2feagyhgr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2mhlbramz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2bbiepvrh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2dllmvoom.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qwofsnaw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2mmtdtgss.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qgwznpfe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2fqwyikhk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mpytldkk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2blpxtlem.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2wggjblyr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2fhlyxcyy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ruvxgzyr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ahpczqje.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cgemmcim.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2andpipcg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fzvvlsou.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2jwmqxoct.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2mtrtncpy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qihwgbru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lznnjoxs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xdogigrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htrpfpnp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jdlabcjk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2njkbhwmt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bfiuuavu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2woygiojm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gbohewye.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2zkofkhdj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2qrehvzeh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jdbcvhyu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tepcyeac.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kzmfggbx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmkqvshh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wopqfbcr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ppvyexin.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2bosnpmkm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2nkidopke.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2yrgzincn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mneflnes.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rscxvpwx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2wieqycbx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qamnflrk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hrmfcovs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2eivzbmul.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wpgeihjs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2axkmxhbp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xqshsakg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vnplukhb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2avaohith.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fcrzpqly.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2yflltyut.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dggecsur.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2twtfekho.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wpyntrli.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cjbvviih.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2kbzltfco.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ggubxwme.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2egukwiws.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2pqgeoswr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxxzmoev.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrpfzzkl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lmhzadcy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2inmpolhn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gthughxy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vllxkwck.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2sgrdwmpx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2gofdevvs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2npqegwnc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2tatwjpmf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2rqagxzji.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rbsfzmdj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xvvjsczl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pogmtzzy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2gbzpyokz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2mauzsbhb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qzqcqutm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2xeifomuk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2kewihgir.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ouwvmrmn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2oipwubkk.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2bqiembpg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2omextclf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgzsnji.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2qlrtamos.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2kdofqbyb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2odtajyht.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2lmbeqxbs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2yirnuvki.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pbuxzado.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tnqtiiyl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ywcofjeq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2zhvjmkzs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2onnsetlp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2nakswlqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfbwogkl.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2uyomtbav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnuffjss.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zrqxepdi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2uzssfumr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rbkliurz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2emxotegb.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ecudvdem.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2frljubxj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2uevvmlij.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2uxklvkks.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2oalybnqn.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2depkdokc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vafjvcja.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2epuknmtc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2lhobqbcp.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2uqbuafxy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ehdylqoa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2anjwlnms.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2yisinwog.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ppzbkmrr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2fpqyzumx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2gfozzjqu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2dtyqeatg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cusvpjmr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2favmvolp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vmbwimsh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sggoxcpz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rzxzahbf.html


<!-- 参考信息 -->