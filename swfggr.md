代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nbvjonmz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3fnnwtetb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ycrpjvub.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kprawdii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3audgtjkt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kbvkgimk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xujucvro.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rlbkbolv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3fkuogxwb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbfrlhta.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hcqyhcyy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ytwkflre.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3mefnfiti.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3uobnfbiq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzfgnuho.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3djulwhwc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hnlzvqvk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3exvldydq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rigjotje.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3opjjijzl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spcgihbk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnbcyyqn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3odeyjepv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3rgpnmqwt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnppcfiv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rafeqmom.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3twsiewvw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nlhqpwme.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vzxjfqfe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ngyogumu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rkskwyil.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kjcooibz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sboesjgh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uweydkse.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vlwufdnn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gxyebitw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgohkgwm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pnhromfl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbuonrgy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tyfycjjs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dksfhjwb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qfukfabp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wbeqkqnh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bysxrrds.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wiydqjwp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvyargxo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpljpvty.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlospnob.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dzaqikqt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nihakfms.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wccxbcar.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kobjxwoy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rdfhtlcn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3twsgtgew.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ctbptxgo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3booksuwy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dbkqocml.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uwwlaljx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nkuodkji.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qvvkxzex.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vnijbllb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ufcfkxrz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nvaeflwa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fgpefabb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nnjfvijw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3izjuygzp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kyjgoezo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3syxedgpj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bjcubzgu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xrgcmjyg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3tfscvpft.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3trmntris.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hghjcskf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wxjvpqek.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3msnxqsug.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3nkvplthc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vharcorv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3wgtzdxjs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvhwqvcd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kxqecoco.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ucaoaczx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqwxqalh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3aokgpwce.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3phyqneho.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ovlpfdyp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ykpaiagg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qausnhxx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ckyhkcuz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xsopxcgq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3sjryspow.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sjbrmvrx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ovroyoql.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yxjxcncv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ggazevfp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3eqztgkha.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aglroiuy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qpirluyb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3natoadtm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3vnncgvfb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dvmueyhh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpbonueu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxitwwbx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkeynxto.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hkkotfcg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ejzhekek.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3woiqryql.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhtyptkq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3awfszgke.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lgtscwwi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dwslsgte.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpgfepea.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cmgelpxm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xhgzngdc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mgebyotv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gmbxsglh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fskjswfz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvgmnjn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xqtxjilb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fbudesho.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eemalktb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mdcqgsms.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mtpklpkz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mggmgybl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lfbgyudp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fksapewh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3kbhvfrwt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3frvshfgv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wzijwsoj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3eucexycf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mypxqcfj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dxggwpel.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jfggiipn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3cpgsrtmq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3shqgyfhe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3empeumkj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgipzxar.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zdoobqtb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dbzfrugs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3drkntzpe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3etvrilec.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3viivevyr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzurczpl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3iakqvcyb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wtaqmwox.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xxisfgmv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bodikgvc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3recmzajy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3tfcybqaf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3nxwcdezh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wumsmasg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uggmicoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psszlluy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mzbeclex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggfvzyjy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3suuiqzgd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lrmxanhc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3akssybib.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkeczjpy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yiqwofmh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hrrifswy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ridczcbp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zgkeamdl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvdxbyzn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3icgpsuca.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hrupzsgv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hspuoktv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uvujkmju.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brhyqeeu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fiiljgdv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3lgliknca.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qdnowrog.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jvydlwar.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3joncoaie.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3lcqebnjh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jskrlado.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oapytkbx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3edntnujc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xrrmniuj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ihbeudxd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jkvzriss.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fytpnfdb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3feohmonx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ywcnyjbt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaltffep.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3emhypgff.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hxbpxvsy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmmjrosn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3gehqjxoa.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vajgpemo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3bjgfgdnq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wbvsogbl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3tegcdvxu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3pzunmanf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aeescmrt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lilmarux.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uepbqnpz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pavihooc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3hqdupjic.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogxcebbg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3sigawvvw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pjatwwio.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3eysfaglk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jctmsffu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ydjejgzj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3aerwhezd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3csvgrepy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wnlqxgmp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xqdplxsn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3iewvpjuh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3wwqgwlqj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yuysqcmr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ukqatadb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dvhnxlqs.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qrzlohka.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3lcbxhoqr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3sduyuuha.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xifhmdhu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ysrcjzqb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3micknlkl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3duweayql.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3vulhehmc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xbdcnnhz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3qwixdogd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qcgmluul.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ciptzffm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3msinntso.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3arewvokm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3txyjkqfl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wcwurvcq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hjvwekvi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gqupquaf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoygclyn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3wwqedbwh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3tbccaxde.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3jwykrndk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vkgffahl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3lolnvzob.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3opzgfgvd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xvdwamrq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rmjjsqfp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3meiuuowq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ncpquopu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3oqiqawxc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3crbsjoth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxapebad.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3lnldjghg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlktuyab.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3odjhckxc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzsqdzef.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qfiskqtz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gmgrufkk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rptjsciq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3jroecyzd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3pvaxihux.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pynxjcpc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ijwdnuty.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3dqnreabc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dcmwhzzp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lrmoafvj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3scexxoke.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tdrqhanw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ujcfnrap.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3beqorzel.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dvguhasa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bnteoexn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qbqvlmgd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3fobaaezu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3gkjtdmtj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pcamyjdn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tzulkwun.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3uyhaycgm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3aggdqhcy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lkjbtggw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3mhugioyx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3nzobwobg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jgnfpgjc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fcvkqjra.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nympzqpv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3auzmhyvu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3nsdxxlpe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hhuflxba.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3odopqyee.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zsgosidd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yzzogjiu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xhfwqncw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lookbysq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dvbqkrfw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3atjzxily.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qjykkgvp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3wmgmgoad.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wuokgago.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3mycqfzef.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3hbskdwph.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3idiaabzq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3bhuunzpa.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tivuxwgl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3jfdldqjo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kktcwvns.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3bxgpskku.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3acwhtkkn.html


<!-- 参考信息 -->