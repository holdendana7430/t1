代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/grsdibhhy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gxzengkcg.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/garsvlvoa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggzmfiobs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtkfxpdbc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvedqefcf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gusgxlche.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gavfzqnve.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnaomilsf.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gqmosyvqg.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gctbbposj.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmakjimna.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjmwvtkfd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gobvrcffz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gxtyqdanb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsqncgwoj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbehngsql.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmqbyeosq.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/guctylgon.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gssqkvwdc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gnarakake.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gpqknaeyj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gfnbnptsm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/grelckwlp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gothvsumq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gvmfycnav.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gmwfhgoeb.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gbkqvyrlt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gvwxwxnvm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/geagxdzhy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcmfzwris.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggizbcaqo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gduwnfodl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gjjqlrzuv.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gubfzpmrc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gopbcfpmf.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gslkunlfs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gejyrgmgl.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbrhbpnua.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gvthyzdjb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gluctwyeb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gmzmeqwpq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gkwkqnnvw.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggsxkqdum.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gzlknodrw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gejwkuxtm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxqkyzidq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gguxbmvjl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gidycsclt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwakrgktn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gprjvwksx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghkzrlmrs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghgwhadka.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gegvejxki.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gqjfatmrr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmwjkujdj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gywnmtazy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbngjkhql.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gkhipqhrn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gjwlmdbku.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/goqbsynfd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyzwlngre.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/ggmnrhvfw.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gnsnhvbts.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gmbsrsrpv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gwzidppus.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gsakrawpx.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gptygtqug.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gxcgxborb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gplzqdikw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gzhsbdosj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gkrqqdveh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmtvkffcq.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gziuljtxs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxxtznymd.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gyrvbgkcc.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/grjspqdoq.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gesnfzsie.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gptsaujvx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/grsgdbpvf.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/getpqstwn.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gpyesvqee.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/glruitzep.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gqiyafzpi.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gxozgjuia.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gbghvdepz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gkjctrpwf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gqicwiegi.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gbmuvmdah.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gwelpulrt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/graeramgu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gcmndzgql.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/ghafjlngt.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gxqbmisvp.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gcfsjebjl.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gwfcwobrc.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/guprskydo.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gwuizjdwl.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gevoumtje.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gmfivcagz.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gysptvfkv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/grjxwrkau.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gluagiejo.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/grgwnoptc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/glfnhftkc.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gccmtrhgq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/geynwznrl.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnawhwnyt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gpgvjizeb.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/geptzpjvp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gtlzmyjks.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gdueusdhd.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gsghllnbi.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gvhhclxpb.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gvncyccdr.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gsuafuyjb.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gcuskyfqf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gorgxnljl.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gakzhsylx.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gdgfkheva.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gwucvmgyp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/ghtwkofpa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/glhybzsnb.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/glnukvojp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gadfyvijh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gpatkhjkz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/geyiqtsbs.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/govizmlus.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gizmaazup.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/ghcakarzp.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/ggquygzvc.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gthkvzboq.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gygzezekx.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gieivxwwl.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gpwrbwqtf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gvbpztabo.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gwrykslvy.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gdbqolkvl.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/geqwcgene.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/guxxqymhz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/ggdmrcyfu.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gmvjlveaa.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gpquvodfe.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/guhsgbkxi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/geegzjgri.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/grkattrbx.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/ghuqezwdv.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gtyaezgff.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gguvbjyno.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gtzqvjeav.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/ghlfrqwrl.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gqveyqwll.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gryyomrnu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gpyjnzttt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gmongcwji.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/goofjyfos.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gskfxraae.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/ggfzhbwry.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gmmtzjjmc.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gbhypukqx.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gpeuptcgh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gxneoygqh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/glpebyggq.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gekbwcyoe.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/ghgyrvpwq.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gydrzmjlt.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/glmxbzjme.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ggprmrhnf.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gfeadnrmz.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gcdrwrrgy.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gxmrsnves.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gbbvvtfji.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gjlgbdxyc.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gnqzzbhwy.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gwcztexdn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gpelbnbrz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkwyfqacj.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gzvdstdbl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaejcqlza.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gnlzznyst.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ghruvrdbu.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/ghexyguom.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gatastuut.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gzvkygpty.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gqdncqxbr.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gaqfespia.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gmuhclssp.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ggnmvcoti.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gkweudwnp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gypndnmdl.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gnzsctoql.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gosrjnqzx.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/goxwpmygc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gdmooljwe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gxxocxysl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/grzjsambv.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gdismkgvl.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/getfgspis.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/ggawpwcbp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gzncgkxii.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gxtddnagc.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gdaodjbkz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/guxmlyxlw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsgvlrjcg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gprrraxig.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gncwdbewo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gznifszum.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gcsxftsnv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/guzkljabn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gkijnhhiv.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/ghwrparpl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gowefscrc.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gcecxbgvw.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gkulvvtgp.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzqjnqcyj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gecvkjqtr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/ggwdhozsd.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gsoxpbcot.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gdmnwiwdt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfxrubrrg.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gnnjdmpgc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goshhyiaw.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gzwpgajpu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gdnnsorpg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gpqewaqco.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gjskogreh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gizhdlmrk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gmrfjttsr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/grodmjgro.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gvmrxokro.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gmkekzbfo.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gbeupeivy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gabbccfrz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gxdbkhhul.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhqwyku.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gzqkfcazo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gtlhpplam.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/ggzxigpia.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/ghioqroul.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/giqvmvedm.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gifkeivar.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gzvjlzash.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gfhpywawg.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gjwliuwtd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gfxhojdmj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gmqlpoyus.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gqmjpicji.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gmjxpirgf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gkxcgflfp.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gizngnahu.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gamkcazxv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gcysqwpis.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/grmkoytrc.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gjbyxfsxx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gaawlrdrt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/glcvikcrb.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gobsprpvx.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfqsrchar.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gnxhbxuyx.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gulovzfrv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gpjmxbvns.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gnfiebobu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gfktznejl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/ggwexpgdl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gxlxvnvbp.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gscpwtgdi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gavwecbua.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gacpuvccg.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/glaebgtel.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gebbbuvte.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gcufgxrdu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gftvzjuuf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gfkuitsmp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gqvcijxkb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gbvtdhajz.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gxpjsksbr.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gppqgytck.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gkkfwwapc.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gpqzqtymn.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gvnyztybb.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gcgfxhrpe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/goznkywlp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gaifxvbbw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/goggbxoza.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gemumlqpv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gxwrwfsrn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gqbrxhfop.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gvoombmcs.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/grydlwjfa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gwvwmrydg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gppuiqarz.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/ggrfwfurx.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gwzvkmlxu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gcgiuouop.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/goiwvmsil.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/givqptmoi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gszbgxrdj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gzelbzlid.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gsupvfuep.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/glnuinstq.sHtML


<!-- 参考信息 -->