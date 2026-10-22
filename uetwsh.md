代发 wailian999

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pztdvlfa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iudbmlcx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vdiesygs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkykexqv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zjkdpypi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wluhmcra.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2wmgjnglz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lqzhkpsr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zhsljctv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2welurslu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2omsenvcj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fmzdpnfx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dphaonce.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cjfkyqij.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zclpujqo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fvhkedss.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2waxuqpwr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2iycpzedp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vxiqzwgp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2fegavnoe.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2orxncjgq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wrvfnigf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jxpsznmz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aircskwj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rcdmjudl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2yyyxbsad.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xxnarqvj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icwguzqf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdlexkif.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qepxplnv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vdriepim.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rvtsjtcb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bhwrxxlq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tehuhope.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zeynzqxj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nskoxmsq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcqwjafm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mtdbexin.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ahikiioh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vsyicqga.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rfeksbnp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2czrururf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dshzjyew.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nbwauwgn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzwadzg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gxabbwha.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ucwnnfmt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2biaaqkyi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rebsfbdt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jgsfenuf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gjycjdkm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ramliwyc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2dbbfpwtm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kghxyagb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dubmomww.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nrlesvoc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tzywwphj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hoerwyea.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2uqejpezn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lkwnlvif.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2asppqnvi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fgsbmuqt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kojdwokg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozaujaif.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hkrgqfzh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gmyuiysb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dwjkricu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2anlhdsre.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zkxcmgoi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tepshnfw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mxjvokns.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2csxpcfhc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kjydwjig.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bouvmvyd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2myucgurh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2yfkkudks.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hbdpiygt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2sbskkhkw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2snnimsxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eatlezlf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2zafikcwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpbrqzzx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ukohwcrq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2egqaengt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2irgsecbg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmcpcvfc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kotcsjsx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2igjrxuid.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hmvgkhmf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lsrdhlbu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2blvboyeu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hulqabxe.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2dyyoicol.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqdvfacx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jgtplmcr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbrxkxpf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2frwssqau.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2vzsdubdc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2tencvuwr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hvztlbba.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nkjiwtnp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ocbasuxt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nihkxbpv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zjnmyfda.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tggppaok.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rwjhjjxt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nihcjgho.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2nybhsxab.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2knauealj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ojgytkmm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vcxhevsn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulinelvo.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfqqheot.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yiuqspha.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hxucumep.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ypxsqvub.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2wjjmgtpi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xwglodgr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2dblxvwer.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2fuuafbtn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hjfymfvo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2uijqzxcz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgnjqnly.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2palorfyx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2glwmeppb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lybqowmk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cncxctpv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2orersood.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ymhpthgy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bgvilvbr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2exgodead.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bbesvdvy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vioyyulk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2grvmwejp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2udbiufit.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2cbalqbuw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xjfazdfp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qrqrrhrg.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vagsjuoo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hwlnnuzz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2psuonrss.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ljsmzidf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2raacuutc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2delhlukz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mzdegwfi.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zrxmevuz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2jtjprsvq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2koxamjls.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2tdshjwga.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jztsgkhu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2aykdkgek.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2dzuajjdh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2olzxeorf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2yrowmuth.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2uoejgvgh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2alhsuhss.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2yjmaccir.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ndkwopdq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2perzmjri.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2hqdfvpuu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2idzjustw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ksagzaxr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qkwvotjo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2wqrtsjpf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xwwwmdtd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ngmngqmo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2novlnukr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cylggmfy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ayuhtlir.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2vfcgjayv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2pwsyxcjx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cdzwimvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otsbfriy.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kgihtjez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjxolizd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wkjkddqm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2izmlkatz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xswgpmzw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2myplvvlj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2orloydwl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2akuwshpf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udfbardl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2izjncigo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vudcgcjw.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2lscxikjq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnmkzgdf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lfbtjmem.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2oklqtglg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2sxhsfoig.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2uushtypq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2arfzsqds.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jxystrjs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bzafnxbr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2tqiipcrs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2skstbein.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mwkqegxc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hwgapvug.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2dqcfanul.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pwfbwucw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xdvhgwfk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2pivotivi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2dzcojeco.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2clwuccwk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2neduefor.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2suqelpqd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2muaxmwlp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hbvubalp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jrxsfkox.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2epfssnrw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2tdfawron.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2islbqtlh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2etncgxef.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2fwsewbjc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tjzanfzt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bhaswibe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2thujsxzn.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2ytjvqfxd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdylxbva.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2okxdlvst.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2oshboknm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2otzoyako.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ojhhdibz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ayyogpjq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fbbnmpac.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2byjemnsq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2exktddrz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2khdzzttd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2qyspwzmc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2irhfwjop.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2vqiyjrrr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2rigqhkzq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2qccbelpf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2rcetlyzf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2wsbivbag.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2nujqcqbt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2eozizdjr.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2kaftnlxg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2yqnotror.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2nclnlaio.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2eppcvpzb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2egsswouj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qcfafpzn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wgsdkrfh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2mtmasyzl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2rfkbglnl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2mklmbuuc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2iwciiphc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sluioexs.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2chggtiqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tphrkkfp.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2brzfooug.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2xhxiimoy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2nbbkwmam.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fbcxjotr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kgbqoooa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2dpjqrxig.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2xmbqlpbn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2rkzzczip.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2tvxplzww.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wcosdrec.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2akpnzxth.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2oivaguac.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2sdccszze.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2dpamlfoa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2avrntesk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2bhjauivt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kijcilsw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ovnjlvoo.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2tcrolewo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ilxgjqkx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2pospdzrb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xyvhzksn.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2msfioagu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tlgvhasx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sblctgvx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lkzlzatm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2uabwcaag.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2jnfkyqzc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yamidrsa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2gjikuufl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fjoagfph.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ynajswit.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2fosmrcjk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2pipwrkhn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xjamqtrn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cufmbdpb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2sdqxvikw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2tbzcgrfc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2iinnmxrm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ccrvuzts.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dfifgmqv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2kubteffe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2aqusyhcg.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2doavfyic.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tkazjdqj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2cvdxgdqn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2tloznybm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2sujmnihm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2xbkqdntz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2mzvfiaki.html


<!-- 参考信息 -->