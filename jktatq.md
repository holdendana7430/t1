代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hddmuxmx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qmhfrpxk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ctwgiqfn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3hajcbqfx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tzdmzmpc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wrkiwwfv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zxohbezo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gazwqnob.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxejfupm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fwdxgacp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ucqwauda.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gdafpcco.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gqoecsxw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jghqqsyt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxytquzd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkobsoaz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ncwgcbeb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tanhfmaq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3twathmsl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kpkxlpth.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3bfciszwk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3runxkhzg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3waswjnss.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ykgiusfg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3thxelvtd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kbkockcg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cznoelzd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3gzttxela.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ooxeikfe.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ftubaofw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ahuyovad.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yslzybig.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tqcucnlo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3htkexsmp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ldusjjrm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hndpmwuz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vzztauhi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3sbhaznxn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3bsikqqep.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mjgsvzjt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3eoagvede.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsrniprg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mfgconzm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ffypengg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3omffqhyd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3aarclsnn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rzyrwjem.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsmtgcux.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yxklesht.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lqdpbuaz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wsidjqbh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3rysobnaq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gcpwkwjx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ryiekype.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ehxgrtbb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sfblxlmx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3luatujno.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3trqxyxof.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rryzhnkp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3baxiffnl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwgxotte.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gvhhfztd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmttagax.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yqvkfpwn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3srlzbzfc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkbwqrpm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ruwqxgug.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kbmostiv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lduemhba.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3onetylkf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyivezdj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qnwtfhxx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ggyhkwhb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rxihzqyy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tkbnfmyx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bnncmeex.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ogpejfsw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gwjqnzbv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hkftpwpr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wfrpiwan.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rouifhnq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wqvvffwy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nfbxyiro.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qacshvkg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gqnoxujy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3pvkblydl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kthlqtuq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ldayfqmm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3fntdfhdt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oevdsipm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hbkbovyk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ljplxodh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3frfmhsvr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tcazefym.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3njyqrhhf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhxghdet.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nqckaqos.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dihiubly.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ruqjpnms.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dhlmrywv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vugpfofh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nlshxtgl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3yntyyabi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fuglniid.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kregkdjx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pbrtcldq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pcwrmrqj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xboyofto.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ygesbrcv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3nsysjozk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3agofvdqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crkfhkjs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kdogwlrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dayvmixv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xrrhdrqp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3icuxsazr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3atxqpigb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hhdrqxjn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ianipdpn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3uvlrzjsp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3fmcmvklt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3sggrledg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rnmvwfuo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rgojffmy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xizqnyvi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3noqkaboj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xoynnbvk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uawrngtw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbezqryl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rukeyklx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3bmrbogxq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvnutjpi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xmijoggv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3numoluvb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rkzitluk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lifobzwp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pgvbhpsb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vtzaxlrk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3htxxomkn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3sdmnetfh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ygxrvxbt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3lvpvlkoh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mymvpivg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fifuyxzl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifudqmyu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhabmyqe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uabpzkkw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3rmyoukkh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rspzxpgq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqlqbyej.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3pllhcvhs.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gwmcizgw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3swysofdp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivzkdelu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkhofuit.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3meftpkna.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3vdvysckc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kvbhhgdy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3krscrrpc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3rpdumbpy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qsogmoec.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gdbsudft.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cryngxul.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rbofokcg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yydfgxyz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ocjxyxww.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3fihrvqfa.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fyldbjjo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vgjevbfa.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3notiejdv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jmegxgtk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iondptyh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mzjgcchp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3lecwxoqh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3aouxfybl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3wbylieli.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ytmuysjj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ptqnoukl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kkqpcfyc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3fjjoexmn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3iqgdmxyj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3trgtijdc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zpwzxupw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3xwwdbtwy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3mrgklscx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zaocvfub.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3htmqwuvu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3aagxfzyt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fypataxh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3aodexpnw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3qgvqajzk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjnlsqhv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kwlswfkf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zvsumwvt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lwlonywx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rvkmhxnb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3mfkntfph.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qwiqrgim.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3swvddupd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3cjqrpdhj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ayhdnugt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3jpqanzpt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3fstexuuw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jshofnny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mritrbmg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xcqqyqnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3joiyqkei.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ywgkgwws.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wdayjoju.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fjlprbjg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hwnvwngt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnjhnxc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3oeoaittt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3cusivoqr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gzfnjrui.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gqhuafme.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xirxjpzl.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3geikovtw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xxeqwyvl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3onnvmuls.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ftarwquq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3hbejtxin.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ckflkvsi.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wbaiodav.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uvzfnesj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3cypjjgyq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3udyqkahj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3naqxondx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dfrbxyfr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3orrixjiy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3delvdcmw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ljynforf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3suonmmqn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3sdlqmvzc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3szhqxaos.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vgimnwoq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xzgdnrpy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vqyinxoc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3gtvpzdlr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lvctiufn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3imzrmivj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xdlquorx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3chneishp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3rbgylnkb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3bzcknxny.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ezjpbnxw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jalpydpb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3rjlthjdp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3hxfizvcr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhdmhtlw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xzsfluhf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3pqcbtufx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ysmlrvqi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gynwumkk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3dcymgtfc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3upzlndxj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lizvqrhk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zdyeqtdr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3azsxcvij.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3excdkiha.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3oejjfckv.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3wkxgthxt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzgrtgf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3clibpyjw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3agdkkfrh.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3daagxixn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3moycdwnh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3qixujpfb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3rzjvttph.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3zfknzxxd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nnpnmyil.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3nohigcvn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xhgfybfd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jgvfrwph.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fcayhkxj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ttrznmuy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3nngtlzmz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3vpwblszs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ybslupfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrsmvuhf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3alifljqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eegdzeyi.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3aozsbfgd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3nxqsxxaf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ypmqjjmg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mpqxaajs.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3yidgigib.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hlwqzgyg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3cpqoexvj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ddejjcuo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3xdcedvci.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fosctbuu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3lmlnkzrf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3altdmeow.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3tyceelaq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3dadrfbzi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3piqagjog.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3cuwyndtc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ydfxnjjo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3njyszvyy.html


<!-- 参考信息 -->