代发 wailian999

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2peudrybf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xyideate.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2goegjhzt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2oklwiouz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vzroutaf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2szjrsgqg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2aiinaecq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ekatfyjm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmkihmfe.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gmqkijnu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmhepodh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2wjrnjnrz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xdlbihat.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wqeqvpgy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rudwozjb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2tsawosyd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bcdwicsn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2iwevtrxp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2aawdplwp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2skbqojuv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2klzynsvk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nnxniyvw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2kjhlojcn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yzcndjkt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nmfwtedf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2yyuzvqzi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wguuhoek.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nljrfyvb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mniwqgef.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qmnpujuy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2fhtlwoqx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ttggybkd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wkmlgfjx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vfpyypae.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2aedchmsj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzyuiktr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scgedqpm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xberzydq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrsxvoqc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tflnzeul.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2upgggtnm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lximnuzo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vwvvzqjp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lzulkarz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dedzfzuh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ermbemqs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiljvxyq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2udixnywk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bgswiqxm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rgimmzuo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qcuigery.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dqgqntzy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2aahhuscn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qyhnlvjy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ltptvlof.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jnajmsmy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wwlzrqru.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2iloppomo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2esssusjl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dxssgdrw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hkirsvif.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2yztthstu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jfpeqzty.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2anzqijvp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2inctvdau.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzggucco.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2viwsphpp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2khstjdmn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2dwihxwmg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2szdcyfzp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tizlplpb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2knougeem.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2biqikdoy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2flpdvcgm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2yodtuvzg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bpwiijiy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vrqpvpqt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rnnhrprd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2gwmjttqk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dsoovzne.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2hskfvgsx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tdjfljqa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2efvbdrim.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2bbifwbxf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2lyumhgtp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2sqsopkvd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dblparnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfmmvrxi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xuatnxaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfpfbyhv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2fklkjuvf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ipnxiuox.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2skxmgssw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhaqsott.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mpucbbxb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2iwhxjioh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zcfnvawd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ebttdhac.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbkmusss.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ahozplzl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2bqibyygn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yutdtrpi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmnjpwdc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wxgmmyvy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpcvgwiu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2qwluvyny.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2roixyniq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zruffsdt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dfcylwuy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zsqkfyvb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cxfosyae.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rorcbrgw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2corjlizr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jgjqcomo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2fkyqudpo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xdsinmlz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pntzxkxw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rlwtpibc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pjjijgna.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jdniftlp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnvvbnxx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2krlwahrd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hfbgrcjc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2nosmhbgv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bgstvovn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2famecnmf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2poavqxli.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ojfoyqwh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ehpkqgct.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqubmwzh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2keerlhgk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldqnirag.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vkzpfblu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2hjeelcws.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xqnunuqn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2avmlxytr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lmabdqkn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cfqywskv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wwincivf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wmivoupb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2zjqkpvfl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hphlaima.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2pqqofpbd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cqjxxxui.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2bhakxozb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vnbvmhhi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2chcbpnqw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zyanxrxz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2teagndoz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2codkccix.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qhejzmjm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2qgnbtlqs.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cftvqhys.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2rvpnfwhq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2gyuokqex.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2tqyshyyq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vpqcozai.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uxxeocob.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ymzuxoqn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2gvwptbyh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2vqsihtie.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2prohregv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qytwsyge.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2eeaqnxoc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2eupuzkwg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2diwqkykx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2hyrjhiam.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbhgqltk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ukpgteah.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2dkptanoa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jqbxgtya.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2qutuufvb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2kfoklpit.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dfrgydrm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xoksstii.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2molisekp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2eqzwypcm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2twoxhqub.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2icxfdnlt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2trfldpot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eaffmpax.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2goedprzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hziusmhc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2kwlkcapj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iigpezwo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2puyajibm.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nwuihqcd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozzxxfcr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2vuxnvmos.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2iydaxrzo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qyflcczr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ruyupwtr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2edhkfywd.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ftmbzdtg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ttcasqnj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2lisnvuoy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2likutrqa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2xyfspnfu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qcfpxwxr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jaxrgzyc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2viqrtsjh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qkjkhqoq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ldhtwary.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lwekolgf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aatjvucd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2lcpvmzyw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ovttybzp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2vtmvresy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kgzcbqmm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2chmnrfbe.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ergurgrl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xdgvdxts.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ddesvvow.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nlbgbxjq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iomhmiws.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2smgnqito.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2uasizxuk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2migqjygg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yelfchuw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dshfzmyv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahomkrsb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hishnsxn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2soadvbbo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2edwclyxa.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2panfmpxc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dxtatjdc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jnyvdoqv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2nenyhspt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2qfavtopo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zwdribiv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zaizhnpj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2keysmzzw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2liywiqyi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vsoxsfly.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2rhstrbue.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2nnupayxj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ymiwhblg.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2urcmbstr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2rnunpvgf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vqcpjjhg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2qehhjkbn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2czrcdwfp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2cqcwvvwt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ffvogszr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2staxrkdh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2itafsicg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2mjlgvzev.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ejlnkdpv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2getjiknj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2khsxiglh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2cwqjsino.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ebunsume.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2siqjvfvn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dkhixnza.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2npgyqoem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkwmlgki.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2vuusnmxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtqfjvll.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2hqyqkswb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2tixhfjfo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jjclnjre.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zucfkxth.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bznhdpgv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2easejjen.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2mkvfgeup.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2qwhwbuqi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2uxyeavpu.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wzpoxveh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2aohypcxk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ichxgjsk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2epghhhlo.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2qaagyneg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2dpemifae.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2clnwtooz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2zthpbder.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2pnmaesbb.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2buifwalf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2kmmexvxw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ildrguje.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yezyhcrg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yovyetnm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sourbhfj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pzpxtdhe.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uiwgpccr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2tymkxzaz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2aculixxu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2lntgpmwy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2bcslxxnm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2dhycxrgd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2hcaflyrk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2rvfrrstf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2iucjlnrm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2iwvgfjdg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tdhqxcgx.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2tsmcxfhy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2znnksqai.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2xbmlorkc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2apxibbpm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rsvpamud.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lgmjmfpa.html


<!-- 参考信息 -->