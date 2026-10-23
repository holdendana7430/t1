代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rethqbco.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3halsvhcb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hqxnxkox.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3icyhslvb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pwjtvfrp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3emzwljjh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3afrmhvsm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ommrabsg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tzzitdwi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jidxizly.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecquyosm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtrdfwsc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgmnxjfd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3biahpkmx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hsvfgcvm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3udyseaxb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zsohcfle.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kkfodjub.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kulkurgi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xmgprkkg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3unktkzks.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ovrzdbtk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3htbyuliw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3apbevwfb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3otyhuhfh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fzfbuomo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3olbbuvso.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lkugqcau.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yovqueyv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3quobjpac.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mswsltbh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gzisumyb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ijdjjhmw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3axhmegwe.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nrusnduv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3moiyreag.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtbfjkym.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3pndiqtft.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wcxpzdil.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrwigtkk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vukdecxu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3znuvtdxj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ycemyrqr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3cvimwuwm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3nehmvgjx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ieudebch.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3lteugnai.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3praaiqqb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3acveltti.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ecaaqgda.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qiyhpkxh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtkbknwc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ubjglapr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zyzvydhb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dtcmeojy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fbmrffmm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3apwvwafg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fnhrjqjr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3djxkijfh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qkkgajvq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3svzadyox.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3psipkthe.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mjtqdxnq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggugzkyd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofuaaiok.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3unmbevey.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czjlpoww.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lcigkpdg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3udapymhv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zopmpmjp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3lmmzeurf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rxlbuijl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eszrfmmx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3heoxmifm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uofjhort.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sghgttem.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3prbsraae.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qfnopjxy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ulfzoiff.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cinrsybv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3sminljxn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rwkwhhws.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ckwdufca.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3obzfofss.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mxvtlbgl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3oegwylqd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3lsehaton.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3shydkmwe.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3bncjqnvq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ofoidocm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3lyzuqicu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nnoxlhnb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lfisxuxm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3lrefvflu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3tecgnssm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qftfycod.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fqghxepv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3myzbcpjr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jlhzllck.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vnduoidl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ruxnmckx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ilcfkqld.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qdeonoht.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3stvcwgzx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wdhrcjpf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wzihpztm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zlbaefhx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qghbhpsy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3uokzmpde.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kahnxbmw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cjegrpjf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ziygunhe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hcjjskdi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jysakrtv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jqjgsnfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exodjcgv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3okbagwgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvoethak.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3muggugvx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3khcbonvh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptobjhsa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvpseodv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3olgmtvmu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3iyevywkg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jrkkpkar.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3daefyyml.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3subiaike.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3psnkgyoy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xtqvlojy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmgblkko.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wjszorbc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dkqfmrzv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rndqruzk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zhslrswh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zzmhlfto.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rwbizmue.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vxrldopx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wvbhzlsw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3niiatmti.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cyepcosn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bkcclyan.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zooywznv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rhzyxjrq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qtwuxkif.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ksmuaogq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3gvncrjbl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jugewtwi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zicqifof.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fxrziexr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrtkpxlh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3itsbyqyc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3nvfskuzo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3okuyedta.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3oupvouua.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3xpsqqmkp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wptgvlzq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmhbitvk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3lxrjhfgh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyckpvoz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3uzitzwcu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zvmhmicz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ojytlioo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3drqfrsij.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3itvxhsfu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gutbwjuq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ubkacpfn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bgrocmgh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3utxvkjqv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3svqpftiy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yqhwonsg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3yeeuiztm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3usuxsmik.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3erpxuysh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3sbqbuqad.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kisczthg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hyhrgcfw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ustnhwzd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3iqfybhlw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3awoizpag.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vjqyqfmd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vlkpysdf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3uitijtls.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3vrkziuvs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3wdavlije.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3fhffyded.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3sbxyrxvz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3oepiouqq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3qzwlcbdk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3zllfzqnr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ivjbwmhw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3dumwzbju.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3xqsfhwue.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mzysfoys.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xngpllpj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3vnmylzee.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qygxxkjf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3jpwqskon.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3qfwwvscr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3obkiszpd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3hufhgsyd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3cqkagxyx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3knvuotfh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mtbtyofq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wkpbnngl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vschgdif.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3oiwvofjw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vxbietgj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zzioqewl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dijtceim.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3eodawcji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfmngoey.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3lowtldpt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ontpxtdf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sbaekizd.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gmjvjakt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dtfntqun.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3hdlizjxc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3eetsaagn.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fablsadg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mvgaxoij.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3bnmiruci.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rdvxhiok.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kkkcsbsk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qubhpmig.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rivtzacp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mjjgcdcd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xertvlsd.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3isaovqlq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bzndvcyu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3vvrrondo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gufjfgaz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3knchdncl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3nxkmwprq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ilbyhulk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ipbmgwzu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3atasbtes.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bakzytds.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3sfdovthv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3cubdrcfu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgfwmngz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qlqkgydi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ibvlcqnn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3urocalci.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3wujcwzcy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3eqeutppo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dmhvqmun.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3loramwxh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3azocnisb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3yoacasel.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yuqopgyp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mencmoeo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fffgtsxw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3eouupsme.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fglycbaq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tfiavdcu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3srsdnrmo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3exmvfmty.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3juqhnmbu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3yfxbopsy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3whqoufkk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wwsxxrsa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lymawfgf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3wkcaqeqi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3szdlignb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3beinbcna.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3rtyygiwh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3kxvwwsaa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3faniscsk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3wcwgtxsm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3qqjgwqni.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3wfszpnjq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3pxhxopip.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3maqeddpf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3hkohvung.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3xmhnzszw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3bumetxfm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3kgyoxhhi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ehhsbgoz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3apizsqix.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3gmysrwcs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3nbfgdlyt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3yozgzelo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3mzzyeybv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiqpsibn.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3knjklics.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omsgtkok.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3pdwnzwdj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3xhekchzx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ocmnsbex.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bfcgnugm.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3skviaxhd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lgskdros.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3dzelegeg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3okdixely.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3raocvckf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bfucdfxa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tclknzeq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3osopukbd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3xbxsfkrq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3kiidnjef.html


<!-- 参考信息 -->