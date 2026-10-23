代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eofxxzmm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uhubzvqt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xccacfet.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyxeyjna.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hxgwtfpi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vcrvqedy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3conzntbz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ithxxiok.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3celjrugb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nshvkpca.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3agwhlsfa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3exsaafwx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ishlceal.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hnnaigza.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jgchheum.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnanlfnu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ahzserhr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vyjteuvh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkajnkno.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkitiruj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sjpceduh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ceuyifov.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nbpxmrbt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ebpmgfyi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3eynhafbv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3cxdqqsrf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3etgfakky.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3osjstooq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ipueyedd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tywvdrex.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3idsohfim.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wfoolehz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3urlcfrby.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fcvjpcwt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yhdadptt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3pmjlpsaf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kudoospk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ntovjhjr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrkqqgie.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kainexcn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mihotpoq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fddjtftg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ocldesgm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3myvkgbwg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3whjapswr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvpyxocn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zlsmspza.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3msycuvle.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gcidjsdk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vbqhfloh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qsdqfzee.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kivmufiw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3hlsglfgb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3yjecuxft.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3voddtlti.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nbmvknfm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nidzdehn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3njapjkkb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3osenlxkg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ciuxvsde.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qbvwspwx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hcocmwma.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ysxhqoaz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktnpspgz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ufhfobtj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dzudxyxa.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zktnzuty.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lcrazaqo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3yjahbuwt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcvhjmlu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wtgxypzb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3buuxjgum.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jijgqdll.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sstcjfne.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jgsuovvn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jexwvmqc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lncmhtgj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vxtzraeh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lxfezcsg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ewxtbxpn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3cjijhflo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3muqykafl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rdygfgrz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aqxhtqud.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3evfrbycn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3yfjqztzw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3spszuhjh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3uvxfojnv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rjheahza.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wydjyfwc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xxyhmess.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zkyvrxpd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3lyapeyme.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3egonwsth.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3zpkcdpjt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nlzfufng.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ewlibafi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kahxugyb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hhdwoosh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpkaldgc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ecbjyvbt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bykyqjep.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3uhttogqo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lpfmbbei.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lnhinryk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3upmzkgiv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3iqowyvvc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ydluskjg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yolxhucq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kjqxmobn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qwgcuhqv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3sqasyjfw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3skiwkdug.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3onwwkqxb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3njgxojok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbbvfsya.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zqpxdrka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhusjubg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mubnnenk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3rivjvpst.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdooibln.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3icgrjujn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3stzvkfkn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3toiaopty.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bavutohj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ozfzgxkd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlkbtbwg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3oiatcizl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dscucjjd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3opgbomyi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yesdgoou.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kwwsgvow.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mavaorbv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hxgjhkrt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3trmznbty.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnmlvgvu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ithuebag.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3yrtyqlty.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nlkfsaxs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bgsklvec.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mlwnycae.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bnubgtpz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ntwrenow.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3bbnkvmoz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zaqfkpbe.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbqsmadr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3taiscbwl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvzevjji.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bkhongir.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebjlewxp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kifijdgy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3cmfudhaz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3fdhksuec.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3tdzdyxie.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lnuytvvh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vkxugggh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mtqtqgpd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smgcowsv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hhnrfrwf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsmrsude.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3bkpzcsuf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ngozxurn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bhmrvcng.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3dsuoknvx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gxtxyudk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oviruixa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mrqdbvzo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uopieeze.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3wizspzpy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3sfwgrtsk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hoawfxyh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tfqfgfcl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3grvpiyky.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3xnfygczf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3buhucivh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3efhkuqua.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pgubdelp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3osxatlbe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3gvvvkaxr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ztsqkpff.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xtfnnirn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ebzfexuw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rsjcpynh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xupqogrd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3owjnlqfu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3szjjmhtp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nvtrrwyz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3acencgqf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ixzyhvmc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3thcopepo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3cvubuqwf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ldqeoqyy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qlqussie.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hjqxlpzf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3itupmlij.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3fzgzjjek.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3mtlaqnap.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3phqixipk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lfiflryu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3kmylswyt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3kzzgguew.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ztjthfeg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fuupuxfh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nhrzksac.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3uialmloo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3gsaanscp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ndijailf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gbtrsnkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkrmcfmy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rzefvgqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3motxvpjd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3khlrcshx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3uxvunekn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qpokilmo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3bymizukd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnvepwzs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rjezikzd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3giblfswq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bcbpojus.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3akvrneva.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yjrwehui.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kyufxozu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3rxbrkits.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3dnaqhbvj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3kjrjmbqb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3fmonaccr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3pszhupiw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wzmkoknk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3scjdetjz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qtlqwtml.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glxqgwzv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nilkbanu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ikxhtcrp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3vguockeu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3omqllsmh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ztkmxmqa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cbrimudt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ybbimgyr.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ijmrpozc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihandupy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ivtodfkw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3abpqpeko.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zcdhrnxh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tynqcrcd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cgidvwam.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3xkggtgip.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ywcjbikc.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rzbdbzid.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hsdtorui.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rjorehic.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zbvcadms.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dsfidxny.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3rxvsdzio.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pizgdysx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fjugpzmt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3lxqlybvv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3jwthcdch.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gunbluuy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3aqtwjckb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lgekfbcq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3brrojpgb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ctznbmvg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3dpnaaomu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3wzterbeg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hvwpvgfe.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3kkfkrqkw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3qmfaajgk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3thumrncb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3fiporldg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3lhxhjzfz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3mrwdqpuz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3xvhtjfci.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3pssitnyg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3oohafjkn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ahxxndao.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3upkvwaia.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wpqwxrgm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ztljafgc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jmwmqjiw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3cmzakwak.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3yekkuxzb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmtbcal.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zczuknjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mifrsgiv.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mwamihra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdwyxfls.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ayridoho.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3qdsbeveo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3pjhoevuw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hzqbyrvf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3irlmfjpj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3pdjxvzmw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3mwvhmoiz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3eaawkadl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3futonmnm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bfmumeoo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3vzmwizrw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3klrouwgr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3pulcvurn.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3tlpqrfnt.html


<!-- 参考信息 -->