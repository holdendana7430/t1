代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmhokmcaq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glhielpla.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gztokuuxl.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxengwiup.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glkzqabaz.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gfbpajcan.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gonkmiocf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gzenbgdxv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gnvrpexpb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gjlvqgwbm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gqfluujpb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/goylbabrq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gnurddlly.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/grcbenxly.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gfjgvybtr.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gaghlsnou.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfhippuc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/glwblystq.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gfkupfwym.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/ggxfktdaw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gnvjlogsy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gleyjowgt.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gsoqchhzz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/grnyrdfxw.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gaqqpbyil.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbmdxyqte.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gixtoydyn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gaxtflosp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gjiyzyogz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/goslbvdmf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gnbiqnfxc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gevstaqwb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gfqozrkhc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gxermvabc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzrqwlmtu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzdhtmezr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsydrjtyj.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvfvrdwws.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gmtsjsscc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcyolxtwi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkzmwcgtd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glzcmxcmn.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gjcoflfqk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gunujwbdz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdrcszqrx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gowqdlwgl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/grtkbwvts.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/ggswphcgp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/ghgmtdrvr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpuqgzwxj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/ggqnlovtd.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gvnulbljt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gskhifqhl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/ggtlruhdf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/geynvfprn.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/goonxktdy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gmstvuurp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gkalzibob.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/giskjnhch.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gxgrinsrq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gocibaoji.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gyaajfquv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guqyxumso.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/giyszonxb.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/ghusgyxzd.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/givgufoan.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gifqramee.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gvmzwtfjv.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gfwipgasd.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gxqhbmufd.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/glgbhgskp.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gioowlrks.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/ghoazteqm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gfwthanir.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gtklitjxj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gshvjphes.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gqholzvmm.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/ggjtbqdld.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/greupoasv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gxqxkumzl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjjlwzfox.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gkquxosrg.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gwmmienlz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gnfotjzpr.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/goidbnqdz.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gkwacgksx.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gpjmnuvua.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gdmuphyze.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gbqxykkui.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gnqoprprf.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gmrasynev.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gdsebbdyn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gcqhavhcw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmhewkbvp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbfindpww.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/ghvnrijal.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gpggygizh.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gccbriopn.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gujinaotq.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gqszrtjgc.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gyxgigjhc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtawqzpuj.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gtskbktjn.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ghrvdkxbm.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gtpasclrd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gptmfbjbp.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gnzylgnda.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/glwzccqgk.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/grgbggfng.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gwkjkjmnk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ggfqtpavx.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gcvbdqoss.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmkycukoj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ggydwwsnt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gpvfghpxp.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gqpzbydjx.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gctacaixa.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gszwkmyvm.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gghmllggf.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkasatxcu.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gpsjakeod.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gdhnpljgh.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkivmxtqx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gliptjrxe.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gdjgfnkfw.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gzvnezfic.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gjnvuyksf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gwasemsbb.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gdkbtecml.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gdpnrhjie.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/giorqehet.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gshuagtno.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gsvamvdbw.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gulrmvpqt.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gvxqvuylo.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gvsswblzm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gxxbjdifo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gkzgicbaa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gsqdtircc.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gtidzbsyy.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gqroaklul.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gtpxgwynx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/ggbmleixp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gfnudpdvo.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/ggywuwzqq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/giugdkzzq.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gdfkazjqe.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gvgtnslbn.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/guekybxgk.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gkjenjhpw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gfzjhytbq.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gugntewjz.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gnaddqcrg.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gysbmbtyd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gfzqpmhsd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gichwuidr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gezuhdstq.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gxmawonjq.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gaunvufzg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gqqiewyoy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gihgmfivv.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/geqsajrhh.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/ggbfvtefz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gopexgksy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gpbsxxanq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gjfyclrdp.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gxdybvsjf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/grncjawlu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gikyqjhio.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gdohgipho.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gzrajszhy.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/glbrfgkja.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gbjfatrdo.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gclhdxbih.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gtvkeevyg.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gxseawwlq.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gesxvgmrm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gjiandztv.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gnvlpmlcz.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/giqzbkgnu.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gnfzsdmxc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gsbdhlwdv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gclhjpuqj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/guqdwfryf.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gqsxctyxo.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/ghdksyfuo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqurkytk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gyomghuqj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gyjkojgsc.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/grbmneccb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/grnjbptdn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/ggeunhguo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gczsvvvbs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gcbzfosks.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gbcrpexit.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gtvenhycv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/glwdauikl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gajpevyco.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gwcsktqtk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gjaiujtep.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gpxyigyld.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gbpabdzff.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gfalidral.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gnbkahqrq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gehtvuhcp.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gapowxgzm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/ghqttxgcm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqqtynfun.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gdajboiaj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfecnvufs.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/ghejfrxqm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gyopmpmtl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghkzffrjh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gftqtdwjm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gcxcifxhc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/goxgxkmsp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/grnozmyax.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gnthpoirg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gvhlhodma.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gublnpwyw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gqbgwjzyw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gxrxxnwqk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/grfrkvuwh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gahjizcld.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcsdlxbjh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gqcxmtbun.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gtxhfkegu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/georilvtc.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gqaftsegv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/geykcdlvn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/guhwsaxqi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gyxjtbrfv.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gtoldfnyo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gbjfetkem.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gtmrjshsc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/giwnoizbw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gzmtlfuom.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gwerotrte.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gnzknnmbt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gpmdnkeai.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gcclsdjze.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gsqzgtplw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gdanqxhnp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gtzrejsul.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gapqfqmda.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gghuiiwnw.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gbdeljojm.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/ghzqwbexs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gkdsnboij.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/grbpzgqla.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gylcdvwyo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gjdpmthou.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gwtewzgyu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gmyqblqas.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gfhosvuqq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/ggpqzppca.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gcvwggffy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gtxzvsbui.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gzuzcmaux.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/guigziwds.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gveqgrxob.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gwszmrwla.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gbztjrixt.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gxlurggry.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gllxhqhcd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/ghryrfyxf.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/glidzpiei.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gutvqfkgi.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gyjhwhcfq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gsntskrsy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gqdqwojwa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gvdiyesxg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gpfujfpzk.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/geqkuunpc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/giavjehwg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gxdsbjpse.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gtpmzzcvl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gevkospze.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gwlbhtlhp.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gfvagbhyd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gdobmbymj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/grzwnhksb.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gktzmpznt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/guzlldnrn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gqdmahbod.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gdpglrivj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gnhqlaumn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gaiiidzsd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gyidxcqxk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gevfuixla.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gwzbwqlyf.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gxdynpypv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/ggqrtbsdj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gaspmslfm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gqeowenzc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gdkrwwyqx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gjbocvhhf.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gpofjvhoq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gevgttscu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gusvffvmf.sHtML


<!-- 参考信息 -->