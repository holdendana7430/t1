代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3avufclby.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ffokpapa.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ljekylch.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qzrsztfc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qafkdmwj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hmroqerw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sdxghyee.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3uqcmmzel.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bdsskyjm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3olsusder.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kyryaiyp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3nzfvseon.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wdjisdno.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zygnbiwe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3padqmfwp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3krjzvexm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ugpesojv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3gprfvyrs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3umdxyjmu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qqdsczfv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3agtaghdt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3iiznpbiv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jxllynmi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vqiggqtb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrhdpnnf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wcsodbla.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vwtsbwjp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3slvessxg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3foicspuq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3nzfrizzr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pggxvqmc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3itemmstz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cdjalvjk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qofahoih.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vspzzvfx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nahwdjpj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vurkleih.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rlsimipu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pfckkzxk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3echpjqpx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ymevwjbx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtxgcxxz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjimmpqc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zbzdvrcp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mnicaors.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qrjuhuff.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nuonzdmt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3opzamgot.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yahadjqh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kujqtllk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3axwzanbz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dazzkoea.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rrpuxxyi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dqwxmulw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ksusxpts.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3eiqfvrdh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3irfvpctz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uxwukchr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hhqbgklj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3czpldaxt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zlncwozg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3twzfuvmz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3tcukeanq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3iqzywdzh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rgpiuliu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tnuqnzza.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3dzalcizf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nycdshfh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dddoxbwa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txkwvvjh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxkhles.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wzpliivo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vgbdtasj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aztknpjg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xncrfmek.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvfxmhrq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pwgqnlsa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3earzkqtf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3moqtphve.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qovbvxqr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pbkfahoo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lbrolabf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3pzzjwzxb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xikeofkg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ahtzbcsb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3biphzqkw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gxbyixcq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hwdsvjul.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zovvmnkq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jxavzkvz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mmkmaabr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzhowuaj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3lfwfqmwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzagskja.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3bvykpqcf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3suplvqsp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fdxldwmp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3afvjyefe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrscgjfh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jldrciad.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3drstcxix.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3redraote.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3pjtwtyax.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ckepahfb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3lvxjjlyi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwkbmbvb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuzlmjip.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dyhazlus.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dccwjvhd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3eqrdxzmz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ofpfxmkz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cdwgioml.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ytbyxodl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qjznlbjo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bpbghyys.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ihcptwbr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ealkswtj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3axilalvp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3earszykb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3xvausgza.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zwtrajvu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ntjmtdyy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vbdhtemt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kojrnaop.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3amgtlanb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lcrdfqyb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gogwzmto.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3oaneykdj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zjylsgtk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3mppklthf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vmogelvl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hlpqbwtg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tmiujbaz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3suohllwz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3lyrvsddq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqmwzixp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3xjyeklat.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3vlchehaq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3feevqacl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3iirjlqcw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3htcigmal.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gfuknakj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3adzodjwa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3prhcxqhk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3jsxdohxt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3iewtetqe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ithjyurg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3njppnqnd.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3xeirmqpu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3iwgupxnv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rafpzsbc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xvekdohj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ltexnhcb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3nuozzwiq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3gfleaafl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nsvqeplt.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xuiqwpnt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3argobmpj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bsclkomg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xijclkcq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3cczeszzc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3czhiedeg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3qcgkylgq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3uzpduxyw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3yqfxsswh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3symhgkly.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3sqlebtcm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ofkmmwpd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ggucbkgx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ivmljqou.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3eyhzqmmu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3qjbwyhyw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vtgypjra.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xiignrez.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3dekysxuz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3reoepbmc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ybtkvsby.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3eyepmtgo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zzuthjul.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wnllcyny.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3kqfclurb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3hdlvtgqr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3hbktwtpe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3khncvrhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgldkium.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ifyicnqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnlpibki.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iysxqors.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vtulypnd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3emvlpafs.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fepnirlh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xwfqfcme.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3zhglummh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijaysyoe.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xpbskavs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3uumrwqyx.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3whvakwqp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ayihuxet.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3iqaanifg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3thntlypw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gxewdbse.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xveermty.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdraqefg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3brzyhimr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wmrxutyy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3mxrkqmvw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3gtgxppxx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3fuafxoik.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3tuwmvfce.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vvoedlsm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ulenfgpz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jmdwsvmk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3dpbtdlcz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3cykindfj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3voshllfx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3avnscysr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3quikvvgx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3bhneurmr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uakvxzle.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yfaebcnr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3bixmcxqd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3morxjeyb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fwzodqfy.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3zkxxutsg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwmvwfdr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nxcqyjvt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gngetdba.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xbjyygzw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3mtqaefpz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3itjcwqaa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xaeulmwg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jsvdldst.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3qnuaeedv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ngkhdohz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3sugtaajs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wjdikqov.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3nimqjryv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3egndrlvr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ksemicqi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3macicpxo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vlqokfbg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ermodsef.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3tffzvjwu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qohjwkwp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3fgiioyoe.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3fsmvpmjc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3cliootnr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3zkbmpenf.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3nzhluiai.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3pbholksq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3kiwzjmyy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3qvyfydsr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3osayssjy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zzxdqmjx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3bftbuawy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cmndleeg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3tpxemrkd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3jrjqmtys.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dyhwftog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwzlooxh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3wceinxtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqfbmrde.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kkvcmmkf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3yguocfny.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3mscvjoqr.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3nmpexccj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zffntmtk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nrookzuz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3tkqjxwyp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3zirmueez.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3unsynmdb.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3puscfqdx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gdyfrkzf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3onwbjtth.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3iufdoagr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3utuwgxgm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3xlffectm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3jezqdefy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3gtqcjbuu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3fdrcjjud.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3hojzdljl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3wffyufff.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3zcotieck.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kkhfctbk.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rugridyn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yvhznamk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dolxbdht.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vkejunct.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3dsyktrrc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3mkdswmqu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3kahwipbh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3bmhmdqoc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ebfzbguo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3nvtaeici.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zmmnwrpp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fmsfjswi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3cegpncje.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3frbptyfj.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3fhozobrf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3rgkvbdnc.html


<!-- 参考信息 -->