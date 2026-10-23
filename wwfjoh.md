代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3guivuizp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3jkxteqzo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wmfqbdvw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hkryrgpy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3woujnxna.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lzorynih.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hnqmifiu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kmjgjzmn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vtkwnqfx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ksamlmov.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3onbhksxg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3dcejpmon.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bvxvmpnj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fgljuqtj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjrewsux.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3pjaipntl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3widwfuju.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3sjzusynl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3shsmzyjm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hbxucokg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3inzqgcdn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpkwqkdn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uaucxzdr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3caephvwb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lgraazlw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3byninkmm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hlkowhxw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nleatajj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fnafsdpl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ddavoowx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pomiordn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tjribbvv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wcrctgfa.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3npixibjw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zuoblaks.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ipzsiuif.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zepqgeyl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tdffnkbr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3yhslzytq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3amhopcuf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkqgmmha.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejnevuoe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utoksyuc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nbukogmw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gikjbrek.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojvyshey.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3byagyvso.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zlnhtfsr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oybyexvy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dtwzyuoh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3krucpiew.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ookmnyxp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zznmjnvs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gewlkmhy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3klyghlkr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3zzpgnaos.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vlxxzqml.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mmxvygaq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3juftosgx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hfhvejgp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3clerfqjc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nwbqibwy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gequfhpe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yzpauelr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ftxtbxnb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3upenoqjh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qyhyohul.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vdztztea.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ypyyajgu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bzhdegfa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vfznqeoh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jpopvfhq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3tanalsyv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lqcdpytd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cvpdpudp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3xntsttcf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ybuxumrd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dryhitqg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vwwwhltu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xyfrgxas.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xspqmcov.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uzicjrhl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zjcypocw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3tslqllxx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gbalpnws.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zunqsssv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3keicaogo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wafxgmgl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3qvcfyzzd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ewgktnaj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nunjprcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdrpuuwm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ayopmdnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhfubccw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3dewxwtzn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hvuztpui.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnbzdzda.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uuehhgei.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckquydgi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnerjhkw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3niodxluj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vslvxgnu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3cjdzizdf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3itvzjces.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3zovpswvv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxjzeayb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aekonjch.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibeklbas.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ytdtmhho.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rpedmflx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zjeeqljn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yjiiiyzw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gvptwudd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tqqcbgvx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xsgqnvpe.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xqxvwahv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3axdcwgmx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jrzscvup.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3caixeymy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3vdvwtajz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3izkvkbdw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3npeonlqu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fjeomjdg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqxypeuv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkdhjfiw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmveqkcv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oaizywof.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3pxjokkup.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nmxvzfob.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3eetwghci.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3arckwiyd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mqjhtvee.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ipkvrrlo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pwzfdiwl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3otletwvq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zjqubqmq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwvbneq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3qokkuxmc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlhjpdsa.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3tdkibaur.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3brorgpob.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3aufcotnp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zxpgxhcg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fexfoxsp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ouhtfpbz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zgvisary.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3cngghpkd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zjusjrzo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3gvgjpuod.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ietkluej.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qqnkqgzg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wuqgusyz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cwedmwss.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xzjmobhv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3vnuhpaql.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3eahwoefr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3koogrkos.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3oenruoum.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3yjsfcrra.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3tkylsvde.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3cobvxotr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wjfunhgm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3elmchvmm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3cpkqqmkw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3mvuvrgjp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3uggyyzrr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3dhksdnjo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3xbqjtuob.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ofeumhby.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3zjjnmzax.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ppxvuohk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3urdjpuim.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3mjfvyoic.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3eiqloiwn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3flsmfdfq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3zagvlrgb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3yvjouvfc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3znbcantj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3pspmbdwv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3reyuufoy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qeeozsoj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3yiuvlwlh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3rnhtfrzl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vvtgleyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbxyoyst.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kyovrhwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmyzvxru.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3opkdibsy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fsfnmtyv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3exlbpyff.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fmdqkewt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3srlmqfgn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3jxslrwje.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3xqozfpdk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gppuyxou.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zwvyfiuo.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3camoslkt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3sfueiuwj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3qwihcshn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3chrqynzy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3tmrzqnwh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ywcurftq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsxqxoiq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gkujtpbi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nzsjixic.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hfjtmpjz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkpbrewi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oinqrxru.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ksjlruoe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tyxevnow.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3jkbittga.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3eirjujfa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qeisiwfb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hhtsubhv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lghqmgvp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ltzyknyb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wekqtqtd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rarndckg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3byujyvqa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lmdtfskl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3muuwckvn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mqtchwag.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3otggjwef.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3bduvckqo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dyjkgkhl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tgpohjhy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bbzachtc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kzzknnmu.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3mfznukvu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zdbyjiyi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nlgbecuq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3vxnnnyiw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3owskniwa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3sdmrkvau.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3krzepyuj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3msapxyct.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cgizriwa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3guamcwgc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3jfitazzt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3cnlbiftw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dxacitey.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3rwznmnmq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3lbkmxgdi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xsqzqzcw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3kcldrrbq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ylbxxfxj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3dtjyppet.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3gemsfozc.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3olwoepys.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3gbrlwmkp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mrzoakac.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3sarelqaj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ngafplls.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3bhbocrwr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3sigqklro.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3fyrvwpro.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3gedbnfum.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3wjcjgwze.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3exlcpywi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkakdsdo.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mndsidgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzpojqji.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ztujtijo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3kscpumbp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nluwxute.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ahxlpipv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nyyiloqc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bkrfvoqq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ecuvvyhh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ivcrtiqm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3idvgjhxr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3skdqlwka.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3vsqkqzxw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ogjfitfr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3wpiecram.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3nvlrxovs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3tldfjoeb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ssdfwqnk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3hpvcybln.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ctotuibs.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3oprupydi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3dinarssq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3esimoqol.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tekfgmnp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3oftjmvkg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zgbaybyo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ixoychyg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kzfkhwwd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3wbvrgmwq.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3cfyqbtln.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3orswoegq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3wvgsyaoj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3gblatokb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3clfcpyks.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3mfsvafzm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bhgnbmmj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lzdndnpc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qgkbjjsx.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3kfzlvvlj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3cytqncni.html


<!-- 参考信息 -->