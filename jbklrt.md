代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ugwuhjhi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2onkooemw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2cvcssaks.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2yrcxdzdr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2csmasmmg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bvablzbu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2flgoqjzt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2exzjqgfx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pcizrewv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oxkmjcpw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xrfbenkg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kziagstk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2osfauaxk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pocfxgws.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bzbzrldt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lugkcpab.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tawpzqma.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2usrssxyh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjzzdyob.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnmqmsal.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fuayqaxm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rabwblqv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2yskrknwd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hfwpuxeq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ufgzvyxz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2edlrxsjh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xwnnjgrg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mcgrwelg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ffmlwacb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pamolmme.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yawphddy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxzoutnj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zdxkizdd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tmyqirnz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rtfhfzxn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2izeybnjk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hmanjgvu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wuvkkumu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hwxefytt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lgdxgbph.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2smcdzlmz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bcgavmlw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rdabqfne.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbxuyyrg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhfvpffv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2acqpbupg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyspmqmo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wsbkzwwn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nrcininw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lcsmtxjo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2txlhwioe.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zwbjhoqd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnksfptv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbemjjtt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yylktjhu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjpherjl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2foxetpzc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wpdkqopx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qnxtkpuo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bxyayssl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dguxndmy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oboswobn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qhbthkus.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dfvfifgc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2izhfjccl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2imqsgkwr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lkfapisj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mrtezjxt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pozikbph.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ixfxqssx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ehlsdxlq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tcjkmqtu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qrzpxbjo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2lzcokymo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ivrvwqks.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jdehdiyu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kkkhwlzf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kigsaauc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2myhxoxfi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztawznhy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ukanvdqe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2etmyalvi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jbeuqpbq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yrcpxbyr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2tbxzplin.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2thmclkzi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lyppzygg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2pkmidqxe.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2yewkzcfc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rnkvqdiq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mvonwtyc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2oogrduji.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tqvjprmk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ubprzvwh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tftulihm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vghdktqy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2leslyrot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohfggezz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dqqmygyd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvozusr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyylxeup.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvgxcwqv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpjfmonn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2voakaddr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hgkjuliv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2taemlycx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2kgfppijs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2kjxzxltn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xoqjvblr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxafaiag.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cbqjfkob.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xdboehqj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gcsmoghn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2jagrathg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2okawvrqb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtzrucsi.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wvlilsks.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xgwcktyv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mygmrjwn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ipvkhvxl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dhvjaluq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jtbpxchx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2bwffwemh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2eaqeqlpb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fsageuih.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2glpyexgz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nzbqlaux.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vbefivpb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2piybtuox.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lrwjlgha.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2minfvsfp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ryosnphs.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2shgycrkl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2iequerdr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2huhkqypk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2utozgdda.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wdmzhmfi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhadgocp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfqttvva.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vhoeorre.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2atwbclrq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mwhqsskk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2nsmxntcc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2evhupubr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2iwgivqzn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jblqpzvc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2crtonjzs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pkpwrmec.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2porodual.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2cfvvoqdp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wbhkjwxc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2otiygtye.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gapfvfgd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2wndymylp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xhplojth.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mstpmkft.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fhfwqbbc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2owpofyuo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2zcowmzgi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2tfrdtsfh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fhykbrjr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2jxcjzrie.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2jzxjmveh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2qxrniwht.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2crmodzbh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jisgfgby.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ydvffcqc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2jwscpedh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2rudmmsek.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vmirisug.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bgtkqaaq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lyvcukui.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2vudixvov.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2atdupuhl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bcrldzvk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2wtivnzne.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sdkvyhrm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2auuckmno.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vztretrw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2suoilahw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2pgexahhm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2luezhfnz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ulicbtnk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2okttkqlu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2qoooscfe.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2twbajovv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2tpxlidwe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2spyuwvsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvaxtpxh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kekoddjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbqozzvy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2kfcrnzpz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lusqwugp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rphufbhj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dxfcabwn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2euompcpw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2fzlluaqu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2mlrdumdk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2scarsyrn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ojjqhekv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jmqnplpi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wigvzjrf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2kfoeaqhf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2fdfjehnv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2skjtibff.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2lvgyqgvf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlbxuthz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mairsoaj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uxwnoqfx.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2bphehhkm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjishvru.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2yjfutcfw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pogkzmer.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2tboxcesa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gqfltpbf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xivbvcha.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rbytbxvz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2lqlhssiv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2lkuarypy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nnsadyha.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hdfcozop.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hvbcpjno.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2wjshdoam.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gzyeagch.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2dzxnmgzw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ldtdmmyg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uarbwrfq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bwkdbuaj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2qaliygtf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qckeajmp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bncjqkxs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jvxjbicx.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2iqluflfj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2forgkfwt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jvyxtxes.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2tkpexrhx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2mpxwlyxt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jlvfhluq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2mlchqkjg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ubxeyvdv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2begecylw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ndtmslul.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2dqcbssfo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2zoxbuxyx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tknjyqbf.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2bcvugozo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2axzhfbzo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wbwltjbm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2yzwovjjt.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2pglvzrvf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2ilkksykv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2otwjmytr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2hkwpaopd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2szwymgnq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2fvlmyyho.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2lxvudzfb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qanyalow.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ghmgtzwu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qkmmmyyc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ipiadhtn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2fwujknmi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2csyvummg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2hkmlywgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtihdfbt.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2conjeikk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvchphod.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tqpszdtl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2dzkirria.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ddvxjotg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2usxsetse.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xoqmwfuf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2rypdegqr.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2wimqnydw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2jcbehulc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2uhhghunx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dvjendgg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2cwxvswol.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tukwouwa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2nseyaveh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2omkkegkn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2xqvolqqt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ohzpilwv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xzftkoys.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2lwvhbkna.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2fpfafixj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2kcijunjh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2cqlsesip.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jfctxbqp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nfwbstlo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hwlwwstk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hghfylwb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tihsujqu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2qvpnugmg.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2qsmokrfd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vjskeoqf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2wqlfckra.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2kdsdnwxt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2zrlivmwa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2dnfqalff.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ignpdzxg.html


<!-- 参考信息 -->