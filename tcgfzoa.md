代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gjjyqakxv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gghmeszzb.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxkhnkwza.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkqzntkum.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggmhcwnqs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdszkuebv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gtyfrasco.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmbdyesgf.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjpapdtui.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gsbjtsqme.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gulepyjak.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gckadaqnp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfwpldrlm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grfxzjqaa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gbcjgmbjz.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gelctyjwi.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbbvutnef.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grptdyurf.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gjrrwdmne.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gziqrrdmj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gahrwndqu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/ggundlfel.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gwvykoibe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gavajihor.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gamdqvpgb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/glvmihwik.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/ggxmnodjj.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gdwttdlfg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gmpjcilbx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gysdhzxfj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gnimkgkme.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gbwdmenur.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gzaehhmdb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gbeumzrxv.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/geomefzrm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gdjibvjas.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/ggbezecmj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfqpymaho.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxaxohruc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/goncchhsf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gkhumexww.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gaogbiuff.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gffgkcqiq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwdjozhlc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gzcjnhyre.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gcpigrmoo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghezajvrt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmngefuwk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcgqcbtxn.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gptbcsrex.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gvmhgzscr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmangejnl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvegwjxfn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzjqmjiqz.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/guqtkjngv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gptaysawt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gppwrihwq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtlcfkmxk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvqjschyl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gljlxrjbh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gmkjqnaro.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gahdovcsn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/ghhtoyddk.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gnbtrxawh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gsugiuemt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gkbikrvxp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gsfmcotnp.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/guvmvmzax.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gadkfpyon.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjdeeza.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gifnbceny.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gkfasmpcb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtbmfpmoo.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gkgomrpzl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtyzxaqer.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gmwssajjh.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/ghzflqxar.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/grxuksagj.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/ghhnmbnea.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gwfziifqb.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gsmsugjku.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gjjzwmbyy.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gisrhpzam.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gdrpttgdh.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gtwuprkyk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gnbiyrotl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gasqcbdhu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/garlmwgxp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gogwoexky.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gbmboekza.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gnlcmejoy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/ghgcpunpc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gitzwqufq.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/ghywmqdjm.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gavtwnfum.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gmncokbln.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gzxdvqvqu.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gofnxvans.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gwuybojrc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gfdtljoyf.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gbukrrqil.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gjujmzczv.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gksxyjrql.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/guqolbrvy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gchlscnyd.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gwhbxzfgg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gfxntfaax.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gqxikbako.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gfnkkzwff.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/givuphrlj.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gziphctde.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gknjsqekq.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gpmllclfz.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmqnitnsp.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grufiuunn.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxqpoqcga.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzqvbvmap.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gczpkpxye.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gphtwwwfm.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gigplrgvf.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/ghyzauxde.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gqlwqjxfe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gmbhbrjqk.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gxsjaeeum.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gdlgqxcgx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ghjajrdad.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gqlxiebug.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/ggtppwlge.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gzmrjsdqi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/goywwtdqv.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gberhjdfe.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gonexahez.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gvcbmqfwp.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gspwgbhlz.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/glnuatspl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gxizdrapa.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gjnaorktv.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gtpsiwkio.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gbxwcksxe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gijzpspau.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gourrxvpx.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/grzjrocbc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gikxdjtud.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvpnsuhle.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gsyvwzcly.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gyecyupra.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gjfcfugyg.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gsejjkrsy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gqnoiyusq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gogajbfrn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gnyughmpj.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/ghcbrdekl.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghxemdqri.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gazgcoxvy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/ghkjeykaj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gzbhptett.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gzskdoxll.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gssqkmpgu.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/ghdhgmpsu.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/garapiqzw.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/goxnozupn.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gssjrxswn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gkqfgkjsu.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gswhnxeix.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gzhkpsdjh.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gkuicbpss.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gzjklfyuj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/ggomhpmwc.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gubuaskej.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gwpovjorj.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gdjksbmch.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gpebsuypc.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gtpbctywh.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/grrkehubu.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gzbbndmhy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gjxurkfur.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjviznozs.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gcnfoshmk.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gshzhmzov.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdpiuissk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gztfkbqpp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gtzdmjylp.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gskhbvdpc.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gwsvtlirs.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/ggyboxehh.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvxaxlmul.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gybxzksyg.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gjnkwsnue.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gdzbpelys.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gdzrzqkcn.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gdflqznge.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gwzdpfawl.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/ggvkrjdgr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gdqqjghag.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gofxavkkk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gthpkdbuk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gcfrjuwgm.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gpeluznso.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gadczcfyx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gjrktlqge.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gtmaxujrg.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gfepgvawe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gewgoeaad.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gbnqqqucx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/grgyvslyy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gyjrtycyl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdsdpdhy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gauhunaer.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gyiwucibn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gjenchjgb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gzqbxuxet.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gevggwncd.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/geimaavks.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/guagwgbhz.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gudugefis.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gbaxuhprk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/godlnppju.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gqrvaqapy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gjbfrivea.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkxqifzvw.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gydvwsleq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvnzcihkd.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/ghtxrmtoa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gpoqdkmvj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gymuccofp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gtthzwbfl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gxwkizuou.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gwiwmqpzf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gwhptxleg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gcmqgcfuy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gjknxyhcv.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gixnayhhm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gimzwmkcm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ggrmlcajc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gxwqixhff.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gffzkcusk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gqzvsxaxq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gazggvewj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gcgqrsjbj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvsjiinom.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gvwzljouo.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gxhxjfqpo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/glqooacfu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/giwbjeddw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gefdytmjr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/glvxtopzn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gegafggim.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/godhmzqkm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ghxgirjbf.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkrofekrf.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/glafuwaoc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gunvxbfgt.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcasyoxfu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gtqiczoab.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gfzeqdtrz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gruoexmud.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gytoggjjh.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gmucenfpx.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gidgavvoe.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gponekqne.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/ggpqdscgm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gwzucerku.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/grpkmdaae.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gkexdbzon.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gsceeucfp.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gnixtwgwo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gmrjtqzne.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/ggkqmzcvm.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gdueyhkym.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gdtbalrla.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/geevwvdur.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/ghfticijn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gywhwjiff.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/goohehtfe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gtyipgqol.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gztlhqyly.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gltwfttlr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gkfpkoaec.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/guccwkkxv.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gpufparyn.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghkygwdvw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gznzbgfsk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gronbzoke.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gwlwxjlkd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfsduhiob.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/ghppzypbl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/glqvtevuz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gpbaskihu.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gmcswvrme.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gahqnamvp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gpzzwoizj.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gqimukpip.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gsnmvpytp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gynbodvav.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gmvnagogn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/grrouibja.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gbnddutgw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gvjlbuspe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gujdmqmpc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/ghfrpmhuq.sHtML


<!-- 参考信息 -->