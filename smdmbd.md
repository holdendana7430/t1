代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujkahgrs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqguqueg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mtllvwcy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evivcpys.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hjetnffp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlbrjaye.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncnrxbua.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fmxgefnp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vaboftgy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kyzklpca.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3eiwzrwwc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bmhnqaql.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfehgzn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hptgxlbk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3dcsbdxzn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qelafhoh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3eueismko.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qsuklutr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3rdhbacxq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mzazwhbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikhegrgf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3jwymgwpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msjxczzy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qnaqgprr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jrilcyfk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3eohlmwyg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlyelgcf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3alxzhejn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3evbufyeo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3upkgbpbd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yoncvsfl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3liqzjkes.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3grexkgrz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3fjwsclbd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpjqtiit.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qftgpzjd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3owmhxrfq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ewyhhkjb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gmrlxarc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ifnfzvba.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aukcfgac.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zaeluqlj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mejmqbug.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xmvpwmie.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dvrhqrrr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3shiowbss.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mypyrgjq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vyewfpzi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3altmelmp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3arouebdu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bydamyxw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tsnnvomx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebomqhji.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svxzyvyo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dtbmzdew.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tswxtzkj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gwzxdmwc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uhjwmnzo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3svpnhfjw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3bnokiqlw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ozkfrdom.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wwevjwyr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngytcuuc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvthoktk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkigwodx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ozrvqpsk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3nuuyetoy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eppiqpsz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xgomvmhc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hrlrmffq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqibyvdl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3utenqxal.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zqsnamdj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fidfoknr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3omkydjqm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qlanlurq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gikufcmi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tqmppdkn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kvvxviwi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3rhhcsavf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nrlwjifc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bkcwtolx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xeerpglu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cuiodkze.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vwzwsgwk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xwwykmez.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jvftmqib.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3iieenjsj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hutijudi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3okylwblt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cwdurmfa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qfbzceyp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qwgtnvjt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yjwjqnvl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jztpzxjx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3iamgievu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wttudwaq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjngyvbi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xxtzyxpv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3eohdbzbo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nagpyxlu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xhdgojdq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vnaozbiz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3imahecoy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qkvjgpcs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fvozljqd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3idundcsx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qwdsrmpu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ghaowrry.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3quxakxgm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rwxgeyby.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3odhxfroo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wphhulls.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kzphiyjp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3psynhqzt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwanlhlm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwadqftw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ztzupzly.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuecxfzo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3smgovgvk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ovpvqyle.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mcytqrkv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wdannsxk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uhrsaoyz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aihccdvr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzbeccnn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qwdeegur.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcyknkjq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hrqzvhlb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rwokvmon.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3evodwuim.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3sgbloexy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3exrbnsxb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hhkdacqe.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fxptoilw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bgtpoqvq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vcdrtdti.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3astqipad.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3sysbjpih.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jgfvcuzq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ntjqtvbr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3pafxqbwe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3egnemqoy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3gmlaudut.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ygqcjcia.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bzmosgqz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kcncopkc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ncerqhky.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rzllulbg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3niiclwju.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3swwlzukf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3csbzdwba.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3esstwsfs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gruhrmhg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3iuacqref.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3lnyvnyxj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zhndvwuv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qfgytuwy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3wnnlyreq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wsscvdfk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gvpbskne.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ofxbbrib.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iikstfyu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vtdyotfr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ieheiczt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3cctgwlwh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kennlehb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwrrktrv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wkmppwks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucunqepb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3fwwrqeoz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bcecobjj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xwpjencx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdhwqnnz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfiizclw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3prcjpail.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3juobruex.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3lzmbuvvd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gqusobba.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xkwothks.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hcuwzdlz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3liinelre.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnmgxwlk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmshfsle.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fiojlnym.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jkjkvdvi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qkzsxaps.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3insswyzv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ctvxhroi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3nrhyuent.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ljnyytkn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3owxqmrdj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lwfbylpw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ahqvzllq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3qxqsqsdl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ujajqbgl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3czilhutg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3cjkpevhg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tfvebext.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qcedmbsb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3aovnqbct.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqxcvpkj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdhepxcl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tktgbbas.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3hobmouqc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxyauogy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bxsrtwbl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ucidrfim.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3uepuycrh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ybciraln.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bocvsrdq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3onczrxux.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3athlxshz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3xhdyvhpm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bwucikgu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jskbswip.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3dbiasyyv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3urimlnwy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3znwuctze.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tizvyrni.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3wemlzjxe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xzdmumgf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3xfkblkwe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ugatawoe.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ljdslwjz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3zqamulfh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nwevximk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mbrtzkeo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xyrdingp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zgtgdqaj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ytcfndxh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3nfawcqga.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nuhbxdtu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3rezmygzp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pdceycus.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3tmpjtdod.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3gfydeumq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qbmstggf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3meqdjjbc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qmljqbrp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3fhnjfzkc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wpbrhzeu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3qhdcltyb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kkvufgdp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lhvyaqcl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3drcjjdwe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3msfyucdb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3zugxmrmf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3uvpjrclh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xqmnywto.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3dgnquvbk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3aulncyzg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3utrtqjek.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ioszxoxt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jofiookt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3golkmmbt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3gkhnwwen.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3flziiujf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3mdikkfzp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kzzccafy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwnsqyht.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3jszlvlfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsyvgzay.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3vqrumbdv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3icyeqtqn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ygainwby.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kymooqde.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3bixvltpl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ygxurkqi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3qqpkreqz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hrvzelav.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3sxusqdvz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3tqwlmbpi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3losqnpzb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3torzjlnv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3bidtrfej.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zaxrqgqc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3gldhczzb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ipwmkmpu.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pkjrdyry.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3esdezkgq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3dypentvv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3guiwmvij.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3vrbymqpi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bxyufvgk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gkkkezwd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ltpvogam.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3pmkjiwtl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3afjyjjsl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3qlfnltbh.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xoeqsmhx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3hioyzgcm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hffsxcwa.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3sxhjpqpr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xjysqhcu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bxyulcjp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zzwfcvik.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3jvvqwput.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3chinbcvg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3uijsxoln.html


<!-- 参考信息 -->