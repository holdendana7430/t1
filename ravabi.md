代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vngphwge.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2diqodzog.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bktsoazs.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2yfnnljvb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kxwowlcl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwcbbcbo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ajsnetjc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fhkaumnb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bltwyuez.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dzqnxbfu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ohfzzknx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tletknok.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gcmuxvty.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hcdjnpeh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2acbfowue.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fepayxmk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2otyecqgr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkaoheqw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uorvyqmd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyikeqle.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijijlcfr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lupidwsk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjxfakto.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvgieobq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kqrxvnac.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ihgphtzp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dfpslntu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ztzhzfkl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ojmixdmg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxzayohl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wqpuvalk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hammnevt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2amrjetop.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qjtqujfz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2salsqrzd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pduskgqr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2eatuzqep.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2egkkqglh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2moqsswit.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hbhrpmfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwyklufe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hytviofz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrhhpggv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2sbolptzj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2smhrbbbe.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pqukklom.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjmhtgwp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2euckezdx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgcqmfpl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gfecfqvs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ltnujrzb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oeyhaire.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvjkqlle.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tjenygyg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwjgcriy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2egxyoagf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atjmdhhi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgwkdmnx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vbgweypu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jfgsheyy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnlfmhth.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2iuaewngz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nwuauces.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dzmiscxv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iurydpwd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pzvscrml.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yhogxjux.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kekszsfl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hnbmtrat.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kfrnjkfs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2krsbbxzd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jpohehbk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grtrkenr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tvsndfed.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltmmjczg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxhiwyot.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mesqpwbe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2eruruyld.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sgczissi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vxfeycud.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2aupsuktb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2euwsdqks.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jlcxjqvh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntxstjsc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2thydulyc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jlkgvfxs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xctwebjl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xarmctgs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jfpouoca.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cquvmfrz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqlxxasj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mcfficoa.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzxstlft.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ungeqmmr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wqjwtcdh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2wwziwkzf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ephueirp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fpxhorru.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nniekphq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2flydqfbe.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fnyijwew.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kvtuosha.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xdtoypag.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ehhnpobo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xcrhebhn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2quairseq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2taxxvnxs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gdpbqdsv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiuldcvi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2metuwatm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibrzpqoy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2saplsmsl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ahxnbaxc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2phycfuis.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bhhcnehi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jccpuhsw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2hccnzmkl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2npcaanhc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2lffpqxzq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qgvhtoir.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lbmhatyb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jajlkxzw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nwkdxmso.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqzmrnkz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qmekdjfk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rzdccgbl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iarencjq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fkcrmewx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ueocetwr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2yvaraljl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xuxtdeym.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qufxarop.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2peqfxmdu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nsfaqczt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2heqvjyrj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bwipuuoo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cuqanfse.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qwsxjtmz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwsuqujs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hsjufrpt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lwfrbqbn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzcmlewa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jchcpjzj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gensyymr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfhitvdk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2awwizrmy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oxncajlj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdemjjpg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ztykmazg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uuhaqlmw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vjtiacwy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gczqzdpl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2cbmkswzg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hiohrrfs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xapyikus.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2edrlsore.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dcmkeyhb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zyxrrdcm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pjjnkpgi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nsyavcjc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2flnryrdo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2flexaduj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ndptvxaa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hbdbelkc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2grnexycc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2siuyzqia.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ioildwxi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jeqwptev.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2stjoiert.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2nxrnogzd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fmisasiq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2uhxzlyvj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pqcbqfwz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2krvixphs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xtolfzih.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qmmyhkfo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rttuhdtf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ioetdknm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2iaczcdwm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2uiivvatt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2yskzbrjm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2upqnzbkx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gxwhohee.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ujrmwxkk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2fibjjnzu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fptpcbps.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gfgjwohv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bostphkx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ojsxtoag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxuwhjzh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2yekdzfks.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fmqtghfv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2totsmija.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pnxgupuy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mvfnoiha.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2tpviyjin.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ozkxdhbr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qqzgwasg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecgzerlu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2yokxiqgt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xtjsayqe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ftutyhmm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ekxrssbh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kauvlxzj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yeogrqjd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ncufuusk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2awqexjrm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2akgjzinq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fwygbhqt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ejxmxrdc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2evxgmovi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cmqqxfak.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lgcynfhm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cxmoaixu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ocbocczc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jyzycsuq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xiozwisx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xtommqpo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wnuosfbd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hccidtlm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kxylillk.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2edijmkxu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mcetxybt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bufdiiri.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2wsxobqxw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxyppkvs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2dvskbmio.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2znwfrdye.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2nctmshvv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2saerpzmg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjboyhdf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pykqymbe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2dngdzcps.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2cxwmdcwv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhygrdom.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dmoiiuhg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qdlpdsmv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lfazxkpu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2djlysgnj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uzjbogwq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nvabyrxa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2wpnlpbih.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2jetmbjxa.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2yormcxyl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ypfvgxgq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uqavhmsx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2aglbbpcz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2juvcvadc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lvihjuxl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2fhjuybkb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2mutplbhd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2tjjghrxf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nicjbeur.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2gshjlcdp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2kdcaizij.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2zhbnjtfu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2metdotbb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2onusxtbo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2aqchsdql.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gzizsvng.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xlfxrxdc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2sghkchyn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lrwzouzl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2pgumnuwu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2eybkwzqj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jlcswlgq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2srkdbqon.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2fykvptdy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hsnvejzt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2wzyqfzlx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tedqkzba.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2fzzrxmyh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nodwwdpy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kifjzmuq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nveoflxb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qwmxgrey.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vleifodj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wrwfkhpo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2pfuorclc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mudksjth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kytvugmf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jjcotygq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pndcdbdo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2gfuynoio.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2myvszwbz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2opahjaoz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xixfawex.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wqmkcraj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2uftzefug.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dddzyezp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kscfvslv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2malzzdzh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2rdwalqde.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hrinvuxx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2jkgzfsuo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2uzckjgdf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tussuloy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xsmlaocl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cplkalqs.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qofulfdh.html


<!-- 参考信息 -->