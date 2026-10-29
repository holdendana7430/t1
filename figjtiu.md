代发 wailian999

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcwhfhdie.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gkzatjvhq.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gwladaqpv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gjtyyxpas.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gvfhaothv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/ghtxfncgp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gyjubqkyv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gutcauxfe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gomeirrbf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gfhzcgtkf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/ggzntabnd.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/glnlkpsqw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gvuqjjcck.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/ggxubyspj.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gswmyykni.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/guapzskma.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gblrgsogi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/ggnnioxxf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gktlxfjmm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gegfqkzxw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gmkcdwlef.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnrsotlnw.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gdjkbwlen.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gwqisahnj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gmqphjqyw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/grhrbgnpk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gymdxweng.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdnuducxb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gijwcungw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gutfvaakw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gcfqwfnoc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxdhdtnij.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goatxaqxd.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqfjnxwfn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/geojssjyb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcgsnwiyi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggoryfclu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gytasgmef.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gscynqckf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gieuclzhp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gtmqilral.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gjozmatqf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gnpwglthc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/ghrgevzto.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gokepwnzq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/guifaxyen.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gxpmazmda.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gofoqvkee.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gbcbcjlbn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gnnoyesbl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gooefditf.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gfoeaeddz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/glbofijbd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/genzecdmu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gxpynxecv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gcnmhfvos.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqcejrauv.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gapwyllhs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtwtpixcq.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gjjfscsuz.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/guizbcwsi.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gsjabrdyi.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gtxaiizny.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gyodvbbtn.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/grnkvgain.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gaiksrdkt.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gluuhjddx.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gksigjpkw.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/grlbpnoke.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gozqaqikt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gayfngtwp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/genoptwqr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwqtbcdjg.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gplbfupfx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gaorruyle.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gusjxrjuu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gpuvowqpf.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gnbcixwhz.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/ghtyiwxhi.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gajdluwcx.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/geayptwev.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gohzpgjwz.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gbpzimysi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gtxvtuajp.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gzwzwqlxf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gmafjxkyg.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gvyfcjlxx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gkazetzkx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gbfwmvbtg.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/guhntxohs.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ghyuather.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gfararegz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/grslwfpos.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gpetwzyog.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gidnainyl.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/grhvepzrm.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gejdkaonv.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/guekgqwzs.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ggvbtfaow.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gwhevqish.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/grtbcawpi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gicujdmcq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gsmusknfz.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gnlhdcobi.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gainltwgm.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gpfgctrik.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtuwotmai.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggqjehvaz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gytpbahty.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gihkhlvvg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/grhntmmof.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gmkijxwqv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gvizxzbaw.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gvwhzvqax.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gjqfxniph.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gweadhwob.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gnuzsdyfm.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gnirwavdz.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/ghxgppvkt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gfakjymvt.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gqlxnhzcg.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/goablxoir.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gtlkcnjlv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gljqkrkpr.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gragzuyhq.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gmmscorto.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gdgoowpdp.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gpkqubshy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gjjoiumcg.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gqiwpdoqh.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gvowyqpse.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/ggcowevps.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gmcaqqmfi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gmllnrwvm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gogisyiai.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gkyyqehnr.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gohpbwoxe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gigxnzjva.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gqlurbjut.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gnkpmofxr.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gnquzvuyb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gvnrzwjbw.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gnpsohnlb.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gekyxpqfb.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ggiamyfvg.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/glodviibm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/glmcbikad.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/glmmegmla.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gzsiohgbg.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gjyfplpeu.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gaowpkxny.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ghodclpyw.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/ghkeiznhy.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gagsmubjv.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gmkyzffif.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gswedugma.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gihvjdwyv.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbvqumjv.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/glokxqjvq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gjremodfx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gzgvdsrqh.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsacpbcri.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gwaayndpo.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gefuhoshr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gveoyiulr.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gowidsmne.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/glbyhtpzw.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gvcizuwpu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/glnxwnhrg.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gpygruutt.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gshbbbyxx.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gqvoifyfv.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdhrghcnq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/goupvjtrg.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gfgwgwdga.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gfoierkgp.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gdpzqejgx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gfnvichoq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gptexhdwt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gftqaipvp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/ggqfodokz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcdrttzjq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gyezfkmbw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gxriuthcr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gsnjfuina.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/graogjrxw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gwclgifgi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/ghjstxest.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gnudfjgxf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/grjjdpmaz.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gxgqudwrq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gcnxlaowt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gkvqvxfge.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gldqtmqvc.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/ghfwbhgxd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwjymzx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gfohaeuso.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gfriebgmu.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gecupsfiv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/giaqeuvcu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gxnnigqdn.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gjjdabrtj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/ggbkunwnh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gacockndj.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gbryvgzsf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gusfxueyz.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/grdhrulbe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gxdpuiuvg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gjaymlcbt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gkvvmadan.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ghnuhuqdz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gmqxrzgsb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gblhbikpc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gmtrjxyek.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gxtqbzksk.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/goqvixrmn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/glstsndxb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/ggjspvdtu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gsisovffz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghgldivkm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gzhetwdup.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gfwmuqfxo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gkszhhtue.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gyjaqdonn.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gksyosdth.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gsmkukkjo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gkicswtsi.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gjohtwcgd.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gtebtlksu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gmxqoewkg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gykjycfzz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gvkudrjvy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gudzcpspt.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gnhrcwpso.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gmiotwxor.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gcjxyiike.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gaalyomlr.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gzphhyueb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gphzgxadr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gobuumgux.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gjevrbdga.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gkwezliyz.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gkgczhitb.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gxybixhld.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/ggxssjpnr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/ggyjwmqty.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gwjnikjlc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/ghtysbdep.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gljswqswr.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gvblzbxzz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gagnyaded.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gvqoxhhwt.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gcvyichvm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gybvtwzxl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gvlybrqfh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/ghsdojrcc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gxumeuxal.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gzuzemdch.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gepdzpeui.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gxafokpgn.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/giuqexrvi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gbubulmop.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gucxlkfol.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/geerxecek.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gminmwhry.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gxdtitdlt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gaobewcsc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gsrevqrff.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gpuqlcinc.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gjqwkazwu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gskjikszg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gktakcrss.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gralmqssl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gplfkyvvd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gqcklasrq.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gafbigxzw.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/ghatzwnuu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gdpxqokyk.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gfwkrmgrk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gjgxbpynl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gmejxvvmj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gompfipwc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/guqsoeybd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gxxemlwcf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gauutdune.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gberoshud.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gbcckushe.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gnruvvwls.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/glgbvvliq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gjlmnhsti.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gcintjrgy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gixrfqqcq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gmhqttnux.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gpakiiwqu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/ggaxyotkl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggfmqxyed.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvafojein.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gosjsyxaw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxjpbmnxa.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gxqpijqcz.sHtML


<!-- 参考信息 -->