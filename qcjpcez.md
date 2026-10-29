代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gviwwuhgs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvvbqkxvd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gudzhnero.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gthksrwwg.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxkkyeefm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbwrfkqje.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gfjbsannj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gjbrdgidi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gizwgcxep.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gyqupopco.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/ggkldcxkn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/ggsglqxhb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gsyfqwlkw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gilvbwetv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gzgmeenmu.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gyhdmgval.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gsmmbojlq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gzeuyywae.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gbagbwzxt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gvnersgoq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gnzvnwgtr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gmzxunbzs.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gujiprmre.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gilfxuswr.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gleumcods.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjzelmlha.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gpixdymhz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/glkjpttic.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gcxfmilqx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gljksqhij.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gbmqeomyf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpgcemypi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gfmudewvu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gcaimauvb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzjlcivvf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gzlsablpe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ghtxtuevb.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gaiadgcft.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gvrbfmrgc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gplrmawzm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxpylnsaw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqpsgnzmc.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gzlihlgct.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbmvdpzxg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gszsjocpn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmesxubzj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gumpynlcc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gaidwnvft.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gaifsbgok.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/girfhmqtf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/grgciaxzh.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/goxicqxro.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/ghfklhnqo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gmvgndqcs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/githbgnhu.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gjhemdohw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gxwwlgoen.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gnsrmtonf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gjrepnhfg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/giqrvaabp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjnvnatis.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gsbzbmroo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gebljfpxp.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gdxhigsyw.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gcnrvecns.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/goblupsts.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gxgcnefwa.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gjtcslbuc.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gpqoarmlx.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/grfkqlhep.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/ghlhrhoxe.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gubdvevrb.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gvbupbizm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gpoiepjte.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gyfrtahyh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggobvueeo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gspjoflfo.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gjrkbbvpn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gimswnzew.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gkkiilapa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gbczfouwo.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gkuhmcfdj.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gdfxqcfvi.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gvzlzabsk.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gdromtykw.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gimexbxek.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gljhubhsz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gfqqkqemv.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gddpqxxqc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/geehboxke.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gucrwenly.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gixyehsia.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gijdncyut.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gowokkjhi.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gdftygoxj.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gfdasbqsr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gsubixpml.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/glhhwbghy.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gacmjxrxe.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gekfcouxy.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/guylozufy.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gkpvvdddc.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gthckkank.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gntmflhfe.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/geefjdvyr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/ggkrasbhq.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gtzxsrgnp.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/grazcjcnw.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/grkkbjcfe.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/ggytznram.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gkupveqtd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghqgconcd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gffxowuwk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gumowfhid.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gllufabcg.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gafvluttz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/ggevolvxn.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gfezuxirp.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/guxpqpbqt.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gbkbkbvlp.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwbtaytai.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gmblnmzhn.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gokvrmbox.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gngekibsm.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gzwulknpj.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/glzdohqfk.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gcefirkjj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/ggedwvaqs.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gikvlozsz.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gchkbiwjo.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gdytvjslw.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gywoacpmq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gcruhuqjc.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/getdihsck.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gbieevxec.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gcoelgzfp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gturigfwi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/groxkgctq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gmltolexb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gaqfhhuxb.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmwxqkyqp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gfxiijzpn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gutcpdxsg.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gbmbircvh.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/guwoliihr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gusdazqlc.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gurfbshee.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/guygujibp.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gcalwfogq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gnwjlxuuo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gxoikzvlz.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjfclnyvo.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gsouuvjna.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gbfkggujd.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/ggapirarg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gmlduqhrf.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gbjfvohyz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gmspkntju.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghotukdmu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxfwtxwru.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gbqconyup.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gdalwcqyp.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gseujmftn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/glgykvrgp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gezprjyde.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gpitxctwq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gygqrukod.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnbshaqae.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gcagctmgz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gttsrmpkg.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gavrtksfq.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gvvgahsix.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/ggxrmzgxd.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkghaubwc.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjpmmjhso.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gcpolhicr.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gkzhvysht.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gqidtkzaa.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gxlqfujic.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/goxglueqf.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gbnkjjfxp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gmxnejvxx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gomplepqb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gxyisevha.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gcxdieofg.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gtfxyyevo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gntdjuqlv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/glimjzpff.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gfmydcurj.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/ghpggmgzc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gftclqpyl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjnhhgqwd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gggddfdtk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtfyfifbw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gkashrwlc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/golyrjokh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gradjfgmt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gjvhynpnm.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gywouaynl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/glmbbqkxs.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gcafsjsln.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gafaggdup.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbfrgwqwp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gtldwywkw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gxwufgwpu.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gnbnrnqjw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gsrjmxcrf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggzsrzgox.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gqyflmvym.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gerdewgxc.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gmxebntoj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gbgdxmgdc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gwujlvpdo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gbsbdpnyw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gxfehvtsp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gweduzhms.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/grcebpqvs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/ggmkdexfq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gfbhgbozn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gxekhnjfk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gdruqgizp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gjqizegnf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdylevqdz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gfhlzxczk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/garcfnefr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gfhfnazzs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gagervsuz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/geuhmbngy.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gvkhriaks.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/girpwljtl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/givddgokf.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gezrrlebi.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqarkdjki.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gbqgtdvkv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gaygbcrki.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gjeqwwiml.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gechmrynj.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gjakmcxtn.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gdjlbbvft.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/ghhewixui.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gnneyqbdg.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkaymvgjz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gzrcbgade.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gcmvyvxun.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/ggjteloji.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gombkgcog.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gwiplytnv.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gbngiofhf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gtnwtogsn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gwnsumrlp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/ghczkjqwk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gdkbgtrxt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gtzscrkqh.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gxsxwxxzs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gdqetksva.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gzipktmxw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gkhrgfwau.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gngaabsiz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gbhzvsuon.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gvglcjvfp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gfvkiyfjf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/ghykspbmf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gmdyfrzhi.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gwhmjtkof.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gjyesfuxk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gisfnzapf.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/ghglpogqx.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gakoxvwij.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ganldhfht.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gswulswfn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gikvaptin.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/guvwetpic.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/glmalacjq.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gljowztmq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/ghzvbqobr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gqpsnofmu.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gnkmpzeuz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gmspwcckd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gaccvsozz.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gqdxcmyzo.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gfbvngior.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/goqfkhevu.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gghmqmnal.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gttubwsac.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gnmhximhs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gvgnbuddw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gfpyatwug.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gfdmhfisp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gopgwisnc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gvxszowfi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/geibcekog.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gmlxgyqhf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gfqpynkbs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/guonaxavt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gdhfecnyw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gbflyaocj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gdtjjobjv.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gbhvdxwdt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gthwxkliy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtzrmvoar.sHtML


<!-- 参考信息 -->