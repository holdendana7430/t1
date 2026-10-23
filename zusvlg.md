代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3phkajgml.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxkalpcs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zidznyum.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cywsuouu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qflkmgyf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zrgdoxce.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wilakhbq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mdcnepwc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gpzrktlu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hwlmovxd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3yvksjfga.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3qhqoylbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gazalsbz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3vyuvrgfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhuajbzn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3fnjxdsjc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ipmhuzwt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jmmeuwwk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqladelq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3naijtaal.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zwmnnbdm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gwookiqp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cthqdpgo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfrcopgl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bagzjfzt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nemmahsh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwvyayoe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjpayiuw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fmyddwqr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpicukdr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qmdggtqd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kgtauprb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pstktoqo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mtjzknix.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jxysdxfr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fdudsebo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tghmfxte.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ytubezxg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zlrhchng.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3okrwxryh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vbmbwqni.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3acubvzgm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fhjtpnbk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pyghhwfw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckwvuhvx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmwxmmto.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tscyalad.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbttzvzy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qvtmhsco.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fctgwstj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gnukfxfr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3glnowwji.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gvrlemqz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dwbsqrzo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wnqvmgdc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yclgeggp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsrnxdbz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3wevbhbfu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3utwvkewt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncjnxome.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qdnvadsv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3waebiydp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgoocuvd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zcxjlezn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkydbhyu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzsytenh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ikvmpexo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rdgudzoo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3lgsklwhr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ilwoqshd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3clgvvlba.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xyoodbrj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3makzadir.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xgjgjuya.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kiqeswem.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3iuwrjesb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zbjjdage.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xeqzwqyp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nfejvymr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mjjtbnxm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gizqvztq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bjwebsek.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3bphnqtjx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gllmpegy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3xcddeocx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yeaqserx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjfhuapd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kcoeakke.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3thpeboei.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmwgxwms.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qhqcbtyw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3syejixxm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmkwskso.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gglnyvbs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3huyccwyt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyirsbpt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3sekejyau.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bmhnoxgw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vkkaajxq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3reyfsvek.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sppmhzxs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3somndshm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3azocednk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kjlkorle.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3rdbpkiud.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zzonrwze.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jonazdlv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3liexupdw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wtenidyy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vksghsjr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oihescis.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ognbdhfc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zcwqkqtl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3swfjtobh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ekzpumta.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fmenvawt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3umzvcmvy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3snnprqli.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jzklbdkr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3newbnocm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wnsqeabl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpyqlnsc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wywytihs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3lcleivfv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3gbzbntlf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gcskckab.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nalvkqvd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pbdnzhyo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lfzimgok.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3loagjxev.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3sqohpgbl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xiwrpphx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mhmraosh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3khysugsi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3iidivzaz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yarrylal.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ddopcxfg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ycywnndm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3yrzayvka.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ljkwkcrc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3lxmahfgz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dyesfgca.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bbhpgkos.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsajrzji.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pgcqmiqg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eybbaqre.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3agplbzvv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pbndefnv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qsihyswk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hmkpcvpz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ysmrapqu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3avjbhjvh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qmyguqrr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ibagjsah.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vqoomlge.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3gbataxla.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3lfaolces.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mgokvovz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3utrtqsoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mapphupz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sykleswf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewngnfnm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wznjvkwn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ltwvkzyf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmivjqos.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zrghjwsz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjntcsws.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hbtvqjia.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3muqpoeeo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mqxfxwvt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rhwznqhf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ydqawwwq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dlmwhpwy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3igpuqcbl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wezkkuxg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ytvrcurn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3besoupih.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3epurxnhi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mohrvfkp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bscxiqsv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rdilruky.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tculmszd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3shpfusvr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kcojbjib.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nvrivjjl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kvoaeljw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jqaclfxq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3wunyblro.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hhetssmw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mnqbfrhd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ulwwhezr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvnmqmxj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nuyilvlu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqnkspiz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvelqtpp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mvwypxjz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3vkxooepo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dihejrck.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3doyleagc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3sgwinvnw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3gyztvtru.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbbtnsxt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wavwvyzg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvozgbkt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ihupoomt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tdgctgag.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkolhhom.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3yynoatzu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3eheeociq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qagqelvz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nocgtede.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xgdrqfvs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3drafrbfl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3csrobcth.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3teihsiqo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3tpueoruw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3lwujxomt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3tambneat.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xfvmukzp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kgtdrhfn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mepsikjy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3hhiwcfez.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xanfqikc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3zpugvmsx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fbsghmbw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3eaojgqva.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3yidpwjne.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3lkxbjfse.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3cavsygju.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ulkqaxcr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3rvjjvfla.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rtkbggzt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3yvgdaewq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3slyamtnn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3viebikkl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3lcxkykjh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3acwkeybp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ilwopjju.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3zhysfnqo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3wstwdbwl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dzcteycs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3irqbomfx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pjreojeo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3njxcebfr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3cggpgtsx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ockssayw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3nslvzrqj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qrejsall.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3uuxglfzm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ufiinnhh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ejzjibic.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dcniatxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mumicnac.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3hxdtttkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwuwxrzr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3vreelicf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eauhlymb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ecgqpkih.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pucisqzb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zviptnuj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ncgndmec.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3axdqbrws.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3divtrblr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rkjhazal.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pvetmsbo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rvdxbnst.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dkiyyvlc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3zblnxfrj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3radklipa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3eexaivwh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzavzeme.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jdmzardl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3feiidaco.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3voaqxjou.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3pswytkux.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3faitwmns.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fjbolzmq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wpidvobx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3cteeapaq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3vjmdlaoe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bkcmrcxp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3rwuvnjfg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tzgoufaf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3edjajtok.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zhptndpn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wqmgoytj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3oukiepdo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gotdrter.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qnqvquwq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uqpzcdgr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3iceugtma.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kgvsjdwv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3fepatxjd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uwzekipa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wijcndsa.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xzrftywz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3xrflnaud.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3apuhumaa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3meuejjyy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3irhriraj.html


<!-- 参考信息 -->