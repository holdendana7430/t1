代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wwzseanf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2dyvmfjbf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2okjcmzrp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mlydcqmd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2igzbjdgl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dqlrdvsm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qcnoihsv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2shkaazgt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mftoatid.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ihnvkicb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2epkpondp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bitdbglm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kajvqswr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kklmdvre.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kkgmwzqw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tsnlximb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ykjlxptc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2igegahdj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vcpezckg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2wdxhylgf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mrbzdmnh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mnptdnck.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2uuxvfpac.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjgdlbfb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2oxormozg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2thddgbit.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ljwjibhx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wigigmvc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2phbqbsiy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2faslnoue.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qylfzplh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2famndmax.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2znmdvdou.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cnrvtkkd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lwluccll.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gzmcqbqq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zgnejlnw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2natbsadx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2cyatrskp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qgtehgie.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjixrnjz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrixpdzj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yoifanxd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ohxzyzuw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mndajodc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxpdvsrz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zrndubfl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pxucnbau.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2guhexfro.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lbbipkmt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcyfazjt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaitibjw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nrydggco.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvlxwdzw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gmmlxeii.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vndzmfrk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zhbrgtfk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gfxiabvg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bsjllomr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dyftdtsm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ejnwmiek.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lzvvukmm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tbxrndbu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ycnillcb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2cekdxcxn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wfeyqotf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2akydudgw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2iiqdofpo.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qfcavsya.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vlqgywtl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mdusuchc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2huuwoxkm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2efsfvqtp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jnimfwtn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sjtqhqoi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxelwvmi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ikqlytej.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rxcnasue.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ytriucsy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wjlrtbxy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zeqkispo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xzdldhnv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2odbgizkc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nmlpuifv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bzpmljrd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zjqcrvlx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xeexupuq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gbatqedd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ztoelpnk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2skyaafyh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wkbmrars.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmxhchbx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2mdvahols.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccbxilqq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dgldzips.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jrfseerc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfutvhkh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jttferln.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dygaydfy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2eepqobvx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dkmmggzf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bozjiflm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2bdfaljju.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2utolkjeu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fgmsielg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sahnywzc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2haptxtsy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jqdbgpqo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nymoswoy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2itzksqvk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wowwugax.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wtunpdrq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dnycqeua.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2esrlvkjr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jruyvpez.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qziwgacg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2spzbigqj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fkzkrabk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2dfmmxccn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fdoevtog.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cuafusvx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2sbnkufze.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gaznqvhu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pytjuort.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kuwyphmj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhhymvhn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nsttkqvh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2initmsva.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qhfljlzt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2afwpkddp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2bjqkxevd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2kjnxrdnv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ryugpcek.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iycrtcit.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zkujtjxm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2uzinatdx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xqyfdfer.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2gbimqiey.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2kozshvms.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2lndmavoo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cdvneqow.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2aufnctlr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fpruugye.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2thpnwsoz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ofqpbwkm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2fcyvstwt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2rvvvsdlj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mkxzthdi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vklranes.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2kmdfnkeh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gjkdprta.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2excccrph.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cugegtbx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ivmojsxo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ealbtftn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xjuhlarc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pdywhswg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lvsqwkbk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2halbohzb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2cprsdagd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kqwpykde.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2fnqubdrf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hhboizrq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2hvvuswrs.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2myrzsixu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xoeoommu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wnoxmkil.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gqkejywb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rppjwpdg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2gscsfhjy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2kvmkozsl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2qclsfvnn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2msuopejw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2mcoapbsv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tjmwhzue.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2hfyjnswc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2rigbacvg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2pdznbhnv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bnsksfpe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mhbwpswl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2usitfbzw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2yjgoutkd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2wftarlaa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2crhuuodf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvntdlmr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fanquesy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rigvrjtc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bjdxkbdg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lydtvngx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uubwmlnt.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mugcfplb.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2diaccytn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2bjofcqug.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2mjeigumk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fmkplbmd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zfrfrfrs.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ygwclytt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tjcwzklc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2sfnrmrhc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2abdozhlx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dfeadelm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2mtgrywks.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2tfwcrqeb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nyvbrsys.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qiqtlobq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2vrxgzvqy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2dksqjnar.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2papwncbw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vjmjystg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2odvnjott.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2onytfhpy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2uhntgfmu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ynynwnlh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ngcpzshe.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2hdbaxnys.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2awkgdawl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xqtanijy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2niktckmd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vobnlqmn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bervmznx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qvfmvnbc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2fysotksr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2eunggwdb.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cekorqwj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ggrainbb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kugqcdqn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2evwngtmy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2juznvaig.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2bjvdfjpu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmmhgah.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2yxanzwuy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2jnphxgvh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2hheizjrb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jjnxspyo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2cmzkymkx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ugoerics.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zzggopyy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2svzzfoaw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2oerbcebc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2haasukfp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hwqxdgfo.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2odazahqr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2muabjglg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2eabxaspg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2hpftlzvp.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2uatzakqk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2ngxbxpld.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2qgqwqbme.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jrdmrkmx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ysnhumev.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sbqkhrvg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2xghyytpy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vkfuszch.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mfphgrnv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pzubysbh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tupbonyh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2whgdqcur.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2kmahnyjp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2osqlfaxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fodgbkpx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2spjwikuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmkqhrty.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fjjbnacl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2vzymmzya.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bvlkchqb.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gxaljzdi.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zwtokbbh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uqdctqjv.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2pmxjixrg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ibgjxtqz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2wspehwbq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qlepppzk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2glvivqxl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2nfucwmob.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2mpcmhljx.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2qqjbvqyt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2zjappcyn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2dnbghgqk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gouscqwx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2cyllmckh.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2fnuuofnw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2mmaimjcf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2gceculck.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jjioxdvj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jhkjlnuw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qtpwtwwi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fzpyonym.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2flhnjhhp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwunkym.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2mdxuphis.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2teziwjdm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2vemqzbsj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rapqelpc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ixcjkrzt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2qwoaxwzm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2zkwdxjui.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2sqvtizdw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2fgqrpbxr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dypvhcvm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2elxvhzub.html


<!-- 参考信息 -->