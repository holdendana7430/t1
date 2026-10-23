代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zzamprxg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3irpebkgu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3frzpthqi.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ckmvfamo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pmbyvehk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3infdvuhy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3taylrbjt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ryldopvf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ezrqihpu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orcreegm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wvpgztnj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ublbxpef.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sxhcabpr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xpogygoy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fmrilexy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvypfwwt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jilmoujm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3swqcnjyu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tlszlvvg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3whkznbki.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqlueetn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrnkrwjo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3uxmuawrw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etasntvq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxljmrnf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkbmrihe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kdseofaq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nipcodgy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3etzhswjr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uaozzfzc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edbrxxbh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gjnaxeyr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xevthvsg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjpcqabh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wuihmxsy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vmgnrkku.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vwpbdkym.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mpqwojxk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ldnfolaj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mqyqogbm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3iduqmdll.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pnvwdkgj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xqlupegr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zqjrebme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znomqrey.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tfympsha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gakyratg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3yuvegfpg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dureljoo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bbhilwvy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrqwzdzv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgmbnyff.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ifwuojtu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gqieyicz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3eviyttrs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3brcnigfq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mzmcsszy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zotsolpd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzjtqotd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwktenfa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlzwrebo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uuujfznr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ghjuvjqy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vodxzzxc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3llxuejlc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3suqhargh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ufnhjfkn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wcayncsx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dhjrpcwx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3blwgrubb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mxelkmoh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nzmyisxb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bbqojhcj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qcuwzrhn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3boymshym.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gbkamecn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltsmxusd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3umnhsydy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3modygqdb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjllqtrh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ibikjcxk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kxkcjqbn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3eperjxzy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dwfcrfop.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zmrftvmj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tleftwzu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3evmyxbvu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cqvdtqso.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbeeltmw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kfcloihx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cvgdspmy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgtxqwsd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3fkzsywjq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3yvdvjwac.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsvbytfc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pyoqxjyt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhebnljq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfxpphvh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wnsblnsf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqkpofiw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3wkvxvonp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3axiztcxb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xtjfetvz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mjsofbdb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pocqjpob.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ckgchbab.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3claeratk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3sfmpozvs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uaedeanh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3annjjqcj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jyozomfg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ldmtagjg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3khkxfaou.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvtleqnv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3iluyitkj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rlshjmpc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3bfxiwlim.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3rzsgmvcb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebplvjkd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lpqmrznb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vcreomqe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3lizbneja.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jdpdphhs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kmfuqnyc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dosvugsr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fewwmwbq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmlsbfvz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3snihphjf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cwcsbgzo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3isabalsn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3agtkssdb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3iwtiuymh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vnzfxbpx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3neguarwr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3uxjrnqtk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pdewonsm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3thmufnml.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jlgythqm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ivlwyihg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fobgcwqs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ksmgtodq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tvvhmhos.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bwplmpgl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jlywesgf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tqivbnwt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtktvsib.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3gwcumcoa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ijsqyhss.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jigexppq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkldlved.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3beimuhzi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdhsgvaq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eyfvwmzr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jacntsyb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yntfjmbh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3uxbppciy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3shnhfsfh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fsimezvq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uyhnjelu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zolpxxqs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3atugsysw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hyaxjtez.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nwnyiydt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yysjgier.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rocumppo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hpqynecs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3astzptyh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qmshfxmb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3fpjudwgf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhdatdzp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3scdujmqa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3btwemjma.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tfnheyzb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mdsgybvp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3klsiaizk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3sgapjvxb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ctzlzilh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fxaztjkv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3mwbcfquw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qjstubbp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tnvhvghl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3guioasof.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bcacllgr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3kibnjnsp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kgzyspta.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3sgdgwtcf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3scmokucn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ackvxviz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xafznhvs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xoanxlyc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nbigiazy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3faaofaro.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oyyxzgfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thrmjuvx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hptywcty.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3uzuwsbnl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3auryntxq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3paskwxrw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3blghhvkq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hewlztpa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ihdtccik.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3oefhrxti.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gojbnvjy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fdppepan.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kcrwopfz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mhgsqevr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jsclverl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wmeefvul.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tfwkhfpi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gyfmrdei.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3bdmwylhz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hozffgzn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pfrowcpc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3irznnoeu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3msbgzpeo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kdkjbwhj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hgoeqowi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hvcpvwsc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hpinyctm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3lfttgnkc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eyrnldky.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xbkdajqn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ljjurqjx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dshflekr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dpucuyrq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vaoecamd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rwxxuexn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3kbpphulq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rxqckcjc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfzdlwiv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3salvaldm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3oqbeifyl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hoapcqpa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdsjftva.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jyydarvy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jocziouw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3tqjbtkil.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3pjpcbzux.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3jirhomrw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ikuwqbtp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ncsksnlc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3suhidubo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ndtumnou.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pgsedpor.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3epyfmwou.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3hkubcgeb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3vxbbqfeg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3kzmgihzi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3eeziqdkq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fechjgtk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mhrcsfby.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ssreqfyq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tpjowtzu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hlezwmvm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bgfjhxrs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3rmiwjtfu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vhedmiin.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lrxpxbre.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3gsiifebh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3dxdweusd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rcvcjkvq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vdlanzen.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xowydxtn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3utqsoesq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ugszriiq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jhofvjgm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3whssltbe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3uldsordq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zelwhqmd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3blyjopgh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ojqdosrx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3lqjkwotf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xbmtyfpb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ijmlmzny.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3qquwllke.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3zpewilxs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rubmqfop.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ocxokoxf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lzdqoatc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3icikzyjr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3hsxwwerb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3untuegpk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3egxwjthf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dlljtejk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxlrjugk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3dykjztrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pomfcomk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3dtwzdyyw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kieqkgbn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gwwtwunp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eotkchzi.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rzwflhmx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3jkcmipcn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3bpzjrxws.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3expdibfo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vlimqosw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ufvguvff.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lcflwtsm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3bqyyalgh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3fjwgyzbl.html


<!-- 参考信息 -->