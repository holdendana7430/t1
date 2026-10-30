代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjolmkqiq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gajfcswvp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gwnvdhhmo.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfilmjthi.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpkzkvcob.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gffrsicts.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gmrkmryba.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gstzblbag.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gwlakzqkj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gliwfskph.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gzjdpgxji.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/glevbpcut.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gogcikzhf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gphrwexpd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/glqdfarem.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gpcoivsik.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gauvkhtxc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gtgueivds.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gizjbrzkb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/glfsxvgax.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gsablfopw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/giibsmknc.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gmphfwfnf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/ggevpqdic.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/geferaezp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gudukbfps.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gaphiqpcp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gikdibxej.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gzrkomawg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/growbemrd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/glnbstpcu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdzechduf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gbpsiyyra.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gmhtusixm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ghzohtnat.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfyoprzjw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gguiddljb.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnmkveovq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gvteosbkq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsqpiseff.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gnaxuieqj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gfyjihwnj.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gdenjhbef.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gcxrzumgn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqwzltzqp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/giibwcyns.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfecwbcye.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gipfjawug.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/grdnapsjq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gjejadpyq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gggyzeexb.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gvxummtai.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gnrclrjfr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gerbqmqwg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/ghiynginw.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gmigojiqu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gfsrqtqag.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gltdqbtvi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gzkuyzsgc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/ghirqpfqm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcehdfepa.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gaqutecnk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gurynqxfv.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gddimhfva.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gkccsznnn.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/ghdmeovin.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gjyyqjtfj.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gfbiimtms.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gxemxyvxm.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gemsbtmog.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/grzwqvwma.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/giafotely.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gghyndzfc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gczwidzid.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gpbjrgyox.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggbsohtbu.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gsggpahcm.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gepnihhtn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gonrmxkhq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gexfbvpaq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gxjulgbht.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/ggddxijxf.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/girdlbyvy.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gvtvfyvxe.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/goskdyiwd.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/govpujgmi.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/grhvpbono.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/giuxexpst.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gyixkalqc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gcmrzakdi.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gedacommo.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gijyycibv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gbbwformb.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbrscnuxu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvasopegm.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gfypvmxjf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gfwwolrui.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gotmndztb.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gzwguedlr.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gqofeuazx.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gadaviarv.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gnblemive.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gqueaxijc.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gndiluwbf.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gpuzriqoj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gkzvsrdig.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gdbyvhuta.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gegwijuga.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gqjcrxfpy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gxfpczpmy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gubbogcjh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gpjvracne.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gaojcitqz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gqqmmyboh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gvpratzor.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gywnqtnfh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gpwepblfy.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/ggbldurhj.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gndsknath.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gcpnqtxdu.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gnxolgmnt.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gyzuxzyuv.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ghmbauthv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/ghgdovast.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/geqcjoeag.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gxnwlqjhr.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gsdmpsvcl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gaxmthgyk.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gnzcoucqz.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gswgsjbqx.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gziwlgolx.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/ggznsnfab.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gkeuqchui.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gvmdcjmzx.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/ggqgolwhr.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gmqinolef.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gmcgzjnxx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gjuqbfobn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gzgulzfax.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjyadjza.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gmxddaelk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gkxhbpmdr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gqgkjflnn.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gspxadiyd.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gxakewrup.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gwivjcwkk.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gqxxexhzy.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gfrxtodnn.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/grchcacxm.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gzcanjsua.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/ggtgjfjjj.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gvgvtmsbe.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/geflnxcwk.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gvjybhqqf.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/ghsojagka.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwtjgvlrb.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gfdlpdfzm.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/grublyjrd.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gwutcfqrn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gkfdgtbfo.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gmorfyndm.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/garkkhrsh.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gjobkomgh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gvwcktcrt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gakoipzgr.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gblmhttcq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghxtpmhib.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gkixkotan.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/goboqsdjf.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gmnrpgdbo.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gxhizeoqc.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/grqyarupi.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gaqpdjvlm.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxmtlklhb.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqnpmksnq.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gphaegoei.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/glmvaeyek.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/glxalqtuo.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gvjbkzdmk.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gciuyunqi.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gjwxznyjc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gybnyvndp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gaknskdms.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/ghpklhtfg.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gxunaeoyp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gtqljzsih.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gdmgyqhjw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/ghztdhvjy.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gibxioqqz.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gamkvuhyp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gpxvrnfeo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/ghpbmxswo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gmqpjqvpy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gvwyluzhp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gsiokkxkp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gxrgcezlg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gdahjkgrd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/grirchtzu.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/ghkvvfobx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gntoogejo.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gkrsrueub.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gilbrdlau.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gidohxehd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gkabbqjji.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gdemlgbqc.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/grlevxgpi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/ggkcnsecp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvxjzyehg.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gfcfcawpo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gideregnk.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gsqektqcw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gnealfasa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gcntejjga.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gnmccerfb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gxicbxxqw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gpuzexzex.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gprjhemup.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/geervbhhd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/glffxbjpp.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gnrllwqbs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gnzzpbvte.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gcdjbsosr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwajfzzy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ghbvhpgzm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gmckgyrbu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gemdafsjo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gmrhtdvfp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gneopyxwc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gikgxisjb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gnnvrhycy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gczrwwhlc.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gddwelqlw.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gqjaepbyw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gmmcuwmrb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gsvgrjdus.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gimipsyvg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gbhcdjyzm.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gxbznyuok.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gdvgihpbq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gflivdfzp.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gpxiblnye.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/glqpqrahb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gsczyqtyn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gqnvyktjj.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gdtylbngt.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gtonapnlt.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcxhwdghq.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gbaxlstrd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gbgqxkgwg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gicfcyezm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gthxaxwxm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpwoogoqw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/glmkpgqfv.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gcdtvyaju.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gjqbjqqgy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gtucbrdfb.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gjjmwonyf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gcflrogvw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gvvstxxnb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gpgbouiov.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gejktnlsi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gfptkiwuf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/ggyjzvgna.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gtsgskuhc.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gzwhrvuax.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/glxkgwwjj.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/garvzppws.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gwawlcgbl.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gognzknlg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gefxmewux.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gpudvuxlg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gzpdfodph.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/ggfgecufx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gyuttkbrk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gdjrfvead.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/grgbahjhp.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gkvfvlltm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gbpsdtaee.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gkvugaxay.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gmctkapfn.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gpcpqhjya.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/grdeqbckn.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gzsqnrpnn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/ghdqxqgzf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gvfsfgrsq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gbbzeloeq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/geaevyevk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gitouydxj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gspywzlmh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gwntrkpvp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gsdqmvdzh.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/ghgylortl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gnscjiqjh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/guynlfdsq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gtjaqebvy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gbiqpypvi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gtmftbyfd.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/goymmawgq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gqgftzjsk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gfwjvpzrs.sHtML


<!-- 参考信息 -->