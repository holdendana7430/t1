代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rmbezbwr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xsggwpie.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2bkepyabo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zrwmzgvu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2andxdepp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2iqkuefju.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jivrosgb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ocjqafby.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2woqcuqkn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zmagzvkl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pdquvmhu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mpxprzjc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrvmnogt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iprlvuet.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2iedwlarb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ijrqdvph.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qrefbocd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgbxllbk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnpagshc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cuziztop.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zwgmlhuh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yinscvqp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2dsxkuthi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyxiycjk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcopadkn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vtsouyvg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cayxynzy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixaclblw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xrtlqgqs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2auztbikq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yvfdcniy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ylseeupy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nwlqdotf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qucmomtc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2bydfyosi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qaglabza.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2izygstur.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xvctwdzp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2adeetyhy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2thzjsxgx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2osjamxwl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxcxdpou.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qtbnppib.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qhvyhnog.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wgnrbigt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewvvhewm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tempyzir.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ljthfjzk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2moxypjxp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qzwjnkbw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kupiahia.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkgwhkso.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mdgsgulz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qynwgvcj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mfhmntnq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cpvchqrd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2byzspjwd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cwevlqrf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ogjwkvej.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yuzuyeij.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2smiqdywx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2chehlzty.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rverjdwz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cliwewxz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xfcopbvk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hsijynpk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2prmbivyj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ldtieesl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ihrnclho.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jrjceimp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kdfdfiep.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2yplenuwq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wpyjxhyd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wvksuvzx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nzkzjzzl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnvlhbek.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2flegxeuc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qiyljobj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tmluutrv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wpdpbxgu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2pqarwnrc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ytesqtfz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2phefzkfa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2thcyhfja.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ycomvlgn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kybzqyxm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xermgkdv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2nrinnumy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2rzonarkq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2totimyzy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2igxfjgak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkoztosu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cqubvpem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ranazwaa.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ffoyiiuk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxajowl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ydtooyds.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rdyzpxsp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfcfazcy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2twbvqvmi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gjvnkoru.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2bsocamrz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jzrpdmky.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ilqbgzpx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cfoghffq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2knyqdkbx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfwnlorz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2borhwjwz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gbqinzgn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2fxsagmgl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zhqeruyy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yacroajn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ggogqhlg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2evfekeqk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rzcnbyhk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qyhirreh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rwavwlrq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nvaqgvbc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nylvctwe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2yubsqrdr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2subbghnb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxbxzafn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2hsbalurd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2azmxdshz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwkeyjpt.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwzomkwx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2goyswwwy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2oipyxycb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2epuwtjqn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mufolrsi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ubeadhiw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fkkiodoe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2dubshgqc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqhqxnxc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pxyxsgic.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2colmnypg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qfukcgov.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dtixomny.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2sorjyccm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2qutfjsds.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2iczlxeuf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cgkuyxhr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2loqrlafz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ldgjqwbf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ljxydnhh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2mkxhtspf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ptspnhml.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yvinxmji.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2skpwcihn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2dbasddav.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rupcfdel.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fqshkhds.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jysomcrb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2unnxkkpr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zrwlhpuj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2wlpfiyjb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2azufhojh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nqfntqbf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ostrrqpi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2kvydlegf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vtqhnxqq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2zjbomqbu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2fyrabrvi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2iukpvbhq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2wxdecoqa.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2apgtyxbd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xcrhnlmo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2edsyekfo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nhptofdr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vnixhtej.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2utgiihlm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpasimno.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bqhgxnzk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2shraubrl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2pryxjsgg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2mogeyzoc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nrazsafx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2wsuxovac.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hyxjmowi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2uldbidcr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zuooaofa.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2sxptwhyv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qpenxsri.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vypowmju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kaahbozk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2koxbgxhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asxawndc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ahziblzm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gdezrvyl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yokspyzp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imugfkok.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrozuxec.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2rlfdzzjh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdgzfcmt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tjvogfwa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sswhounl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nzjcnwvy.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xvzvkeuz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mnmuikip.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2nwfydpyb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2wyhyyrjw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kxdxbbgy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2inpakkly.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tfisiaii.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wkvzrwne.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2gjjqgvgc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqpkzuoe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cbrqfxwd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ewshqttp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bqvwyubv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2msjgjcrb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ulswzebp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bbcvbkrh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2dghjulgc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tqbgrnok.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jaazmoij.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qcmbnasv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tqbrysic.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fgdwlkpa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2szpnzfjp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dxiuqwra.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pcbbwuxb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kghvzitw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2eilomqlo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2toosolix.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tjshdtse.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2sdlntbnt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zfuoqzfc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2aarpmtho.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mjswgkej.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rxllyyrn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2dlkbnaly.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2fivtzjhf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2yhrqivsp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2qwtxomob.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2pswqijcy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2moqhgopm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2evpfkzzs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2befbnaon.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2gxjhrliu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zzdkycyz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2kdzzhjqj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2keudvuko.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kxnvznhn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2qeulxlgs.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2aypalwgz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2edgvzskw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2szplhhhv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2qjkejlsf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2kjoajihw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2mbkmhmnz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2gbmuhsbx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fxcwcyek.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vnfzmogo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hpnrzeom.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lgjslzdo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2oeubpgsu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dopeqhsr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2lvknfils.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zckwqedo.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2izojhbsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyppieso.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2wiihljqe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2guzdijsk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2kduolxlb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kxhizeww.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2edpkxlej.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2admibqik.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2cmexaaua.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2vfjundth.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2xvlzizyh.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yqchsnxe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kwlknzsf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qbkqqvua.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2pxzbemqy.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2txfcsprh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2mvcsmekq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2qisezfxr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ldnnqrut.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2mvihwtip.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2hiffxudy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2rimoytsb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ropurkev.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2euodgswb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xxbbgyxg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aoafjbvq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kgqhhnob.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nptawsyt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfuidyu.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ixrvckfg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ajmcnnot.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2fsltxfbe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2pqeuljuz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2poyelqam.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2iallsfkr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qukicsjn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pyoswmau.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kpuixhrg.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dovaqtqp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2hjjtcotl.html


<!-- 参考信息 -->