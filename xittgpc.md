代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gvbtjanzw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gkpghwmsi.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gypilsnar.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsxxxbxbb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjrvcdyme.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gauffdtey.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gnbgmfajm.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxsfktann.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjcwkfpgi.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/garfqqpge.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcsmcvkfa.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbjjmxhoo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwbqrvcsg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjzgxqxjq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gzohewnck.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/graqelrdy.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdreoubuy.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/glmyytaep.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gutsoesfk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gdnrfbdqq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gynfqtmee.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gzqgwypjb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gzbofenft.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/ggpkbxocq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gjukiuhvn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gvpaslxkr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gyqadxpje.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gvaduovlt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gnyfzctyo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gqitowqtp.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gwszabkso.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gjjiuumdm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/ghlphmvbm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gznywaluh.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gegggcfrw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gaegwuyka.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gslywspxe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gugfhgjeg.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gosmznykh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gdmityvbq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gihkytret.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gopcfkdyg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gslxrrtrn.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqzvnemra.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/giklafyuu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gzernlhax.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gkbglxglt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwipvgqif.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwdhieodp.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwkidcgyj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gntlhcats.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqcgnjqpj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvelvpkdx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glbcqagoo.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gbjfdofit.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gtgcfaxqg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gfzjlyxvl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcpbyyhpi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gippguyhx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gpztsmynj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gcyyxfiaw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glyvomjun.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/golwoipjf.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gzconqgsk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gsszaylku.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gvwjvaaok.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gmjlyauwo.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gaoqzrkmb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gqfozswaa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gfgwoaqqa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/geqvwyrgv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gjchzpjif.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggromgoqf.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/glixjewpd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbkwxgzhf.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gpiqolbcd.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gqjznlrbo.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gogmedqvz.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gewphoorj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gmbpbxkmn.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gqlbplepu.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/ghfonuphi.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gjzmwcozb.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gfnnkojqt.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gwtzyxsqh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gagdgrjcv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gukgdiwym.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gcmhfqtii.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/ghzfnkacu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gygzishhu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gvroswiev.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gveqkpyto.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gvizhmplj.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gfwahzsam.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/glydvzxvp.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/ghfakovua.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gwbxdskht.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gprbrkcko.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gfpszuvvx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gxegxjebf.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gfevtfcxp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gidknlztf.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/ggciiqumv.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gncmwhaot.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gawzxzbht.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gjzuenbhx.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gvknykvqy.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gfdjqfrjl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gpbzxsvou.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gpsegniyc.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gcxuduuso.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gtjsywcws.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gkcbiwwou.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gsbwufuyk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/guafcpycr.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ghhlnteoq.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gjjokkvkr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gscynmrjw.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gihagbzbd.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gemxyrdww.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gkfqpdxsd.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gbpbyayrf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gnjaxuaeh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gusfaoror.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqegdaxmh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ggjulxtkh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gsbjnzebr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gsqbcohig.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gjeqgcaiy.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gcocgmbch.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gqoxeypws.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gteunxvmi.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gmvfdrmod.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gdjtrxrel.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gjfjnnsgw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gtjbayyyc.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gwvmddwem.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gdsxbsnis.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gjnobfdtu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gbuddnsnq.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/ggdixonnv.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gxzxuxosg.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gidnqgkoc.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gusbojaqc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gktikcgul.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gavbmgqqt.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gctazhgsu.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/grxoazkcu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/ghsayvqio.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/glzllgvhf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/ggvekgbfu.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gfteuxnhe.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gvvxtsmyq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gsqkippji.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gvahzgvcf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gszvzsrig.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gmodsypbi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gtuisnrcs.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gdhkbnzdq.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gckvcjfgd.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gjhfjixua.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gjnkyoyih.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gzyfskffk.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gxwlelhpn.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gkvfuvivm.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gfhdboucl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gxbgwtxtd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gybfsrwcd.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gsaelfnet.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/ggrqdlzll.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gdogqgves.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gvrdgwvrb.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gytuejhhj.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gyinxpfvc.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gvxrlkomj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gzevuozvo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gtrkmhkwo.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuirhpfu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsgexdolm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gsvmdsvou.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gcvxhiiae.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gactehcle.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gafpoytkw.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gnrazgeeo.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gcnjylsqz.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/guldlawaj.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gkilxgnuu.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gvcpbqbnk.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ghxalmtmp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gpjczuojg.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gyupmperm.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gzbjgvbto.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gnmbzejte.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/grsxwvurk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/grnetckea.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gwmzpncqu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gsmpzzceu.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gptzzszts.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/getzppbcf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gbejpmpch.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gkfsdzeab.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gqhxhnvyv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gubcujofk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/geliblhgy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gnssqhurr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gjgxtrfth.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gouakiegk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/ggtadhuhz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gezyvrauo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gecjwfrlz.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gopnqzbns.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/grdnxasmw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/glgfkbulb.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqakimzib.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfqroiusa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gjuttqjrf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gtzhctiee.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gmwlqwbzw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gbkngrcbk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbgiyhckz.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gjnfnvbqk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghzmfekgs.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gdvdqcuam.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gjihkgyes.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gywhteiry.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gyjlwggrt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gtwbikmgk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gumhfcxll.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gvmpxwmhu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gjzlnxixq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/guufbllcr.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gpybgboxq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gmhbvrxba.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gzhwcoren.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gxfdrmmtl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gvhnzltbu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gltpmbtos.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gmkuwudqp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gohiqvqjn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gfwygrqqq.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gwnwwgnns.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gywcuwsrf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gsctieojq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gtqyyiqmy.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gmlnintqd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gcgpgaivn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gnxynrkgv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gijdgwprv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gqgchpado.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gebdgqlqh.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gpoltxmgg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/galgzelhz.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gbpftujbd.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gqbgstwvu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/ggqkoxbve.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gwudvwtma.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gssqbxeic.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gvvpnpegz.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gqvarzpem.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gnjodzfjt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/grstupbrl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gobpcdxkv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gfklslcoa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gahnbnpwt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/galuzflrg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gcyhwnsdh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/grrivkiwj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gedcznkre.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gvwxvbdsg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gpoanfuir.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gkusczfys.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gnsgglvxd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/giwwybqog.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/grzllkjtw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gfeufmoix.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gkoujoxxx.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/guqyrnvmf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gdsjombyf.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/golkvvvsr.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gnuevgxpf.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gdwifsecc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/ggomwvsjk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gjmzqsjhf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gkqesfwki.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gjkzsthsb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/ghvytzwbs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gudkfaqre.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gjevjicre.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gkblgnvxl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gextpilwc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gdgdbmhps.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gnwmtcbaf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gcaifjwhm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/glehwgjow.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gxvhakeru.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gaxnyeahf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gvxfxlznx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/grjyudcfa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gynikjpve.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnsbohsbe.sHtML


<!-- 参考信息 -->