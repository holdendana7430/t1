代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2lviyskru.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xuojypan.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpateaka.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2achvnpjp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2onhpvawe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rexxgovd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vepsjnes.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2nqaxvqhm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fmbeymtk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pxrfzzqc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2lnxtkvfj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ewfsgrjw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2clhcetto.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ddfwoahh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hwsoidfk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tfzwnsxp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rgpavpkg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2vhtodzfy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qkyfvrye.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uxwhgjci.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqwnczpo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2niuohhbb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsmqjrfj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iygjmeup.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ovbefttt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2praeesya.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2paksohxq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zuyiyobr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2txnowmwn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwjfhjgo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2svjwpixx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2retlmcls.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwoceymx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2orlnkrqp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zezgmiax.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2srzmbuuu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2adsvpqyd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qfqnzdqk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nyfkmvfv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2disstvky.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2byrntidw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2jguzjceu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2igeowrrj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gcevgbhw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zfrlvuxi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qcquehyj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2awgasblw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpvvydqt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zylxmwft.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tqcafvug.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffobnqwj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dnyumvib.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2syoyspxb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yxwqoubp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hzyobqwd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fijhunxy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xuqimjcp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnxxodzo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vpzeybrf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wpouygpc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2otdzltjl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lypmmmma.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xvrcctih.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2sipceebn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2njoltbne.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cnoximei.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2egxgtutl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gzigbfwy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2udxitubg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vtkmvdfz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bixzagtg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pyihvkyp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kzeqwsxz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2btlaorme.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2klhscsha.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2dtvmgfuz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2buamvsqh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jychtwhq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2hrmdzslo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vqjccuym.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2sphcpinq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tskharrl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fyeebims.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yeymeomm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jtdmdeao.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zibicapx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2mfxqptwm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lopxwtoq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nhwiuyal.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cpuybuqh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2naqepwxo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zphvdwxi.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2yzvmpzqs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ivbyvmsk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hdqztpoc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2gbebbrnd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2spyguduc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xrawbvgm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gjszzwkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kghrkgpk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2aarhxwro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxceftxq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2etxvhkrx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qjxmzlec.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzwgwdsq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxerjqqb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mwfpdnao.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zglkxemq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vcaokhfr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2tojohmvc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ntltmgjp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gttlsldg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2vhmdypsc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jooxuqot.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mazvjikr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pbstftkx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2onhrdyyg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wpichqyk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ynljbbpm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mubgkcdv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vvddbuvv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2uxhajdlg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2urinwmmi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kmvdjbus.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qrpueatk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mlrbbizc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2exmsdjvm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jpyfjpak.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rzlybzek.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2asbflwwh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2efvuhtrr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2unwxdrmi.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqlyoqmr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoembfer.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kgvchqsg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2genpylzw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vbrjkqfc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2dtluzqsu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2zcyselyd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2crylzixv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2whqyymgq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2awxqksih.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dttpkhrb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2hzrijojd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xtguaqeu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lkxmggtb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mayxcqxh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vyrfnfhv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2fiziccez.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nzvmlqoo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qeibvewt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2cijuxywf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lnnohxfm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2lvtyolga.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2rjkmghiu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yzfoswip.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2lxynuubq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2nvirvlgg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gmbiozrl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dzvdxjzh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bvmxckmw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2lcpkqoqo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2wnlyczri.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2witdbkeg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xwwankmh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ghgpnpbg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ozhupjdk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2yiczlehj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2pvsblsja.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvcwlez.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2lhbddrut.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2airbufti.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2udemymlr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2aylihnnz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2fyjsfkjq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2nfimuylh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2qqvsznuo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wqccluni.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2fqqxrtqu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzyfrvuw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2byxwncyv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2qjjukemo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2buzthgzb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zvwzgyko.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2vbtkaqtp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2bnuptmnd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mtzynydp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mnkomdao.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ciqfuwdb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2oetorach.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2nuqvfsiz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mdgwavvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmgxewma.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2icqhksff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ashedqjs.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gfvzpbbu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajtnqvof.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2auclbelc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2phqvlrvq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qbfiekkp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2wabysrfp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxnrfhvq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gbsuvtxz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hdvbsvpi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2tdhjsaii.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwnfkxbj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ecaszhfq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vgckvonu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tymmlezy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2dpopewos.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2iwlffjsd.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nlgpcluw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cxqglije.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2vnitqqcp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cosoolhr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bavbwcmm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jkynuvfq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2wmdenbij.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fgpavune.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2nicoruoq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kaqvjrkn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2qhqhdwfr.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tyggrnxp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jjeyjpnd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2glrliscg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mcdtfwda.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2agtovzur.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ochouyjd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ylwfjuyr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2psfmlhpw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pkflypbr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2dcrnexzl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2neoznhsm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2trfnaebf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bxenetqr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2danadnrk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2vlteugpv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2okmvadws.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qvyhmtwz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2hdlxvotj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ecmidlng.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nwtkeger.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2rdpogapb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qfsubfbr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2egabfqks.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2imburaol.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2xclcntup.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2mzhqlbmy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ehjlyflv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2oxwbhceh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmymvlw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hgxetinz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2khgilygm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2liuwafnj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2sqxxzfrz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqjcqsz.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ugmmqmvg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2lgojroor.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2pwerxgwq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2qhsafcyf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nmjrbien.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2lseynqql.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2fyppnlbg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rtbvnxjz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2xmdcmycb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2tzzwuvoa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lvmdgyka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hghxxhsx.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2obfslmca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tutdibvt.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dlodyvgf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dfxerelt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mqrfvmnx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zbfepbus.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qhelrsdx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2uuzqchji.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2azssngya.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2rwqrmtvq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2ivffevrm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tftvyajj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2tbjhnnsx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gqprfpnz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2eisozrqw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wljijecd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2eoputrzg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2fnbntalm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ufgarisn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2hmspvozw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ocdgkhhd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2utjjtpyr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2slwhlvwj.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ehicbxjr.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iiswwiqa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2iyaunesn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nxhtnmwd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2orhkcpkp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ftujknbd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2irxpigpa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2txednemg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2jbqksriq.html


<!-- 参考信息 -->