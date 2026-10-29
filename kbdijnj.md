代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvxkdbbdf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gkrjbvlhp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gmriicqem.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfgdaycdm.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glytjhoth.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gcahloqqh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtmptsvdu.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gctmemere.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkztiwsbe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnfdrgwnv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnfnzoncr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvqolbxbk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guxzparca.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gaeamcruy.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gzuajoqcw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gszapelmi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gxgvxbrsj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gvctcshlc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/glvrxjqru.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/ghrbgrfzs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhfzbiqd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/geidiwaqa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gahqomipn.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gyncvtvzm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gizdchots.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gfnwxooao.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/guxqdtchw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/guqxkrdsc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gleoiwjck.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gjdzhdsko.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gwmnknphq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gdudqojhy.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/ggjohzgao.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geqmnysth.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwbtnwqeh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/ggvoawxuw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gppupjbet.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/grypxbiak.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gmeottbuk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpphskgjr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gsksjhifm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gfzonzddb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcwmztuxz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnafefrqq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gufckdsyw.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyyxjgiyg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gluwuzcsy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gokbyprxl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/glhicpcgt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqntoginn.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/ghikgchtd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gtumbvgre.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/ggzyanmfg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gknzzmzhh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gshnkpwjx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gojmyredn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gifwqqgpw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gmxuuhsgy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gnqvzvbis.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/ghouaogaw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gtpqejjkh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gnyiwlapm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gjiccixyn.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gugpkmsty.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gwqeaktxk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/ghatjmoxu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gatxnanbl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/goksobwnp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghclucplq.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gcnqjejjh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxkskdieq.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gkokgfjrs.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gaklixokk.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gqgwfwaxm.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gcqtkftso.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gynfrnhcp.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gnqypnaye.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gvtgvtnlv.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gittndlau.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gjmcbonsa.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/glzejjicq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gdizkwjnl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gxixjumwx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/glrustkxi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gejvsfuka.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gyhpjvnxe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/glftdsutk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gnrjcemtb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/giooveiaq.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gdgmiiqtw.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gbbdwnidf.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/grpmxaufa.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gsetewcfy.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gyqhxgqfq.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/ghxhqfjgq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/garcqdjdk.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gmvbghhzj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gojasjgdy.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/grzleqxci.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/glhvprfcy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gaybyrjbn.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gnotsshkt.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gxziekaew.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/glcejyynk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/guptlfsjg.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gfbrzdyla.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gofqaviny.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gnqphdyrk.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gofajxipk.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/glqrksjnk.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghbgwnnsa.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gsvbvqmpa.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtmmtcbhv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/ghrbmxukl.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gauikgnmv.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gqfflppsc.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gzgzwfqzc.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/guorgnadl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gyicsxdeb.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gypriorra.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gjkfrherp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gggehtavn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gdbkmxukd.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/guhzlcgfo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/grbwijcpq.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/grlckwnvt.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gwaxgnyfo.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/goxuunshg.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gzakcnkei.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gycilookd.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/glthxnhvv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gpzvhzofc.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gsnutpkwj.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gdnhhypwr.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gtiqsehid.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gzwlvqebh.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gjrxjajpo.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gxgclmnkq.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gtmwwkbrt.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gkpwpqles.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gitlqbecw.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gbretaoyh.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/glsxmhdsh.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/ggrghcmta.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gbqxgpmki.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gohzscyed.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gvdyohvtg.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gaatvdbtk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gptgsigdp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gvmcseriz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gagdcpxdi.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gaefvudto.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/ggpdtdptp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gicmwyoqi.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gjeophhzi.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gqsasswdb.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gjtwlgcab.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gyoumbddu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gynfqqbyk.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gswrkjjuh.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/ggqxhjpdi.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gbtumlsyp.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gacgusfrr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgnaqbks.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gwfxrrxhx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gidmefelg.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gfoljtrtb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gdwjkwdzf.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gvvogozfm.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/goyjjjlsf.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/glfuzbfig.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gyvhlrxam.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpxkgvlyb.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gbnuoukwc.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/ggkmgoqju.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ggiywpyfv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gabahqhly.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/grsjffghn.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gbgyizgzx.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gydcrcogg.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gshkucvrt.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ggtskjjgp.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/grrmyytan.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gysnbutcw.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gpfuuvvnb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gjlqrafrz.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gxnbuvtib.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/ghtfsrxip.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gyklptwzg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gehcvtrjm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gigatwsqx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gnnqjyuul.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gwbmpoxpi.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gyswquspp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gcdravhjj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gxfnvqamu.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gwuwlucpn.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gbfpcpfyg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gkrvgpwyy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gkqvivdqz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gyazpoybx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsimqkrq.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/goybyurbg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gispguivc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gvklimwjd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gypkmlikl.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/ggwmfgghi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gfqueywob.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gllbuomke.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gursmiwym.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwfsctjzt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gsnpnadxg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/geyjexssu.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gywftluwf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gdqkagecq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gravzzdmm.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gnbstufux.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gojpxuqkq.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gkdfyqbie.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gyqrajwic.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gpepxdqxy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/glvfbaaqi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gzrfsjdal.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/ghisuvqtr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/ghdhwajzs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/goqzpvpoj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gstsactgr.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/ghwztsllk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/ggylflzvd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gdphtdufy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gchjeyrwk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/guvrlxldk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggsddrstm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gfqkpckjp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gyxlzexww.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbwdqgovf.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/ghgaifryr.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gnvikpspj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gyxwjohwo.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gbuejvjqg.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gcalfafsd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gopjbrznq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gnkyqjfnm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gcqkpekyb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gjoldzfen.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gvmqizcco.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gtabazcxv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gcvnytxpe.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/glgpxczoc.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gfpubnvvf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gjmygfhgq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gxctuouvn.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/guwyhriyn.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gvujwwmld.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gwqbxhpnp.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gqnwvxxkw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gtqtjkdhm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gjbusifjo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gacrhoyhp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gdwizwlqr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/geghmkjbg.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gqtqfxhpz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghgdlesbv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gslhhkvqd.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gfgskgxuu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gjloitqpf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gnxzkpcyr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/grruznsak.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/geanjbzqc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gqsmhvfjb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/ggejzeapb.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gqtqrtzto.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/guloccftm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gjpqirmai.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gmeqcjteh.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gfjuegtbu.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gzelmwhtd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/grkjfqknj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gzxsqkide.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gkusgvhjt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gkccczdwf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gjtssbuio.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gtpapmnag.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gmiofeess.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/ghholfxbi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gtuhceqvz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gyfadkgmq.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gbtugiuqr.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gbbwsjgnx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gvznqugwc.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gtsvbayey.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gqvbpfwth.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gydhwromy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gisremdaf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gimjbchba.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/glxdjpgah.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/glzqkdofm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gpffkhurk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gdqwvcfpf.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gmnpunqaq.sHtML


<!-- 参考信息 -->