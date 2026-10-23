代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zpoxqtaa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3krmvdtqv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ckyvwdom.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lmdkeity.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3oembanfs.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khgzestw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kukyfkyl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cprxmlxy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fhphhvwi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pfxqdaya.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gfwexitj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tpjiczea.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hvwttlds.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wepkhkqm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxiztbjx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ancsgyxo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwxvligr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qodsndjl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kvagoqje.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eocnxdcx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nrvlntfz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3epvqshfj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbtjfbqu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azfwienz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akefyxbd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbmkatzn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tezafjiy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ebfeuqww.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3kqqumevq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zyufswnf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pztknyyx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3oykyxcli.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xjoabzrn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tmmnojrc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fvohargu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3segblynh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ypqhipve.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vdvwjsuj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3llpwmbaz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3slzobiwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3domafmit.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gkgunkug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsmwhimq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kccmopbz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3puvyxopm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zpebjnbz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dckgfalr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpcrqvxq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3vvpptaxj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hsxymgow.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dfxcjdlm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3amztnkan.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3esygzbpd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tzffdihr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3spjnscna.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3isqudmhx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwnmgvhn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmscuaib.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3scjyhoxz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dcqnmmvw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ixlfjpuv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jvozhhwh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ffeldqvv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3krwxwzdv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ozxrwkqv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ewuxzqdx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wvoiekoh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3laztncvl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3grqgeeqy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ycrkbnyq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yxlwpewm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rrlhhghp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nbkgxrtg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3swyuuuvj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgnhlyxe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkeebfan.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xzrdtdow.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3toxjmvdz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3furlafax.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xdotwdmg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3fdwibunz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hnfzwqxw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbjivupy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ubufpoxa.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ucyngbev.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rbjwseha.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zmmjnyuh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkwiqame.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kncjsmok.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ehxbsyup.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yclnwjps.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnueclcv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gedejirx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zdynmemf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3pczjrhea.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzvdziig.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jozrtfen.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3yzoqwcii.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3tdsujyjc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rpqaneeo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ujhrufzz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xjxnayjh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aalngebt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3dmfbennp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xfsbylgx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xdkeiehw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3zfymuxow.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ttfbsvsl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3swimjazi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3uvoynmsz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqejqahb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqlttllw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3obqkberd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3exbipstg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mekijvbx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3akbizcsv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3artmkdag.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3shjvnbcg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kagplwat.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3axfeqdxo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wlhchxiu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gqdnlcps.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ythmqxnx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnblcyls.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3pklcwivd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lxebgkxn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3klxvskwd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lybrwhdm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mnsaybes.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3iavvzjmx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3extimdgl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ffqkuuxn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ecemcnft.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3mcoyhmcp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pnhplfzn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oktfdqmf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnqlwjvw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rwuypnnt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3srydrswx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qglxbdef.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cnapqver.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sdoxfiyw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cksotkqn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ikawtwah.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nukkpsze.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xubczyyc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3butvubpd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fshbiypu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tvyiicix.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dixhdvsa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ssdqrxox.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mnccwwqe.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xlbwbiru.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rgzkmovj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rqwcgatq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3htqvrqsa.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xppjtylx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tmnkdhor.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qhfbavxu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3oyibijaq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tmrltbgi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ipeltmuc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ixupephm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3sudcbqos.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zllmhhxt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbsrjabt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3rukgfara.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3emyrufgq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3avhgbrtb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ggfjoive.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dyxxwjnu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dffpdinr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3tigqdgwl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tfcmpiyb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3knpfpddc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tkzjtlls.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ouypdvmu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ymmxffjc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3rbmzamvf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iimlklcw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wagxqvrb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pepuphdk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kjhuogou.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xwkjozkj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3sjdceqgm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rbznhtcy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3feqyyyjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlllfvef.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ofkyglnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynvfhcbf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qbsfupxq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3shizrdmr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwfvvydd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ashyiazo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjzvtgmq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qtywdxmx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3hwesrico.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vvopiefj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rzwjiboj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3gsujakxe.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3zenqiffv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbwbhfjv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3njznqibz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrujkhhe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yjdambrc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3vsmkurdf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3nomjvgld.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sqqgtyxd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3olkskizu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ciyynmoy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vutncglj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bafffvpf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xpuinjjp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yynlqyre.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tmzdxwkp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3aqynqlfc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3idqnqqdb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gdylfumb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pbwidwqi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdhffqhr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rixssfmn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxnwfejy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjrapiur.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3drogvybo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ousmktme.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbainvfr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3elmzcfsm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3nncjecup.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yfdnozgc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvlmsbsp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmzdznfp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3saykigbq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3avohevty.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3onxlijup.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjwrydyb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3fdzdelww.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3bbdjjrxm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gckiohgo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qasffkti.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xxmcopdi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3wmanpvmu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3acitphtx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3gypivpke.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qhkurmrh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3acnqnuhu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xjtcbffp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kcqekegx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3twajuuzr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rjiryrqi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3huhcuvmv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pkhdfrzj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ainambbj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bvbhsavm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3nwwvlawd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3eprvllvz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3knxahahe.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vydwrpdo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3uhlwfukb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3nvchfnnb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qdotfcyl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3wxosrlzk.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3kjtddfsn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mciskjzy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3hcndcyys.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ejyyeebg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qsdrnyis.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ftnodsko.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3pigesrcs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3whdbpets.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3nwikwnqx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3casvfwbk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3cvpeutdz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pqpbvaxx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3pemmvsrq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ztupnlit.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3sgxkpfpd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ilzijmly.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3gddveiau.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3jhgpeeau.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3chffkuvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngcdnatz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qnwsnxiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwzjwlzt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3qyzvtohq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qerpfmke.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dhxfliyz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tfhlbssm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tfpwykbc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qysgnkgp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3samuyanv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3doaxmsvu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dczphjwo.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3jvqjohpq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jvwluldi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3nlixtoul.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3sybrtdzp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vootzbww.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3cukaomia.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhjdhfpe.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lmfqcyeg.html


<!-- 参考信息 -->