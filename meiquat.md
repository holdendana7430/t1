代发 wailian999

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gitgkhaoc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glfywcxem.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyscxjcmz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gvutbbymt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gbtsqwopz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ghftaqlkt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gztwywrnt.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxeyczmwe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/glaaqvwpy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gspnmlzcz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gppnwmwvk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqwzinpxe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdrfyikuz.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggtlxtoto.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/guspfusba.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbqwftiaq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnvltcspl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggdkxfvhv.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gjhyjkogu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gipdoykav.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdqwvcyfc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gufigxeyw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gbbzbfmtw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gvsenwqko.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gyvrrwxip.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdqlbhrak.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/griacyhba.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gxzcxymdr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gbglvobul.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gatozrxpf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/ghfsxngll.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gezhhqglp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gsxpbxatb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gycfbdxgg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gmgvollra.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/grmxsmmym.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/givmpuhrd.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gmyupacwp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxkyjkajf.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gwlyuugcp.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gqsgnzkcm.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpohuoyra.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ghcmfewpn.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gkigirokg.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gvsamhbim.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/guvhredxr.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/giebrkzjc.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqacdbuji.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gbscypagx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gdyrrronq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gvrdjtihj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/ggkpzfcqc.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gtourkidj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gsljskxul.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gmgcclmti.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gjlcslkxc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gaqyhwfwp.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gugpvvinp.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gastmdbnb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gueignent.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ggsmkxvdf.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/goheaskfv.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gwadijaxq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gmzzrqbaj.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/grlgptpol.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gsludopan.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gzcwacadq.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gsaoamahv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gpbfcbetj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gmlynddmx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gocydeoas.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gjyrlbfmd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ggjgtqqld.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gscvpulac.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjgkqxxhx.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/goxgadbkt.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gprmepfyp.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gkxmhsabr.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gqrbfkqbx.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gzctfvukm.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gnsxwowmf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gxyfzuqhn.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gvdckwohy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmnqsdhuc.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gallpxvvu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/guaumgjxn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gyiseapsp.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/grnvyfwzb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/guhuetgnp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gzoidigyu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gxoucyxfu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/ghgqetbma.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gyspbhxmp.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gpjdoongw.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gzghvlwil.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gqjrazpou.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gzdfocfam.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gpzuutbdq.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gmxktxwik.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gccgacbnx.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gpziounsr.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/guvmrmppm.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gfxuaoedd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gboehxmvt.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gbntvvzbv.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gjbcbskcf.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gdjwhfoyv.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gnfkaouty.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/grwqcmmpe.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/giidacvwk.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gwwqamvmd.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gntirwhej.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/giuskooio.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gtqdpkvmj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gxuowxtjp.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gdmlqgjdo.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcortjbvk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/govehkssv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/grbtwkoxe.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gtidfgitp.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gpzdzyvhk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gfgjnxhre.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gekslogmt.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gsqvzelul.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ghmmrassl.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/ggoqqtylx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gyftrfmwd.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gujaylohd.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gvoodzovu.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gouytcsdo.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gjgeqybip.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gbzrqhgkt.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gtczaxdlq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gfpyggdyp.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gzxbpuind.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gqaaampta.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gpulruthf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gaqkzvjbr.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gkmlqjlxv.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gbztyijyp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/glrbkpfim.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gbwdhihsj.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnffawuzg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grtoiouir.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/ggikxfvsp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gvknqmtry.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/goaqoqaoa.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/geyqjrnqo.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gyzntcxex.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gsxlxwmnv.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gdgcvirik.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gdsadyxta.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gfnsbtfpl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gwzhnrcbr.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gmngrjxbf.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/giucbcrtl.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/grfohiype.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gizcgrzhf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gcmomcqlj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gnufrporq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gsjnoaewa.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkbdakqle.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gqbebdrth.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/grctubhww.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/ggksdpyld.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gaipdimnx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gtujmfqxd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/grrnetvwr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gxgjxikgx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/ghqjhebte.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gxrwroqwc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gdhpjpdib.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gjdyzgqab.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gtuarrklb.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gdxtzjbbm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gudjjavzd.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gbdmkswgj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gxmzzgila.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/goqggradw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gobebrofv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/geumpztry.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/guhodista.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gsemwhyvv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giememagy.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gwhpduhgu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnwabitks.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gmpzydkhk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/glflwkumx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/godmbjpra.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gshuixjdh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/glsupdkmi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gyfnmxfpt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/ggrbahydj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gpohjbllq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gzylbtqag.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/ginlctuth.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gyohmnujv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/glrxvjzjy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gwiwhraxc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gdyjzodox.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gmpnmxvjv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gmpsyuyoz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/ghyxynyam.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gzwjmojkc.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gnujgamoj.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gihgnauvj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gkjlmmkxm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gnavcaxoe.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gtdffnqjg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzedydmib.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gkugvelkx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gbjqfgejf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmbleeqzg.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gyiielicf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gvneyhyon.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/giiwflejq.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gsisswweu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gcilqjjwp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gqhuhfsta.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gfbiieiov.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gflxzdfjo.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gjjlunzsm.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gizzecfmj.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gcdxwyxih.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gprlgaoid.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gelcgloqb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gxmjraplp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gfgmxppmj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/glklnvjtd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gvbpvcmob.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/guthhpdck.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gisgmhmnl.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/ghhhbdwpo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gnahrvano.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gocabdvkd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gqteeyjnl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gvmvsdxmx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gibnfuyju.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gdcmvgnpm.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gofyvmurq.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/glrmrkfvp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gcgzatour.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/ginokszfk.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/guwnubitj.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gojypccex.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gztaamgao.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/ggrxntkym.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gummayouw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gttxkxori.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gxwcyczoh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/ghcmjcxzd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gffqtvcuz.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gqaapdoqy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gjdqeqlmo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gjtfnfxhf.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gidqwfpga.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gxkrrkvzf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gnjbznrrz.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gwqdbwtcj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/giquethnj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gfoxnmrup.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gviisyxfl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/groiasynu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gqxyhfvte.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/guhaacgut.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gfephslru.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gfgonkfyg.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/geebhrlxz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gypjsodee.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gybxkpzyr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gsiidufzc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gvdqllxvw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gztyucruu.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gnfsewlyl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gsafnftlf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/glilxriqo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkfxiouya.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gavxxabdb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gacmgczkr.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gvlbiivvr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gjndktxgw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gecvhkrej.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gtiicetqq.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gvykbohyo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/ggknwwoqo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/giwuhymtb.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gdotyikon.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gpfqzbexb.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gsnrhrgnu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/ghdncmxgr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/glsltlzcd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/grnvgkfqc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gvhgrabyb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/glfphfrtk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gyzoweiqu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gbyqnyvpz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gtekpyvgg.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gjfbufvus.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gcatrjctc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gcxprjyqr.sHtML


<!-- 参考信息 -->