代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxogvdtg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2joyukvpp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ezmyhpap.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2abzxykin.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xwiqvaqq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ifrklxpz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2pvgryqxf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2warmqist.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mlffsvuu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aisvbqau.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2llivkobf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bcfekefd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mahuoafb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mmhpqjef.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2opjsuybj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ymdjpdnb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2mifohaak.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ctenmecr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzzwqlgr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2pvyxhxhg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mrtjgpim.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2aiyjnvcv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xzzdclop.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2opftwrjf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hpxrhckk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nxvxbwdj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ruibqddr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxfefqhr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2adldgweo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2tcljmqvb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2erxnfnsg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lbyzvzyp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2iqfzvmek.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2iaycdhpv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xztxbsmc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mzlzbvvy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kcuwpsnn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pdckcebx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qzlmeitd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qkcchxih.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nmlmjdmm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2criudsea.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2cxkunfcf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkrjfhnq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rhzyvlwl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhiqbxae.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcgxrvfj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dukdtzgr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2apaqxrqr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rmnyynti.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wvqxdrni.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zjnbqoef.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrfvbcjm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aqbxpybd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2euclphqn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zokmnceb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bfmpfpws.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqvfandu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uperdbnn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nsjaewnr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rcdwewaf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xlfdymle.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2efvuzvsu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rbyikxgf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pmppbien.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gpgmwbtu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2sryjyqoz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cmvejgyg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cyubcedr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2gfygsqsp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ndbhjtae.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yogwokke.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wbvxsizy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2osupuvsi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2dplmfiuy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ctioqoxr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2adutyuij.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pbqlksdm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wecjcmhl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwuohayu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bazqxwyo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rhtllcqw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yjkfuwda.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ffqbsdvr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jvkeozfi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hxbsimck.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bfbbmlbh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ieyiiflm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wtxroftt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2puowvtga.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kyiavcpy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2eghtzkpa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2fuwjkgnk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zswyauba.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hfepykpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ssynhclj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jryjupdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zweighjt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mygsvvbo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qptxuxvr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2crdmsjyf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jkmrsiwq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ucqkxrdz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mgmjcyqd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qedkrowm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2pyyudxir.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2njgyxick.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2dzgxlgfb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ojhdllyx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ubncfcbs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fspbsrtg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndlromut.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2czhzxpee.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2noyhqixc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kmuhnuus.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vixaszgs.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pajhfrwb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2utyszhwr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ljaamedb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rgzzvqtd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2crfzbuao.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2juwbvtxa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ytdbhizn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ogylxzfe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2smnuumbe.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2yjhhaiig.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2behwjaxy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hxcszcfy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2afaawtjz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2iqmizzss.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtodnrfu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rhbkziot.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfoifxhr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2isxavtfl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2wfgwwfqg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kwbqdbsr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2udxwwcep.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgvmyhef.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwtffokg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehznukya.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2exjooeuc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2sqtetvjr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvjaxnrl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2awttjnsw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2sibzixzm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cnkuhill.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nhyhowyp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qjdpafap.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2gnjwuxiv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2vqjaratu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qovorwrq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oadwearg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2uemesajc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2rsdblttl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rbmavetw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iyamvnfw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fznxwrwb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2tycktuwv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2iznxpoop.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ztdhqzrn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qvmlenme.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2frgurmnm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2hrefkkuj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wqxloqyu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2yfvaiwdd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2pwvnlkcc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rscasbcw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xmlwvbho.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2wxomniol.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ctxjgwmu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2pxvgxuud.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2owvqxghu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dahjcrlo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2myflxuhg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2fszhdfuy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2fahknwgf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2twuujakw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2uctmtunw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2cqaphnzd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2jtbxwhik.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rrplqldc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2przjwcfd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yrrdmoej.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mccldmce.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2renvymgw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2lwxxmxsj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2aksbeumq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2imafzgoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzuqgptz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2rqpdiuao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsszleax.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2doptwapg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dthenotf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2swdiulnd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmsucbkv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gsclaxrf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2fzadvorr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2apeumkmc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jmtdfhbm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wjlixleh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gfrerfnr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lsxdsbwt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2eahftwcx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2taepwnqn.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dzcsnlcj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2tukyygeq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mindwild.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kxtlttkq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pitbawaq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2vdsbkbgi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vudhinnp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pgmndtua.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2hjoveqez.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2axcwulky.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vzsyxmqf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2hgmrwhug.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ekuriudr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xwfhjngc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fuvqbzxw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2guvfymft.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmjtmejp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2awzmxbwn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ebvnrwak.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pwkauqgj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2jawtqctj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qpvlrfgh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dfhtvqss.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2lyjnyheh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2omixxpeo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pbrmlcnl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kuklowxx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2oumokvkc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2krrzbhxs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2nuoneatr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mlgqdhqn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2hgsaeeyu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2bfnewyov.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2dcpcykpw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2vujsyktx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2dhpeqgvm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kecsgyqe.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2txyrnlcj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2khzwgpld.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2pmyipfct.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tvvqyvpl.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2oqgbjkcv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2dvpzsshn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2bsrgzujr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2qbnryhmd.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2mzbbaohk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ufdjahsq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2bqwsoxyb.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2fvzsdvom.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2sajqukuy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2mgrabxqm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2rcygkbyg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ieqjqqvc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wwnnwqwz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zdiawxpi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ocdsaouh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2clozuaud.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2fsginerg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lksdkbxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyegyitd.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2qltjtile.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2legrqurd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2eastvzmv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzpuufm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mnxwltdn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gnrttcnp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ifcjwxgw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2uqocrghd.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2fsymqcvy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2xoaklrbp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2sacclzgf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wkaincvj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2lolumdhg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2sjkssrev.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2yqbggmbi.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2uagrfjsq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2zdbnzodm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2nnipzuha.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2psdlsqyk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2pomnyxcj.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2hlwhgibn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2xcgfgbby.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2tzfyeyjs.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2okugwijg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fpwjjugf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2orgwqbkl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2spkqtaux.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dxecikxn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2rarcknvm.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2jhsaerkc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mqrrpfaq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2obaaltvp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ohcubtrr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kxthpyzq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2mwqoyhrc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vhmkzbje.html


<!-- 参考信息 -->