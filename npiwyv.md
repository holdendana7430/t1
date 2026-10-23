代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wbejprjm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3gpjhskex.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ecdincrk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceflldxt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpqwqmeo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgtlrakw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vaspsqcp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3gddftker.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3piqvkpav.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3oycmrckz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3lmwsjwir.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ribqmtgr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3smrlblxd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3aeaojkax.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jupmfuji.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xfnqwjsx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lwiqukov.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fngcshqq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qvjkhzqb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cerqnrcq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3aeildaoo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zgrxmcdf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zmubmqlo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3keuxvbsa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ilynrlql.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fnjeobsk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tkmlwsrp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3pedenvii.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3rzhlgqhk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3besacnge.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qlpuguyy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3stmjflnp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vzbwmvcz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mbrslaam.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3eedbrwuo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tztfhgco.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zbnezkct.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fggeiltd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jguhgvrm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jktgxcju.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nuxnzyjf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3arkgicyk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xnwuebbm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hyyzozqk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ylzhlzwz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xnyyuxsh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rtbwgxlt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tevdchxv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kflvrobb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3phfckfxo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3skzftntt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uegepivk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kfaxdpjq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3liqkpspu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvwkvzrc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uzvknjrw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jcjtycnp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hraepplw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wjwfyzup.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irrjmqcn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gafqhfof.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnhrszru.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ycehsmdx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qplsxoli.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xfbyojfe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3itnaxudj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nvvogwkc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qbmiektu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vhjosmdv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tfcajmxi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rqhfanan.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3upjbktgu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dnoasjfr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zhkqgqye.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bfcxojrt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vylgapyw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qetyuuof.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3xpcsjjkt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yzqcwglx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zhmkbjkv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wcgxkidr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vxpcydjn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wftwpsyy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcfsqcwx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3wkpzxdxb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mhpqgmes.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rxxuomvq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xzspcrlx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fnqiyhrw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vleoecew.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bjtpcoou.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dqjsqacu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3oeyajsco.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rcdwkcba.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3udgkjkfy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ujekroue.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xqtcbwuk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xtmaymvo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yvgjyfte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcuxpabv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vywkbdhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvnwwxjl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qqbqvaip.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3przqhlux.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzjwqdlo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xijrozgx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dntjoahn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3uwhlsgss.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tayyrxng.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ycxfzcmu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlhzwxlo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3mdyrxmoe.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3jhlawwtd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vhfnflvx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vzdumhsr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ytddntop.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lhnqxhtl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3lngfpycf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gzubngpb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jswuqnby.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nfipsbsq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3crqbcgeu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3siutghml.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wvrrqzlx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3psgityfj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aghkihyq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3xpngdnyl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jqyiqofr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oqhpjqrl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ambhqhlu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hzqypusy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvdqfleu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kctmuirb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtmquutv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3buqlycpp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pnohkhbb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3kqygacjq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fqssurha.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vgjnkkhc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3erygxjjo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3apceshzu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fnbuwccl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwoqgayw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3jntxzmxm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3divaaklx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zyrhndbr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rydqcmdx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ekxbiewz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3srxrmsoz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kmciviiy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3phusvxdu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xfczduxe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3fcpqioim.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3dsgpafdm.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3euiwogfr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3mjknhint.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ygpvfbef.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hjyucgit.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dildjqaw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ztkegbci.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tumdcbbf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3tijhoppc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3bnbmptmh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3eyudaaqs.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jqfsykvm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3klwuucvh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3lsrlgrsz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3grpbeiao.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3rwvmfnaa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3usjydqkq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3dlsehnta.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kkjdzggc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hpvodeqj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mzflfmui.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3hnicsppq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kozdhuxf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ymzbaekq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3tzpjhwle.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ixmnypcq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3dibxeuht.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lheagwia.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3rljnuckw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3dvfjkdho.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3gtivlisd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3kotflhak.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3crmgcbms.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vauusfsq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vyaesbxl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3zqeebdqz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ytpybkfz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ozcwjayd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3flacenll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bukutawf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3rtizfopw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntsgkiwa.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ftwatnqt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hpcaqwzh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wrzxojsa.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvkznxtw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jaockrld.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qnttxqpp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrqfaju.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uwsvzqgr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zlsnlakp.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kfpogfza.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wzlrqbhu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bkdedjfs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3sbrsistt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3srnjiwuh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3wyopqall.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yncorbgm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nluqcwnp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fiyfugpy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qgjrowtz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3dwskxxje.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zfplhrmo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3wtzqjakz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3snyidmju.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3patfmttr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3fswvwidu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3auzzlhvo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3nerwfzfd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3tdpjaptr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyglpbvu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxcvsuoa.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wkcsgdmu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fyfhrdqa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ldsyfofa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nczsvskc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xslhwpaj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3btfwsstw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vbghdssw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3paepspcn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3omdagihk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ekbtfeai.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3exuozovj.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3rnfxvqrn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvfuzyqc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lkdmkdqw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kgxvvhxt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3tfjiiieu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ghuohpon.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ihbtlmkz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3dggwepce.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bgvriqxl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rvykdbbf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ptquxwqg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3xidmusub.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wxqwjgdd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3kzyghpkk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3cydlaxdj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wtbsozdd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3agivaush.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3zwlafgjj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3cfrwrsoc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ftmkvqtf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3lozefpbx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3smemypri.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3hzpyfpke.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3geirsuqa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3rxiopuei.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3suqoxqny.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gftlfwhx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ltfoeyhx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3masiqdxg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3elicymon.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3jnwweark.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hrdyshpe.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3hjrqrdwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aweetjcn.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3dmqxkktn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3pfotxxlp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3zfhbbbrw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3aqcalqzq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ncvvxojn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3roxpyczm.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3xcepttyr.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3vjefsbxq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3eqfwlwru.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xynthztc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3jlvfryhc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ixbcmvhf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3wibqshsy.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3mroqoijq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3nzpfmimi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3codsopas.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3rctffooj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3flpwipdp.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3sashukpx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3yvyvvzbd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ffszfglc.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lukuxpcp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vedhkplu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qtbrdkhs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vwswgbyl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bqrhstuc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3yyaudpjv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3jqzbyeya.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xywpwbbz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ucimawqy.html


<!-- 参考信息 -->