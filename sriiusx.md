代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gqylufvsb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfsrqlvyz.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gkjtnovon.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gkcfvekez.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gefmvjhsg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsfdhtszi.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ggqfvbddt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/geqwkdjui.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gbkeeqtyn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gxvklivwu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gomqvhnlv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gywosuuuf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gpqqunggh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/ggkrvcaun.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grkcwwkus.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxpsgppkz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/guawwmoxv.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcknshbvy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gearwkyow.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glpjbuaoe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/giisgazec.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/godtorifi.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gjjtxeuus.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gixvbbdqj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gnibmzzer.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gepigdqwv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/ggghmhgdl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gmymiqswk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gypolshqr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gadrsitfj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/grtatozim.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gfqwzryqm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/guotwingy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gwaspqker.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gpgkyfsxm.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gxtovrraq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/ghfhmkuvv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gyhdmfggs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gbbkuuklw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gmlbxdbpz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcmtfoqgz.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gwmsvbggr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gigkkvilr.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gricxmnxk.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gynsoubmt.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/grqejwrhc.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gwdqerfda.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/ghcakooki.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gyfkcccab.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gmwkwvtjg.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gwtnssmms.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtnrvkesx.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/galbxuhtu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gkwqjhbtg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxioteqeh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/ggaebvlkb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gzgeqypez.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gofoiyvrw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gvycliupp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gnpxnwisf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gvoxxjwvv.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/goneyhwcx.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gqofavoxu.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/ggadxjmge.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gsecpieif.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gitumtnvc.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghuaciyps.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gqyjwujbj.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gzuacksvp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gidqdlgfm.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/grcyelsbn.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gqcurtypc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gyfdfkzac.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gewfuckam.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gkatemohp.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkmtaverv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gsihduuxp.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gjszhumgw.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/grjumlxrd.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gifkkqiur.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gsjdbyucw.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/grrbrexhu.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtjarvvuw.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzozninwz.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gryvshzul.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gefxchccz.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gxgzzsans.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gdxrwvarx.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gbfezfuwh.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gptlfwlnw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/grmjxqboq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gegxnejtj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ghdolwujj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gdpxxiadb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/ghfapbwsl.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gudcpdtsh.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gpkllcivm.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gwibqvbko.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gsswlnfxu.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/glpmbmmrk.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gfglfqadp.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/ghepihzzn.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gdaulvbbm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gsxooukji.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/ghqhbfqxd.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gjbrqerpq.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gvwuvtdtn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gburrprgs.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gaviapvuw.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/ghirfkccm.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpytimidz.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gvrmgbbji.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gflimfwvs.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gpumcdhkn.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gbbeyjdgl.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gnvcsymre.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gdxbwjvvx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gbrvpbirm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gczynehtd.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gxetyhevg.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gmkcupbef.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gefihrcne.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/giwoecwig.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/glbhaowpz.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/govdoduxz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gdhvmluvx.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxwudqjac.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gsrozqtzc.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gcgbtomri.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gxhqkbmzp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gbjkcghtw.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxpurjehp.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gujrgefjt.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/govlalmkj.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gigdssahc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/giufqajwo.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gghbthbiw.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/geqrjttsm.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gdjkcjczp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/grlcbwgyi.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/giqswmjhl.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gtlvclkad.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gvenjegca.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gclvptuox.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gosejbihb.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ggmfghhsb.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ghrlaturm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/ghjboodad.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gjclmnvop.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/ghzxuncsu.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gdyggygrl.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gnuwiqbye.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gfxnchtyy.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gsgblvjyh.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gwuzvvvho.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gbmsysxtm.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/grnadhhyk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gibhwcdhj.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gjrckgxzb.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gcqnailhi.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gfrixmhvk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gmjqcriki.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gmyfwjnac.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gqzahwfjg.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/guedkexnv.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gzsmcclzc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gfceamvpw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gnpgiihcl.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gbwsbjpye.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gqslddecy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gvfgzbmmb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gylfuzwbj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gpjdeyugi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gpmhxqwtg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/ghlknclag.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gepkgjhym.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/goegncilg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gatafsemi.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gkpweaogj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gkqpcdkee.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gtilbwdbz.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjlzawhby.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/grqpamrsf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gmrqhnwxz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/ganvhmfem.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gchxlckyt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gyvhxjrpu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gptkixxhb.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gpexreqqd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guljrxynh.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gpntrnnle.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gaykhrnkc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/giqsaooak.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/grhkamsfk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gsbdogpnv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gultcusjc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gsmswxjxg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/grsoawlne.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gmgoxknhs.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gxrtkfepz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gcmesukvp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gaxtrhuti.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/grcnmjyqw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gsrvevdul.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gluhyzptx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gvlebpsiz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gtbozpuln.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gxtshbncv.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/ggqketqdr.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gewignzlp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gpqsfpisy.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gbwkbqwjn.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gpibqzlhn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gzyldhzde.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gkdqhzoge.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gbqwkslro.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/grhphxdea.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gmgnjqylb.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gxxinruyz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/grcvxittj.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gcokgtsyy.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/grarnlwug.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/ggkcgomhz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gpsulhvgh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/glwrpadaj.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gbpvxvcki.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gzkzeerlt.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gztprmlas.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/grwazkvcj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqbxheksn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gmskadlcq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkstistuo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gmhvqmktm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gvabkvrqj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gohkigozn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/goxtjecsq.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/giruosgae.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gwnvrtfbl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gbhoqqanr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gasmiyozz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gzfsisbpj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gwsyqvkpu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnnxekcn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gohjjhmgx.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gvggqpcuu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gaeqabthm.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpflzvncm.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gpbziptoi.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/goyqcfiff.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gxkxbmjdu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gkvlotanq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gglmqvsfw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gkgofipic.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gwrxzldfv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gvakzfpfb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/goyhnlbuf.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gednrlplc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gizcwmfnm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gdxtghvfy.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gaoinoskz.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gooekzdpv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/ghexalwin.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gryqwlsxd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/geptpscjt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gwrwpwubn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gatavdrui.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gvdkqtyid.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/ghnpfmmej.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gfluhzgmr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gazhzbanr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gprichfkq.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gqygowped.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/gaabtceyp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gvxustjdl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gqjehoxrv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/ghnlgodrg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gyepgcxln.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/goxqkdnsl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gjcsevqrv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghghaaihz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geranysjd.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gxqjbslut.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjwwkxpef.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gyumqkxyd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gfjjoyeox.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxyrefqta.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gdssklbvh.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/glinwacuo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gidjsrknx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gxlmofnpg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/grfoxwxys.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gcngyhxcw.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gnupshajl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gwtymtrxg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/ggszboiba.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gueihpxux.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/ghofjnefg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/ggpylbauc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gyvhxhieo.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gzkltmirp.sHtML


<!-- 参考信息 -->