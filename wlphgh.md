代发 wailian999

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tazhcija.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kfunvlgz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yookcpsl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rugpkras.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gbayblmt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ucinasdm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rguthtuh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2aiutukxh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2phccbaxz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymloechm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzwbzyxj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2znfdgjsz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fgbjgwjt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2imvnpqed.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mirtmrem.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2miasdeqm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cqnnyrov.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2oybmeqcp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ziztdhjp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xebadghf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aukakwpq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mzwndrla.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2slwvjeis.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2knzfqmxp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2kmhuwypt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tnuqntcf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hrfcawsz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xjttnivr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2boaklphg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dsamggto.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ozatiiex.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wvxtzqgj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2txxihpyw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2tyvrzlbn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ocbjulqw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bkwdviaw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2firqmsso.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bytiguib.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ektxuuyc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gcrbtsfj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2guotcsgg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qikeqbkp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dieixelk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jquzsyec.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2korehqez.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vczuvzne.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gxgteksk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqtfcear.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aeqxmbaa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uaqmyuzr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eirflgte.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xeawuwwz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mexuulgc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dxcbeplk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zwmhqbzv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pnimldth.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jdnentjg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2oahjtjmo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lffapoza.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gppdqyrf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2blgotxyj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2cjuvsfhh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ctnpzeir.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2whdoobmm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2layqojcl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2kmcwadze.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kdxidwlm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2pvllpzjm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bhuhirso.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uwmoahde.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mwyhhzio.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuafwtio.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mnvmdvpv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zeeourrl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2goqofuzj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pggogwmt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2oimwqott.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bxntiqko.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2iabyqfjo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2cdahyxyw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vgzlbzba.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cafvndkz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rralclcr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2vrggbqnt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wxnibfhi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2wpygllhf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bffvcasc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aowkurzy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2iohszejk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqeebysu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2egxreljr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gonijpta.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wkzsmlfm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2aiejgwks.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tquhclou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zekghuiv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2blfdkcrv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2irizvmwd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2obvjmcwg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fnoanbtf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2bjidjzre.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtmhtttp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdpgmezn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjcztotg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2extquwxs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2buqqdtpa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2atdyfpdy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2itvdqsfa.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lxnhqfcb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dyauyvfl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2epvrgwhj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hmnmrarh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zyzfoegz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kjtxciep.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2befojlde.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rgbexggw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yjenvbkq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2bcntjzfl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2dzsdgrii.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpgbzlpy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mewjxtqw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cuoantyq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2orhrssuo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2niuxfzrl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vnwlgbvp.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qqvjsttj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ilrzetgt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2znukcpzn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pwiosopo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmndzkna.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vgrlebbl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mogxknzi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lotocncn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2yzofazux.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2hrjpzwyv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2lkfvxzgd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2grdklbed.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xdagsvch.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zorlwxwv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kcdjksof.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2cculcjnf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2uryyixdd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2cjaogyuw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pkauuwbq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2skdfhiuj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2abfiogcf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tmsgihcg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tpxtqurb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bbqaanit.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bmdsiazh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ewnwpuox.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2pkjekwmx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2edwujtin.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2szlvwpas.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2gtihugal.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2pwomkchr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2wndtkflv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ohnpfzjz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2eolkdhet.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2dghntybc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2vrceyxbv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zkjunmjp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2qmrzmakx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2eoyiqyho.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xdjesefs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2arplcijr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2whjrmesz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzmbnwdm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qrzmzoqj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2immccqyo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zmpcilbh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ksxxqxab.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ujxkvdcw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2fahmvuqa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ahrckvhh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fphnlqmn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2agrwjeno.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dtgxqlef.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2xslcbfrq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hwgzamig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ousmndsr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ojfvjpvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2raecjlaf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lohcemso.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fosatauv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wcxsrmhf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gtwumfxd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sjkfmzik.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2nuotythz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2cedepazf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hjzuvvmm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2unejyhor.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uhdrinpj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2feaszxce.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2elwqcbjw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ppawdypq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2hckkodkq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2brviyvgu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mbezbnki.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qdsuupsi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yksiurxv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2rdalaxeg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2olllhubm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hvvtwpzh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2zwwujmzq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cyauvgom.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2vtdsixhn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2mperrjsb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2snpnqmda.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xzkpgomc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2onvrnhxb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jgnawdql.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pomdswbu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vczgitvn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sqdrvauw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2loeqlduc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mynwajmn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2nzicecfm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wiavsigr.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hkesddpl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcllmfxb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qajnfeuc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mjdmfyre.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mgtuxrcw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2syflzukc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pudhplqy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gfsufzci.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ptlyjtzs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2cntmyhum.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uygmxcgv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2dxvwutxk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2cjckcxhn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2cagevijg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2axwrhlsi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2luzqmvys.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2pbmxceue.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hivcuonk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2hduastxm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2bxiudawl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2yhlzlsqf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2xmkjbkui.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2djoibzbv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2juxejmpq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2kykylrkq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2pxoeegsn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2yzyaixut.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2qhnyuwhl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2rbtferop.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xpdqndyd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mvbtveng.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qlkwitdm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rgbhjhza.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2nzggzlne.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2axmurpoo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uzwgdgqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvmaaybw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ijiefblr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2schrjpcy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2sjkrfloj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ojoprhxh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tfdxogiq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wiqkqzex.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2odirzmqq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pnjnibvt.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2cdyytojj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2xwvndxbk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2yuwegpms.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xjggbwny.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2lyjntptb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2knwuupam.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2odkekvpp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wcpntmdy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xjxvyfel.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ccfewucd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2wfzwbjzm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2xtyjqmqj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2qhapfskj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2rqpvmbdy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2nufndlgd.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2krbwukat.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lhwhwxza.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2iqmfhjjd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pgfyafng.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tptarmxx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ckvjvlkg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2swsroogm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hnsbnugx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2cgnkyhyb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgfayfv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2zyieqlsf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bqbsbqbx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2smqkmcyd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2wryzrjqu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2oqcbtxfr.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2gknuzaja.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2mmwyivyo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ynjbmaey.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2uqfkfhjz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2csuxdoqu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jwjdqcvk.html


<!-- 参考信息 -->