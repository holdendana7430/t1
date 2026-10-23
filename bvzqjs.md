代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3osxvbkdq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gznvwonh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3zoidhljr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3udciexxg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ehuxvvpn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3jipcqwex.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3cqucwgmc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jmwqmbbu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3clzacplh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lxpcemsa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3atihjeev.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bqnggiil.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3apizlapa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wnwdsedy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3cnwhsots.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3myisoenn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fowmzgit.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3spghwkti.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3igjuosfw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3estxinfe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3nfvgohqn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qrdbfwjf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mrqimnnf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3krqwwiqg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gdqhofpr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3csyrtrzs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rnejfzzh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaunfhfk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhjqqufw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3tpdwoxlp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hrbtguxl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tslnxwzk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mhqqjjwl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ugxkzwec.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bnaqeegq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xyzikjjy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rlsqobnq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3bpofvlde.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kjywnqcw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ziontreb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3cuewwtqj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gssvojyw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3incvebvp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofrilhsq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3necqfyat.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pyvhxrqk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lbkwfvzu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3etiarhqa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kdpyzidd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyfluyky.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kuycngyp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cfeeehgz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqhhyklj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icbnrdax.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoihnsny.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjqnjmvn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cmynzojq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pzewmcww.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wjhunfps.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3epynlvbd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3sszjazik.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hgcqsynb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wsolkxoq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3phshuubt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vgjfiyvs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3cytztcho.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ivqtzcxr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3giqfhjrl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bubwwmuo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ripehvqf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3uthwflar.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ibshmmmy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jyxmwbge.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfsohpty.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vorvxmas.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gbbpkviu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vemcqgau.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xwktlruw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pcqumqmf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgdnjcsi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3cofghoum.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tstezjin.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zgxzklty.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ozezmqtc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3enhggibk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3inbvrqpk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ompvqvgo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fpbawpys.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3idszeohv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3obrrxukw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gmnohgpu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zmyuldwk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xisxjgxu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3prforged.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vialvako.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzusdetj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qctiapyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obarvkmh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wfyplumg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zabfuaml.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ctnzbpwj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3anpwimkp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqgnrhvl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcatigam.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rhomvkwx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vcykrdrh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3pcrmiupk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qouhgeze.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3zkmawggl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3afidexym.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kxqhmjib.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ungfdmca.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ufxyxvde.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ilhuottx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qjpvgkno.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhpxrzuo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nnvvjdyi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3yjjgiasb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kdouwuln.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jizopnrb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jzqtyacc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eunaylru.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3mhdwiisb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qnzuavuq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lrwksesq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3tbjqbzvx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zajxgich.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wfbdmtoi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3udedpeqd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3skftwcch.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qzjlhycx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jsakpgqw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3elryskto.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlnbdxnm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jrzewkyj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3avoginvu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jqxaowfv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qeokczbf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ajfnjisg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulpbjiru.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jrgnyllm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3htohlwue.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcxyyfeu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wopcxykn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3oaroijgl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nydqpvzp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vvvmgxyf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xzdqdlhe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3umkykvqb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3oocvlmnn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhpgextv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zctryqvd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rxfequba.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ysklcszv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3togqbsgx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rheieakn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3shctynlf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hzcpwgfn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zbcxwnlr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xczpafeq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dcuasakq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ybcxtezy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3eengbwue.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3tmsvqwbq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3crsvqwmp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ssrtimfe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ckwlbuuf.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3fyfvwaeq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3osohbolz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3dmpykzwz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3upcyozbt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3utasxppy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ihumfgkb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3jsxnyobc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3rugpcnop.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3etctfrhh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vdjpnmss.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3kuhyaknv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3tbnwctma.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3euwfkeyu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3vtzswnxv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3iakalste.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3plsbvaqr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vlxoupfx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3lhapyrcd.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3donszguu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3rdnajyyp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dwdlukpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3redzpram.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3toxmrdyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnlavsjc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ogauuiat.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3krsngshv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yvamebpv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dtjixkhk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvoqgpts.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3kiyeiohh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jldklmup.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3lvvetfpu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gaujdwiy.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kwuavmma.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3meeaycwu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3jitwofzl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kqsofqxy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlemnor.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mioeudad.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gkftvjox.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gnxhhbmi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mpmtdkwt.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hhiewaff.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3qjznbuqu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3kpvgnzfd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3szmnschj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nwdebqub.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xbbnmrkv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3guhpenzs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3crxuhndg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3abgbiysy.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3iixvrkon.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3mvqvxjqx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hhamgzwr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3iirmlrup.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ifddlorb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3eehckqqh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fkyczvqa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3oyhkiues.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jmpsplfz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qeqpshrv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3omqpsyda.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aqajtvfi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ajqsniri.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qyxckzss.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3citcbhqo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlenheii.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zuprihkk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hxebyiwr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3opgurhta.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jsslzeku.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3rrmvgehc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cnxnongp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3shvayhtd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3htstfgxc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3fkceyjgo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3acjvzyes.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ginulfqd.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3vumxbbwc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3rpxjkvbk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3tdsyisew.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3wpcrvket.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3cyeaemlw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3aczjyroj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3yqjrmmlo.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3zrytmpge.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3twnloiee.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sjlqrkjg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3gmakyrok.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bpipveui.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cotpfjav.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3kbhyexrl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ofudinkn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ckuwsbok.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3evksxdkj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3jubphokv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txnemgdu.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3wvjjeego.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pyxvzhre.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kzvbqraj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3geooszhj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3badgpbkx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ldiijrts.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hnmogcjo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uowhnzoi.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3lofrcwok.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3qytfecaf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3eawzkpfu.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3eigbjrrh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zmdlowls.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3afrxwrmx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3uzjubnqz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3qigwymvk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ecbptqst.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3xzginyon.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3kscdvbtx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3xmhqntxg.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3bklcpyqd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3iubqcueu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3tsrljuwo.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3olbairjq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pcplakwa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3phrwgqrj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ktbwztbb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3viuqyyao.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qzrqqnhn.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3rtztfhgr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3aoeyjuwm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3pyhzfcba.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3depultdq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3irjgawen.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yfoyohxk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3bsjbkouw.html


<!-- 参考信息 -->