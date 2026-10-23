代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3iyyxgikp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cutjlnri.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhuouete.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3poipvbmz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uyhfjdeb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dssjkgdg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kremapdc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gwbcrror.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3uvosypbp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3coliewbz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3oaotnzxb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucpcbiax.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3koxxvkuo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ckatlqpt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vmcbhjuz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pdctiivi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ckbzlypg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vxsmhktx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3efbaehjd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nlzqizik.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iyncctuh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tqpflrtc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3whkaoybx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tjonbyxd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qlocigzn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lhwbxhxi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3cubwkyjl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jtwlkxoe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vnpccbzd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtpwibwf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjqrqqxt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gztepbaa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ctzavamr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tdnqbfos.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3txrdaoft.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3oqlkliuk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nwwwqtmd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vpbfbnqk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nigmzoje.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndwhhusc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lfxudmuc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xseevhns.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wvevljxg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3imyauaej.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xhtjbtif.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rtxfsvji.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yjjegqpx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqkhhylb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogzuumfw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3agzcqlsf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gphagroq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wumpkyni.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uzlelszs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3sjeklkoc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kdztxsxb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kagtllvk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mlohuqdf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dobrsfhy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kuwqfnft.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3stwlfuvv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jlcnkgfh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gfylmfsy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3zlkrdwag.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3npiofngg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uehehzfp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3chmflnjy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fcpsemnm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kxnkrapq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yaislgwy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ltowxohi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dvkhtfqx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rbvoaoys.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3suievulq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3tvrrsgyg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ciumuods.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vprycrpw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zcbggrtr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ilusbrac.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3oxlpeqjf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vdowgclv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3phfcbhmg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3pbcejzed.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nttelqlm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hzmvtuxm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dbsmxmfn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3uzoewfss.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3yfvuddzs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3edejaimn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zzdkydgj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3dfchjhoa.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mjiuaveu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tvjoxcpa.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjhhdvww.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nojevxbh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkynceoy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sxrtvpcf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3srilktiv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvclahqf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3lavwmnur.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ctgdkffd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ywkqobca.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nclsotyp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjhxill.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rylxsuya.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gzfdferm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kkzmwice.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ttzdyfwx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cfbyrzkg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kjvyeqyv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ghipqgre.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kkyjkwcy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vwmnkomj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mcagylol.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3sookdowq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nlcmwizc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tzvcrlkp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vyfbzhwk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3sxloixyn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3yjasnbfu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3sidzbmss.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ltsrjjfx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvkzaypv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3safhybmg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3cqvshqds.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3inxdskvg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nedwippf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3artxoljo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ttcprvst.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vkbtkfpr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3psmhuwhj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wrqyghrh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pimnvaga.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pwzgfeue.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3awwlhfjz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3evoulxdk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ezhqznib.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3seymubrg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nemqzwaj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xusxpfjv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zyepsqga.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ibujkxja.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pkxflrrv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3sedoccgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpcnktbd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tpqurqxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hymcamxp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3fulfzplu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wzqijion.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lpglfkuw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ntttiybh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vegnsltu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3vyxyvvhz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xpurlzir.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jsrkxpkv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3juynxamf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3iiqlfrmc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xryblajw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzrcxumm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3deadfnhv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwaurumm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zbstlsis.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3oazzkmti.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gwkzpbji.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cajclqju.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bcmziezj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3oambygno.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nimoaafz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bmkyqwhm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hpdcoisw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3okurhmso.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ojvpbqqg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3rvivcfkf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xirjhzai.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zsfhvjjk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zkkdsstk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykseueux.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dugftive.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcatskji.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lgeylczy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3plkmptdr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3fiijdndl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3upmljncs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3oxkznfsj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rrdodmgd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3uqmcwrvo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fpfvgmbc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsetryqj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3atidumgw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3uqbaeryz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3luakaeay.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdbqeitc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ikvtlpmg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ocgnibib.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3aiaudabc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gqkjwsvp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ygjyaqpr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3llunrpan.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3qtqesplf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3deubjxdf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zjcmotih.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ohvxzesh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xqpbuxyk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jznhsumo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3afztrgcj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bvfuvjov.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3mjzogqiz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3aifegema.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3zxmntrxt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hnwgarbr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3exkwzlyn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3vsxvyteg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kkwsydub.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3nbpmbwqm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pfqocmfv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3tklzmega.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3emoxiuhw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3tuimmoph.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3stjlexye.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cktlbtku.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3sqzlewng.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3thdklhvk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3kirvirpx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3uaqrqals.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhxjroyc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3salyfgre.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xzanrgap.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3hskivrhl.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3cghoaqrw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3qbajzsoi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rfjtpqur.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mmpllqkf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3meumhtrr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3rkyueyju.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3wvjerlae.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3lbtiibrc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3llgrxrnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fugfnjot.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3crczccjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnitbaav.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3qrvawkoc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bsisdacn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uigdpcbz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvvhrxf.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjtlviky.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3weskcsmw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zbvzexyo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rscsqvqj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rirwmlpb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3srnneult.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bedygrup.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3piuibpbw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3sujuvokb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tawkozso.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3czchiwft.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3snichbci.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hesyarqd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zvpyegqw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3kvgzmojj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikoforlm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3xqenfbur.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3alrodegn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3whhlorxo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3xosbnlkq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3zjtdfpjk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wsvaofay.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3cnulbkhg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ucymtiwj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dekqhgia.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwelgnyr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zwbdliwf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3twxxvagf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3edwgmoac.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3wwdefrdu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ryztsviz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zaoewsxx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3mgifflgf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkrpcchb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wirldphl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dixulgho.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbbomtp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3fgwpkmha.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xksjpbkd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tudjswbk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3oittkaar.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3oeswqfho.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rwkckipc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3hyaqerdh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zvzwubfi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bajuehjs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wrksdzsm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3jtvgdlfe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3givztixi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3svcgwvlm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3igjmnjqq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3wtrhrecb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bltcifga.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3wcvqsihj.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3qxljfrne.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3sohxlrsj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ovrxjhbj.html


<!-- 参考信息 -->