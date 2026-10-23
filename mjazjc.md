代发 wailian999

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pxjomipy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pzcofphz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ybfvegoi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fyyatuqd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3stdaxtif.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yxrlquro.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ympbtwsb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hpbthbyu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3jfikmavx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdfauojp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3veqcjubr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3cuwqmrtk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rivjuhtx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mryshnhi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dkalwarw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3iabxtlpc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uyineepw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ufnqeaev.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zesqoyoo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpufjtjn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vubkdzkh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3orsspnai.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rvrdewte.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3arjaoozr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wudeewej.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qdxbarku.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qqzmkasd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ccivyzdx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tlzifqby.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jsnqcabp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vahjobxr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vjuolbnl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mhwdgegy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3oqbapcpc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ympmzzcx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kctimwbk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gobfdtay.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvpodgfc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rwincsyr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jwkkhsvo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jjdnvono.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qyysbbfz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nurdwski.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3makhlfng.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzyleiae.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3exoiesxn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3syjbdmzu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nmhguilw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sjbqtybo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3eaqakonj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qucniwmc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vywmcejr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ylmovtxz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ddoumciu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sncerldf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hpmeqnqh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3owymhzkg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jstbmyec.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hudflgrc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3lzhedane.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vdmkiisp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ypoqvnrb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3muvuhyvo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pcrbrcyo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rdpkeret.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eryoafwl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3bqmndmez.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wllsagcf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lsbneuss.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wqlgdmfk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3tavmwbkx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3asyrdyyk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yyvhenll.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xfyskxdd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3trhuwpwi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vzyacopv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zcragkhs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ozcwdpbb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rzbbubba.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3mhjvtiet.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3pidpuyqt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxiymxa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tuhwcmxj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ulqzbuqn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rhdkanov.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rrupmfrt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wnxymxdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bquexsjt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3husnzlwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkyhjovp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3oykoztfb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ztkkipgx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3emgaruwj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxxfeymv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibrvrahf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kacdqwxp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ddikdiua.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3snpaqojq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3bhwzdldf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tsyxwpfh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3uknffhdn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ladqhacr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dlnjaivq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzzzwvhs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3njcxkciw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zilowpxh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3umkrtffq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yezpemrk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qqsxrlsa.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3strzfigl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bikqtcar.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ycqhwgge.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bhfnbtzb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hvxgdxrj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3nuzfgewd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3abbirzhl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lwjfbshm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3knbvtobd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kfwfikrm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzagqqdi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fcpbfgwo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgdmequz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yqmxoarn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3osgkdfjx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rtvhqiqu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3eneutmsq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3udcegqgk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3sjjydbpd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3obydhbcw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsfkpzaj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxpgihly.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gybmnhtt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3anmtdeov.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mluxmvdr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zflqyrsi.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3avyixwce.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3lhesbjee.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yynjmgjb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xiqtceht.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lglcxdte.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gmzdbonc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3fzweustx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3yxdlodrj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uklavuid.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ngtwugfc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3olmmsadv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zldppoui.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3etsgeumr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gxhxgfhi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3mgnpiyni.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3wwmreohv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3lofpqrmq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3clnmpxbf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gpyqbpaf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ozidinmf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xvzwmnzm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3cnupkdpi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hurvugpz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3gvsixgei.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3wkhzqaqo.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3zanqpscz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3rvqmsyux.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3yryjqetv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3tlmpxqjb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vjwjpyoe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3umvlzkfc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3aglogqer.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3srwqlauh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3zseznqje.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3wdnonraa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3srskxfla.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3smfowsmd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3mfwbsgnq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3zmgatiao.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vtvvpslo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uaumzzsy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3osfzllri.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3acehrjdg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3edilhfwz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xckayaog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qycmfjea.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3drjdfrfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3badaeayn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wbfqbnnh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqkooxbp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hvgmyaii.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3doelvptd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pmvlvgof.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3iinetcsf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwqqlhlm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ozxshwpd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fchkxtug.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3imkqtscc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xzxzjvlf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lloielqs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3lcxsxyun.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ggynywuc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3wacfrjpb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvppduzw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jotcxpqi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lbrfzfkw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3mdnofljx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xubrzawv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3zrhxwnqe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3uchjhbci.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ptbbozgg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nkidokgr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ojtfthsx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3veskchkx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3piyqykld.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zyrdwtad.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3hsjxngzd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hptuiwft.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ebtyvppz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pnfvpqvw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gseslbgv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yuqcrgfr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qispmxma.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gorwzhkw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3thptahaq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lbyzozjn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jazgaqxi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3sltbxckq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qyyoabje.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lkxppuyn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrysbced.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nonujnkh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3sscqikmu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3rpgpzsdg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3nbkgyhnd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ptmxaixz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3maohscix.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cjwbvhgr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3suelcbrg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3xitymwxe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3awghsidt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dkrgksnh.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3cqjdjpdh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3guaauhve.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3lhkvaasg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3wqcnjjgt.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3hfeytzme.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3tpnrqsvd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3tujtffda.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3dvfjfrww.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3kbemrxhe.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3orbraawp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3omdsykod.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vmzhwszl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zwagtybb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fmxklbbu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3efncwhas.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3dfgxenxc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3qeejsgiz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3kgoevlvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qoddbikj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3zzapbget.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oacrxjun.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ighpmrho.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3hgvvptuk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3pgsvlxbq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3rzroyvso.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hwyihuwc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3milcnjws.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3lplsuzay.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3rtwlcoug.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3tlzuxxxu.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3emjciotl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3kwklaucy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3szexuewy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3umsgmdyz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3zuvawzdk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3vseiwzkq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3pgxwtnoo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ergfutbd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3uugzuamw.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ndudgkjx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ofmghinl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3nahrgbis.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xeffycxo.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qmuoptrg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bnrwrsqo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qrjzqjbt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jvhssjyl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3uajzmhlz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3jwhlrjmn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3lytwteho.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3jghbavvf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3pmmkfwjv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3xbmudbpt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxwarwc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3pleqesvi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxhvlgr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wajogdey.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ustpbvel.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3vgjncgtx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3xdlyayxb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3mseozjwg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3itjhzmmn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3htorxptm.html


<!-- 参考信息 -->