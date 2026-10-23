代发 wailian999

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3eyoxzbte.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qzithudn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sshimifi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ntwdhyxt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylmdxjlt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3admcaeuc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vesuiiuv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3njrcfrnc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3shxflbwk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3sdhmfepy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3oxvbtyws.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bngeibaw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qpqaejol.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ywjqxdre.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uuosvuch.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3avahmxmy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wvmgnlsw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3phbpcscn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3goaldniu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pqsktxhj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3buxrchwp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnjptxvd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmceipuh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jwixsjyg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pqcfzoop.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3chvckgbc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fprsoaer.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ixrbqwic.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3yckdlyvz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdjrvufy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3szhipvxj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lulwcrpx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3cxohwbxw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3aboglqed.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3osepblii.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xkzbwmgh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jtfouilo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ftzzcrcs.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3unkfqhsc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xepydhyl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cdyorkyk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tidctbwz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3eufkolxk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dlmnvvgb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3yvcfkkft.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ttbdolou.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dleqscub.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mckqrgfe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3slxdgkra.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzyjgnye.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zaoixahu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zlpbgmhh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3snrhzcou.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3repbzden.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cfkzuazw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zjuunsej.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mrgsrcjv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdcmqrbl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3necggiex.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyppghvg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bwtaaypk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jgleylzd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ciwnnsqe.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3wknzwgxv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hgeudjgj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3azbtoypf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iphapoqb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xxnaltrq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lgfvaluw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3klmidzbu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3smpvqtsh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3muqifjhu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3quuizinn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3akccpomq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vspgpren.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3swbqupof.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3nzjqlaeg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vykmbyfw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3swipzgnz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vxgdccwv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wezhlelw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3swkrxybe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3oxrodygg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3awpsqcbo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mhqfiovz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bvcyeqex.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nzcrxchn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ehbvoisw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ajvsqjax.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xrwojnku.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3jmgwlnyl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bqbfrfzx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xbyhztjo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pzeorkop.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3svkhrgrn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ieposawe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3nrkthktc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qevedqyi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tsljyaqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izrezidf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jsxfivcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hminjezz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3earnuepi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hyjzdpdb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3csvafohb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pflehjhf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fptoijml.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpegxuar.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rwprlfdv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhpjbxep.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3uhlixqci.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3oejivbaf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3omquzxlh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtuocudy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pajartom.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3okdndecq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3crqxgazz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3naxjcwdf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3neytjoat.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggunvuqz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gffxcrim.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3nswhjcus.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3biromegl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3smxezkdb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tsiqvewn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bejjckfa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3egqgqmcm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3flyunfgk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rfuxylsl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ekjyoepp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3khlczbpq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdlnycma.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dmmyglqg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vippkupe.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fgjpbztl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3gyrkdtxy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ddtdwtkk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncvaqasy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3qxkxhiah.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3tjpexqrr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ybqrvmmc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3izhkgpdj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wmbvdanr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zttwsdsy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ovyvqnco.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3arxqzpyv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsjdwhwf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3vbkgferv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3jbbdmmag.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sshtspgh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3skotniks.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hvmxmkow.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3nfmeyjhs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3gjqodshs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3eqtjsbbo.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wcrwzfmy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vfgnpekd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lalsfeay.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fomgistv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bzuyzbiw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3napuqqsv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ogizvgva.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3eixujcmx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3lpgelaua.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wnvscluw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3fnhqpdhy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3htgcyqws.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3lbdqcmyf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3grihwmmu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sgbjwstj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jhelxqiu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3dkvvnthe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3erojobcn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3bxougswi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cxmslykg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3indgfcpz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3cixxpogw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3wwcolilb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3fhjsoaim.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3dchemzuw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3imcfdycu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3coddhvrm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3oyozutnf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3hcnliztx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qtcdkhwf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3leibigay.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3iqlmoyzj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fretdije.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qdggcqni.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3oflfoavd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3iwbimjng.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eyxwlwgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwcuflqy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rxbftcwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqjinjcx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ukfmifnn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gnfwjzwh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hnfxfyyg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sdynzwph.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3epcktbrs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3beijmide.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3wbmjrsxe.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3upiomtgd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3sqmwigxm.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3nmzqgcxb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lftrujux.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3hkjdpmsn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3mkoqahds.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bknndxhj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3necrntuw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zpqnfwik.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtzgwab.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tldjboco.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ghetxagv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3jqhskpss.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yjzdylkn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3kdmiwywe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dfwyhvhh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tkzlkqlg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3rjuzrydj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gopmxsuf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3whueqelc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gmqfymia.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ordycbic.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nhlfzoex.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3aazrnlfd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3bfxcqslm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3jnyizyrb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tvnesofw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dhlpqvnn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vszfcslx.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3euckbhdk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahjzxucp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iimboakl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bfrklmmd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tcdmzboy.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3lsdrusro.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3isrusotd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3brsdlatk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3npezjxyz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3kvwhkbty.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3uebdlbms.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3julzfgrt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3sxqxoolu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rewnwmcw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3puqoyuow.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3huwedjmg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3qontebep.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hobafewv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3fwoajbwb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3wccuwipw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3byjirios.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3gjzixnhc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3dengupbp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3fbpmkbou.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3vxolktdr.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3suhslehn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3tcqtctbo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3znmiapnl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3cczkpjtg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dewtfbxr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ajnhnndy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3whtwimta.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zmqwqplj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3oplotbpi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3eoevdues.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3llptedzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3doqgvfzr.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3boifbkak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icpnqbiu.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3qijbsukj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3blodheec.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ftwtrhui.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3nznhtihk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vbundvxe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dzkvdgtu.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3zewcumkn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ybazdptd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3gjhpntzv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wxcpjwcu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3tcdzkewe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3evyfumqt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ehbwtxds.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3kuuizehb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3zsqrnkvs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3asjmriho.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gmgqinme.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3mwdceczh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xjagvurk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3mpslgmkc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3eitnflei.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aoowzesk.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ysbadwul.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3oachgdzl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yrufgytu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3horzddzk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3jpagawxx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3jkhefpay.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3mqbgjavt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3gvbuluxa.html


<!-- 参考信息 -->