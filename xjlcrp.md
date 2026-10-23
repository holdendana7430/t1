代发 wailian999

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mdckecsr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mjvwuonr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3alzdiwjb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cihwqehs.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tjoqzwwj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ebykwant.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xhetxikq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wtgtsnky.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3khxeyvow.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wqcgubph.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3founuuah.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptuqlkmq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3guqvduvb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3heaqawef.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzlhrpkk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3aeybjclo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pgaegjhp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbglobuy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cstkvfor.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3maplokwt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xwdzutle.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bydxjzko.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhfweyst.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtlklgas.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3oywxvyor.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vzmwsxck.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sbbbazax.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hnzrquni.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yasqnzce.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3quitwplv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pomuypsb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uunrmedy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fpetrixw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vamrmrrw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3vkuwmgaa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiawfvut.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3npjaynyp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3boxbpsxi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qboduxux.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pejezpwj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gzvpglky.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvxmboze.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3khinyyxo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uxhpgqqq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioemcsqg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvxthqln.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttkzxsux.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtvxiien.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yokgwnbi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cmmhmqeo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qubbupqo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mgozsssx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3iwqiebxu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kyegudeo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tqhmykvk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3smpjpnec.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aptgpvtc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3puokknow.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ycbqjgjm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ooiuctir.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jhmyelht.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3pfcrcera.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3huqoatmq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3uktdzsrl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pbpxilnn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3apbycdbs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3iqrdopfd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qxlyzmyg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3igxmfuzy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bddtmhxf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lemmkpkr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3tdsqjhzo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mpdsurvm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jeluaggu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vmxfjenz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3gzavwxpa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3myuypdyd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fkwlicas.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bbogcmmb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mqlzjkzt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3uujzlksu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3aznwkzog.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kljnpmxr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3anfjucik.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3axohsasw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hjntvonf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cdzexqsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyybbuup.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dsjzqzbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfewelmo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ihhfasqf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ymurbdyv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3spqmykwg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cquyvbjx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbrotbor.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vieauxoq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vmtscdtj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vvjzbiop.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qplvkpdr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wmidypzh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3sgoaahkj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3grdolpcb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kizrkdam.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhhkaime.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gtezwuee.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3njqtncfm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3iyvywjbf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmxhioab.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jhvefmkr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3faznhyvd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dtveyemr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tnlwfomq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3smgapehf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ujpqbxmj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rdcdmjbq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3axkpoaip.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lcoccsku.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3nauevtjx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3nkmyxehp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3otynbbrn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3idrulrun.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3csowhkkq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnfmkxhg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3omqekliu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3usywvskh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pagdgayw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3cfrzjest.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gawlrgaa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ghxqvztm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azshlrcz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3niruppof.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efphktlo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ononwyqg.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zbfjawfn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otgtekeu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3uqeywhdy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3zxuoeyge.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3opgwcsut.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kepomnhx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xqejmlxu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xvgnucju.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3fnumlmss.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rcliqygq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3evtdezbk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3zpdfrqoe.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lfybjjic.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gmiykcee.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zmoqwgzt.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ynhtexcf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3alnzvumy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3zvhfujdo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gktbrsxs.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3enyfmhqv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3impbmqaa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3klmjoqbq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3dfamyyjg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wwmlcnfv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dredthdv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3padwffpe.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3qrluxcji.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3iibwyiab.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3khaccbxp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3nytoxklt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vxgxhqty.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3etaehstr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3jtkbuowp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3evtyesix.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dvordmjb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ozjkbhjz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3wuvpncne.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3folkemuf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3kidodhmy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3tgwwpllk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3urgzergv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bkfvvjym.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3glfkrkft.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3zmbennnr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3rzomlcih.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3izogkjex.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3plyceola.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbksqodw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3vflwmhvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wziumrpt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3intmzwqh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3occzjsqt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xkpejmpa.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xtiqdiml.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwzxzrsz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3bkjlzhip.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jutnyvww.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wxdrvtmp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zmibualq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gmjditys.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3peiyqenl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3suvxupuw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3jihrsszy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dzfvegza.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3unpsvhzt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpjrysbo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dvlturfh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wzqjpjrz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3qblotcrv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3boifcsdk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ibwdebgg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dechrsgp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3brbbigth.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3airagcrk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3olsvnskx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3skyuieyg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3syhpztys.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ktqreycd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kblehjag.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pezxzdqp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ncefblrr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3phakkqab.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bmcuwwmg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3mwvwkmvb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3geqxfnda.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3sjarnalu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3mityusru.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mzgwnoax.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sfdqtaow.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3imzktcjb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mxjljeup.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lgljzqec.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zodceszx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3frnnzfxo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3scizwoaq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3nsaqmwwn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3oceioyub.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3lfoisvbz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3vnalvjzw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3pyvabkpp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pwidjqlx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ovsrgjji.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3slficchn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3janbrtul.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ylhvpeie.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3wletvgke.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3egfixmwi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3xpqglyab.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3vgsmndti.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3bdpuvhlb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3jdgeguel.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3llzujnzi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ayiqfjbf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zmwvrhde.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3dmavtxhe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3cyvchwbf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jwfmujsv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hcazsfcg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ekeycwnr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3mzcywyhj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3vuspoxin.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mmytgdld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfphxfhz.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3vkrvlrhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdgndrwf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dchatbfj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3emiwpdgu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xsixojnv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kfdmmexo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ybbkvljg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3qwfivapg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3vexxwtcw.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3btqaydtw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3xcipxxji.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dkwmmpbt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mjrirsqh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3faqnyndy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3qpgipxoq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3zvscqegr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3zyfnqocw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3qepwaccl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ernifryj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ybwhzzvn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3vmxsteqm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3yyhhtvev.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3wwlpnuky.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dprnvusx.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3phvxvqvl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ghcdaosp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wauqixhu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wgqhwdsk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3jnnatvsf.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3pfgrsadr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3waivarwk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3hoymvapu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3glnzwlmq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lzulvofi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3yhuodzqn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3fasetzrf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3wtvkrias.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tpgokoos.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3zpfhsklg.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3fydrquov.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3puctwnio.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xdbwilni.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rjhyngad.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qytskxnd.html


<!-- 参考信息 -->