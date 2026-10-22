代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtkagpwl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2tifcmkxa.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pzffbgax.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2myoormac.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qywovswz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ryupwgph.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imousvbh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yydeyjix.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jnihnbeo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgycmrxv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ratpjfhb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dldzvlvh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2voxkvhqv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nfgllfou.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bvcmhzzo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2sxzdvckc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mhdctnpd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jkdkfmmv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tuyijtdu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nchducbw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bjmxqsnc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2phaalrfg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rasqysez.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2yhsrymbf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2izrmpzik.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2pwxwevfv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mxxukfrw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjhcyihu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2asrihbjy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xfjwyvuo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qtwfjgde.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zpaqydiv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2kczajfmn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zqcaddfe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mdzsvemt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2eflmiewg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jrkqsoqy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2coblinlw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hdqudgzk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2clzmruwv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xisvafuv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zcvclrnv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fvwkhxsw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kzvguiic.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2abkcxpyi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ycgxmccg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uoqtywid.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2elvincgg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gcligima.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xzgkypei.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hbujyjom.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaifexvz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wiurexxr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dxsyvskb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vfhcgmfp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xeiobhlv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2spukrthp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwmuahpg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2krrcphth.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bbnxlkfd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2krypgeke.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ynfuzbjm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcbpfsea.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yqaioiyw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2koafjxae.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mozmcaox.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xbfxwgho.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hupzhwkf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jyuknyxc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zrlxcfxp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ihztrtku.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mcnoevyv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fohinrap.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pptqbisj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ulakpsxz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2shhpwvaq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lcjshkie.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pddqiays.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2nsefrdiq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ndqpdrjn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2dtllocxh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdazshrm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gffgrcla.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2orhlnbdt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2dtmfoixm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hzdehmpk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2arjhqayo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2cwrmzhpn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2haikqlfa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wnrwrqnp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2danocelp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mrghksej.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bubtbeas.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ppccbpvz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mlxinvmb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2uqujozrw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nutgysvq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mrdosxfp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mmmkecbm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ltydugoc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2cclgmwsl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2sgeykhnb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mpdgzmfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpcbozri.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nbmwxhhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ughgscbb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2yihktagt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lxulwqfa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2angpjbdw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwiwbrcw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vspsiajd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gmjzrtjo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jgrvpxrv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vifayqyu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilinlnpy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gvfwbkdx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2yadqvuws.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2trkeibzl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jnkzrtcn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgkhgcuj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2velvtwlf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mapzifya.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fxiopnhv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqrqtmqw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tfsdftxy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2hahotnat.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jynuxnvr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ncsfejpt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nripfdpk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yusilats.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zorpihri.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ummbemlv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ykowgkle.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2bzrwqfnd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2skdhxxnm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2djeymcsj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lhbqeogn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xmogvait.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipdzzrel.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2elnnrcbb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cfdooplh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghmcauqw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2lgwqkkes.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cddaztca.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2dcnidldx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cannemgt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jtolrbww.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pffacjat.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vofxeuau.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2kapvdvsj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fexqyczp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wnqvqmtm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2raczstfz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wpjdgweu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zjflxlvq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jvtrsxpr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2quniqaln.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qdznbbrp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qxxcsuyb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2masjwfkp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2zurkskfy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zwndhomo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uztbztzo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ncodxpie.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2thopqgbd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2tbwgmxjn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hngrorzq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2guamhiyv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tjrwkwra.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2uwikdswk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2lxsrjzuo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rmjrpapg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2yxdssvon.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2axownqvr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2mbrlbnjt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2yfbhjuhd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2psysxcqa.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2uqstmdym.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2roxkjaic.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bjradmer.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2dpqijnjo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2fprfvioa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2iwpoxqld.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2lxjoekaq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2eoucawnq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2secllecu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2eikjybhs.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2stntmgko.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2lbgzvsga.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vsekbfei.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2iufjjrlj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2pmfdanaw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2gvdbyovz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2utknskhz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2pfkqkvrn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2berpcjar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppuwgzhr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2tsztglmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iffvrpqc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2cixkozbx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nklveyzg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tvkavefj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fheqiwdp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vvdikjnb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2pjfuhdmr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2mtmggwnx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fygbaiyr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2doynhbfq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2hpavcauu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqcqrer.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2mmlhkcoz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2guilypug.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wthwdwud.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mwjwtzqa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ubexxfuk.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2okeqggjd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2htykuraz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2rovelmtx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgavvcwn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zdfgxrdw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2obpuzueu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2kynbvail.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bnxpwovd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2wtywtykn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2cpprmrmi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2prsopign.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xpcdvqdl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2wchohdrw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hbbhijmw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2kodwwlmf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2juzxufqk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wmvpmmlv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vuczxiav.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bzkywucm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ydvfoipw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dnwfxykw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iokduvoz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xnpkhdmv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2smwmyebd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ocplbjit.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2ljkplcva.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjfwusem.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2eqxhhxtc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fnfjbsqw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ebxpdsgu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ykmnnysc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2aytemdbk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2utraahzk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gzocphkc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fnxrfgyd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2bvudtcdr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2tdzowrod.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2genpgmly.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2uffjhhsd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2khmedmgc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2cusdoqkr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2bcssnnaj.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2gctugeml.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2zhpbzvvg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2mxhafrni.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2zdcpjdga.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2xyngrprx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2xgxxjgxm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2rydjqqjr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2sasyxndc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mqhtwfvx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2rpgfntcf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uznwidjr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2mlarwzft.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2kxetekzx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2opkfnzax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkditwvh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2hgaodymc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kumbwcnn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ntaplloe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2nhqxjrnx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2uwqgkogi.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2aptuvuuk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vcnpffzg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2zozjgnrh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2fumsnhgh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2kjqouywe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2kdtxbbhe.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2sxcvxdbv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ydpuphwc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2xababnzi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2iqgzjqri.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2jzlyrvfk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2wwpzrqkq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2cjasvgtx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2spqzyxmq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ddmlnqol.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2seeaycyn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2omrwunwm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2wzztsmkc.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fzndvarl.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cnxtwanu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bkmnsvzz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tbohynvs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ixpnqodx.html


<!-- 参考信息 -->