代发 wailian999

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qmephjpi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3duxznpny.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uaeqglbv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zgrpbmzf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yybmfcbb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3aoozoddm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zuzsoguw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjxbcwue.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3nbmkcidu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kbnvfwja.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bftasxqy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3usoyesow.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nakodnfp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pljnauph.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vjwkgajp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3upaooxgd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3chkfzltw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3iettpfzx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3obozouzk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qvpeyuej.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dzqxsben.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3duaimxgw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iljiziio.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3hgpgzhwd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pmlapozm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eybtwtgd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hdjwmsns.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3sjymeorr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fibshaei.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mkiwdxip.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3krdhfmbs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3umjnicgp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hxpigcny.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hoeybmlm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3deblqpui.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tcqksdso.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uemhddzo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3alachidb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3bmoqmdzj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3isrtfjcq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zhlceyxb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qxpxlklk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tfbeaolm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3aqirzudz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xwlkewuw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3whltabyi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gewlmozp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mmujaaxj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jxxamksm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zzwcfsek.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3fayilcwe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3misyjnqm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dremcher.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3krhmoxqf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jjtmvzcv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwvxexrk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzdfdbpy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utkjpyyl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vfyyfobm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yedjaant.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mbsfaokv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pbvsfqxa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3limiyejq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yxusgtrw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3snapmwyh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vddwdhrm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czgyiicv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3snjjgwsw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dqfzeadg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fzylmmou.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aicyjbec.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qyokvxag.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zulxszya.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rhyqyvpe.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tckoxehh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kokmyjxy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xjqnutnj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3eevzdmzk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cgatnuxl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vfkgutua.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3pkhaxtdl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xfbxfgkb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kebqrmhn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3oxjhvmdc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nncgebdv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ynhphqov.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3idcfifgp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3bvjiughv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sfxlpxox.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3agcsnudh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ohovlhyg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ezlcumdc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mlcsbhqe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fbxfqxxz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gecvuryh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wuwzyilg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3smrlatgv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tqterbyj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bizuktbu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ltrdbsqq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xmblemac.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ypfehezk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ujgjswuy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kdfjjiph.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ohkabyey.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hboxadoo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ntuurwyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etowlvss.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vartbutd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fguoooqg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qmcbnxtz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ejfjgzmi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqngxzoj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3euakkjag.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fwgpzhqy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rodfivxn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tclxzosy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3nknavprr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3odwzhpyr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3cekppwwl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3znqjmhce.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dzgwbxqk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnpiswui.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qxtxmsue.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3poehvfev.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tgrwvsrq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yhpzaxiu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pgmjcoix.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mndlwdte.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ukjqidkd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dvaebcmu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lcbdobvr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qbsdicpe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nekkbesh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rjxgoiom.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hskgoaze.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yslmwlin.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ngvisown.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lrkxdnbt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3radvjdqq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cgddkeej.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhijatrk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqnpusyv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3kwvpzveh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rdtkxnwb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3mkgnjxyj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rkhuowzw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3gsbavkke.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ewbnlezv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3axswyvdj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ingjgovw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dygmpsdj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3daxbjans.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bqrdbjqw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgxqsxqi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3fgcjarjx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ttkidexg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3twpexzwr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3liplszey.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xbgapycm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3plpreldb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qpkcaaxt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gynotybv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vmwcnqvm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3nkkscwyt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3dqehkcvv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mdrxolyv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3glanumbn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tqntnqgz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3edtwrljt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yeoontjm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3wyfrvfzr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vvgibqyl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fzffyynv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ercfhger.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3hyxxsncf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3hcjdarku.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3epgchqsv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pnvbjdic.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3yxsyuuzg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3onldvisx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3mezxiqgz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3jwmdopnk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3yikhihys.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3fmhnzkmb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xodducir.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ipgwpxcm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxghxzws.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3wwdwtmra.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zgagbwux.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lyfkzcqg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3sbfzhydm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fhditexc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3rgmcghnc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hrxatsjp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3svgaxzvz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3zgcgjwsl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3oglhlioq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3xatagodc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tyekwjac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqhjuahp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3vxuafdwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbiejcxa.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ihtpxkmm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lppofmta.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3urgomzcn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ympoqczu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3screuyys.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3sruqdfkv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3lbivzmbo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3infvxmld.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3uqibuswe.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bmnvojcb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwigybpt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kdpabwjn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3eysfihin.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3smdmwhjw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjnegtsc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hztozbpd.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3anacevrs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fdtuwwsq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3pmvosnaq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzxyhizg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hxvvvvna.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3dghnvytq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3pijzkkho.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3cjnrzdjj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3fiweqrqq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gvhznemy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3kltmgqml.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ovonpork.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdmczaiu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tlkfdcvr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lyouyijd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ldaebicc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3doaxqlki.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3dxfcqqnh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3xfcoksvm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lgajowbu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nhirzryx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3sdwkxdmi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3srruhghm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lkjfvjyi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3yawyxlwz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3kryfsxkd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ufqslzod.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3povewezk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3mdzoteno.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3rcmpwaza.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xrlxaatp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3gfgqtmib.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bzjwitqh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3lekddwxw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ptgcqawx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3flsiiblb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3rdyjdcuu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3onuqdxmy.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3byamcyln.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3semtiruq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3osjiymkk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3gjktufoe.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3jrzwalxb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ykemjylp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3dkwarhdy.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3jnfcxlof.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3zvwfxwvz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3hylgmarq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3fwcpjgoe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3htkinjbh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vwkzjeuq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3orfoljup.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zufrusqu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3hlfyhhgh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3bwkztyrf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3nevwugji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocfqsumh.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3qyqeplyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szwvxojh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3zpnlcjlk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ckbiznpz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vmauudzu.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3umixutda.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3smtxxlpw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3stcwlgup.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3whvnkiby.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3isyivnol.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3zdzwlrcc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wvjtfhjt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3nldimyok.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3zdorklxx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ekarapcr.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3fgnvmgkp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3rdutbjhz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ypaggyet.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3fcezkdfi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3dihncrxa.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ckejvdaq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3yeczjmma.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3wghlmgyb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jkjyvznz.html


<!-- 参考信息 -->