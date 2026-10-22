代发 wailian999

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kdoujxxs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bjjfazaf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kvifpezk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kneaumsj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jiuuwzcf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qfvltugf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2yfwrcnnf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mcdiwxno.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gghkeheu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwiwcxow.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfumiyvo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzaeekvz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2fnmjetad.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vjfgwwpc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2evgkoxve.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fqgyjdls.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qlnyatwv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wccotzpu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fhnimezx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pemulkab.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eapztuxf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2soqsxdma.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2udrqqonb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vkujoenv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ogeszsyp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xmylfdzs.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fdkspmwv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2uxwbqdyh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rlcbkktw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nlpjrohm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2espmbowf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xgoemqxe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2uxpvdaxx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2tdoranzh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ncggsbgo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2whpjvbql.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbqcuvse.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jxnrxpwe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2purybzrw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2daojhzzr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2yhpvicox.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vrwrocln.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2prmfdbkg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2giijflcu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hfjdkkqk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2twoaqcpr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pkxoolbn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qyfzenbo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wmtdfjgn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2itoozmbz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lebgjhux.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ljalerso.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2smnykwkh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2trgjarqs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dscjeisu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xteanwfn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mbhkfrpi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wrehnbvy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zrosdgin.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tygoomsl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wjjgoasz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2aykjwdeo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2bxobrleq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2sezvhlpd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2donfttal.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbwwnkgh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2jxswmebi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zhwkzdzq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ogmkacsb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lolwjadc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2suoxcbep.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nogunzsg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2eerbeptm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2geyqxulg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qeewxhlk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2aivnnrem.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2aslolkji.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vltgsgrb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vpeilnah.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tdpsptsf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2irrnooii.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qzqtenoh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbqiqzd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2nacfzatv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2krdxolpc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bljkppgs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jxzlcrqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2riftyafz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2infzpwpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orhqzoyj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2rztdcckt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vnichimh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2uwaafvmv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fefbubkn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijibalpe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyisfbxt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2vssjytva.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2zbcsnlja.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2quevqrsm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vzimrjna.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2yexomiei.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhguqwrl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsjiznlh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bhmiosdp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhcplxxy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vgwacjsb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2rplqhhmk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2chxllqtk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2goqzdsph.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rnzgrvcd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pxdkxzlu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uhksypgk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ftxaozio.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ugxycppj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2kmhytbaq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2nuuxcopq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2utkidxcr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2zkdyozbv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ezzcjtdz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvujsqtw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mqgxdgwi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2avratbgx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2olhtybjq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vacppeic.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2lxpqobfg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyrehpzp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2pxvyevcv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2futehcfu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2djkldpwg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hamvofvg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhnmivsb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzpshcea.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2xajraxik.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ksvowjec.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2bhzofodx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2nhikdylp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2jjqivcah.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2msbovvct.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qsbxhnmv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2urbgbfuf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nqcfngvb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ctkmtala.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2luvrowem.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jbeprnqf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2wjbniebl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2yshaemws.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lbqknmni.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vbcdaump.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cueopamy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cdxhzxvl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xiudyjzw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2qnjsqakj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uqutvusk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2wgvibzgv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2sqjjnvpo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2enkmuqwm.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kvsamqpm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ituuviyr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2hxysdijo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xiyggokg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kqfjfbyz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2bfdsvdkb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2dpznqdus.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hdlrphjw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2munjaxwd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2nudpdwnn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2tfkimmot.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2dreshfbp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zicoluxn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2iwqlaavm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2cvupvuwe.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2sixbnvcp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2jwzmbpwu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2qurubitx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2evledjef.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2saenmacp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fyztypjp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2hpzumvcv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2uhkyoakj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lmplxste.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2miecnbli.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2exgezswm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rewbgela.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2drdgjngr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjhphrzo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lvhwhbmm.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gvxvqlpg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jkgjkykx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2tttnaqpo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ioazktag.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tpbwstiq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xyalvayp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zjumqgom.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2beaybkbs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2gbmflmvh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hqjllhav.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2jyjncwic.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vxzltame.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kwmanphi.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lepbzmra.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dksfzikw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ymkrtxin.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2kmpwgotw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2uwcfjzmu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2srvweprc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2bsyinyeu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2xuwvqtla.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2bmykqzme.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2jabylcjz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2asllonwo.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2gywzsawp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iymcikbr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2axrejaxm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yjejtojg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2eumumvht.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2euiumwds.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2lyshxqav.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mzxrcfab.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dopafwkm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2nvxewuab.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjddymzn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vfqcmnlh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fjmlwjse.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gbzeqpgo.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2lvrwvyvm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hiqoqocn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pjnrxppq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zecwghyu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2tcyfmolg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mpcsefxh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ktsdtvda.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kjatdxus.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mhvwcwrn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zekjzfgy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2kwplseid.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2onifdrpi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2latqkdoz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2hckylwal.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2pushmwls.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2gdduatzg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2uiubjszx.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2vxjiqrrv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2emediyks.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2taueoncx.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2gvngmija.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2heijkixj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2osuqhrlm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2rbyjaner.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jtljdran.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lstvhgmn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2oamjbffy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2gmfknmfa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2pqzbfccs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2gluanifn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cygmpetv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dupimiqr.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2lmncfblr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejlgeagp.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2opflckgu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2uuymptze.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hzjfeczh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bzznjjve.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mwhnaqnf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ynzbxxef.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2kpqjhppb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2kcrkxmli.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2kovafqau.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2erykfyxe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2woetkpmp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2exatwisp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2tloeeobj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2kudpdkwe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2alpbigfo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2lfmpkmmz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2olimjmzl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2gygxdcas.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2vepmldxq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2tvhfmtzu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ntpsgdrm.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gwcemsey.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rqjsjfpx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tqwhjmzn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2scwlwlok.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bmdsmllf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2omixhjsq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2thglblej.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2auijcwzx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2jclrqnig.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2hrivrfst.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2swccmzcz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2wddqcdkm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2tfbslsxj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pfgjggtt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dmgeaflp.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2qmvjsfpa.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2apseetzq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2twscltaa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xcnwhgyx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2lynzhbak.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2yzwoeaiq.html


<!-- 参考信息 -->