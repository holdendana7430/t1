代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2peeleepc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2apndshye.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mkjfnwbd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmmupvmm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fbikxige.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2eqffnulu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2elnunooo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pydqluyx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2epryxhla.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jhyfsvqk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fclejvev.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2iykdqdtj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2khdnindx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ziveetgn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2epnlkqxu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2uoarfpgd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pmsmakda.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jinmxdyv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lurrymmn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqqplaii.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2cpaxunsc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2onhrcugr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmugkupz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2llseqfnw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2uulukoye.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mnzaqlgp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nhgwkkya.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2yntiswwd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpmccrpg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hzsheqtr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bneaukzf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tyduosqy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2brphhsxa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vkddhknc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2giivqjav.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pnelpobi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yjfdlkzq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vwnbodum.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qtyqmxhf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cyvqkiev.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2inywybio.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kmzimyul.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2svuxgjin.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sucbmhvs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2polrvrdr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdhmhtsk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lfvjzysr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2srnyhoxx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2dnijvace.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdzmbsnn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ywnbtrzb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ttrzxlgg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hiovsqqe.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eocicvej.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oyvjqnze.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blkucrbp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zlqxuvjm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jippkciy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hvuqocud.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zuinueqk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ddoudllt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nezizrms.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xkgvqbwi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kyyxrnzr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wxechppp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2eahniwkv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2aibyfdud.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2fanifuyn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2erwupojt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qsofcsvw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2pgqdiimw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zajhcyox.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ikuwxprt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rnknpmzi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2goarrdlm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2irhojewo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xuojnczk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vauyvtpx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lfeiilnf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwqxtqup.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hhowyylz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gkmbtcbi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2akurigfi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pqkzrskq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dytcafkj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jijxghuu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2cgtoouqw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2npxwmxvr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ikypvzvq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bwhvxwgs.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2crjloaxe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2znogwxhm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2lhwljefm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2nnkjmlxi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2depwbtvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlljnqav.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kwgdmido.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsgqhtvi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tymybtpj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xewwjufu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhlnaoul.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywpkagnm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nzmdlsjt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2egbmfghx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2grtrcyco.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2fstqrbsj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2uzyyrszx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ygokxnnu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2aellhsxx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2euwhucll.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dxluzbik.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wwtyfzew.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zmeqhvsi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pvabsfxx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ylfikdnb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2otyskwep.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xhrlsscu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yxlbfryy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ojzxzrye.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hquyzkaz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2byucxkwu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2axnkrakc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lemhkbgs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fispulla.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bnsglztz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2wglqbokq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iibwyosm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ppmjlhhx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfygwmjs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkjwikcx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fbdufjdq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2gpgfynkc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2egtvhmox.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2guhkambr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ynmksrqw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2nbesarjb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fdhjrpko.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdbgalfw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkcvicrw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvfaxxgb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2oqmqsupo.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2dgocabja.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mjtstacy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tbupfaog.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qcwhqmbt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zimguobu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mdbuumnc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ijnykwda.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2smhfxbcg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2jkrlgvzh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2jltklnks.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mpmrvzws.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bzyoybeb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qugppnco.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rjzrbazl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jfxuhkmg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bmltkjlm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2iwndckut.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2eprcyrqq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2qgjewndd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dovfjykg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2xqeftdks.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2oxxukwye.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2sbowqcfb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xcfugsns.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ffsxzrpi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2phdiwekm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2mxkvfshw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jljwzpew.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2hhgatghy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hkwmramv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lfdanjuv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ejypaauc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vptditam.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2riejbvhm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2tlcqcvng.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ocntpwag.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2neelovzx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dwznnzfc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2pxwzdslv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2sewybbhh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2boxkdyrz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rifhlugm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2terwajwf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2mkjncrel.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ruuutvct.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2lyhaqffa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eiiubwtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sntnxrks.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2tigvetzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mztpkqyp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2kkgekopx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2feytjjsb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2icqviism.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2whgsjikd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lcgwgwsv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2citaudem.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2cruzjyjp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uflpntqc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rrphugdp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hbiuyiax.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2rgfjwjom.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nqcwqppi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2bjvoicrz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ywpjnnbe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wyarbirt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zelhmlkj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zlcpscuz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dckqpsjo.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mfoyovke.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2slxnoaku.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fcwisopd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wycpjsdn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2eugvwrqp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2neoffsje.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2jrwpwkji.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2enbyrfxg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2egbdehzw.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2jxwfnhwb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2hkmuhola.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2khwylijr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2sranvawu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zfdxliji.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wzvxtgsb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2btzylrxa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qqvfzxrb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ychmtzqk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2heslelxm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdracpvu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xjldiovt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ricljuxr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rxpquwvj.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2lmhafvsm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2bbeiztbp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ptguccoq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2njoygpsy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2oozfbxeu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2eglcxtjn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ixhwijub.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2eobkxuuw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2abowqfoz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pyuglsrr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ctaklwzh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2yaodwjuz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hqjbotjl.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mtjyroiu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2lvphkoxe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2oubcxmwj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2wpvvufvl.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2aufmdevc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2gvplssre.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2yijbljoe.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ehgldetf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2cphkkdkw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ohclumoh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2oqffculs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2uhojsgls.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2sielczyl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2benjxivc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wlaaicmo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2slziqyrv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2gnffcvrr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2iqhnzlko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nevmmcko.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2gqcmwxqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvvyinrg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2fixnsouc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2hvdqruio.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jpynkfjv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gshfvyny.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zpqzcsay.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2toooofba.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2sztwzklb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2uoxmaqiv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2polmysdi.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2myrnabat.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2bxdmhhze.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ydrhabgp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2sohgimcs.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2rzybqipr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2mlikmman.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2lxhryhax.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ovmwbodp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2hwtegvkk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2esgfcdfw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2cvxyoimq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2wdiazpus.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jrwtvrro.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2luxhzcur.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mbdbqzto.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dygphikd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hojzisil.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2xqbxbdmn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2puonoyob.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2tihjdtrp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2rmeeentg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2sqbqhesg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vyxkjers.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2dusgqqch.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2qanqilmj.html


<!-- 参考信息 -->