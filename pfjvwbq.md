代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gntjuwokw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gzjuqbzew.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/gxmtpxlnc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiaojlpe.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuxkiwzy.sHtML

[F06] 删除文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgmbhdlm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbwnwqfm.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbbrfmxo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnttomno.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnpiysmy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gghkzxlyp.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gkqsvbeoz.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/goexdabzh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrewtjhx.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/goshjncds.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gwpgihcvu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gredzjhjy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjevehho.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gsodkosat.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqgzicll.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fanxiaobao.xyz/Article/details/gvxezvrxu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gsevppqni.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fanxiaobao.xyz/Article/details/givchgqgl.sHtML

[F08] 遍历目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmplrfmm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fanxiaobao.xyz/Article/details/gdvccebrb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fanxiaobao.xyz/Article/details/gscqjmopl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmyjjttz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/glqtxooot.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuemrmcc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcmjlxxp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gmsvrdavs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gdivnnygo.sHtML

[F09] 获取文件大小
来源：http://3g.fanxiaobao.xyz/Article/details/gkjigiakx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ggwbmdxbc.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsduxxnhk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqebmevj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgpqszwk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/glwuyrasj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoxlkvoq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjlgnynq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsgkvtdm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwmjhpqo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gxkpgiecn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaevftoav.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gyanzalcn.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrqdqhdt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fanxiaobao.xyz/Article/details/gahrqacxd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gglylvxda.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/grzgdsxgo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/geborpzyl.sHtML

[F11] 复制与移动文件
来源：http://blog.fanxiaobao.xyz/Article/details/gogtgutot.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gobbwajqp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/glzygcmjv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/glsjihqpp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gjlbyjvna.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdimjcfmn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fanxiaobao.xyz/Article/details/gsgfouzwp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gpdqnokov.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fanxiaobao.xyz/Article/details/gbvjnljaa.sHtML

[F12] CSV 读写
来源：http://blog.fanxiaobao.xyz/Article/details/gfcfbskjg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fanxiaobao.xyz/Article/details/guoyeydpz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fanxiaobao.xyz/Article/details/gojsymwnt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gcldunadl.sHtML

TS:   // 同上
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnvnteio.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fanxiaobao.xyz/Article/details/gudbsfpum.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/gijagwibj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqmseuqt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fanxiaobao.xyz/Article/details/gdrrsvwrp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmvbwpae.sHtML

G. 面向对象
来源：http://wap.fanxiaobao.xyz/Article/details/gziniwoqa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcmewlwy.sHtML

[G01] 定义类
来源：http://wap.fanxiaobao.xyz/Article/details/ghdieksiy.sHtML

Py:   class User: pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnujajbo.sHtML

PHP:  class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gyzoeyjam.sHtML

JS:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gogkeoyjo.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggptpoclg.sHtML

Java: class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gakjsvdfj.sHtML

Go:   type User struct { Name string }
来源：http://3g.fanxiaobao.xyz/Article/details/grxsuhqml.sHtML

Ruby: class User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuqbnpim.sHtML

C#:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkvdsofm.sHtML

[G02] 构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gsqqvxiec.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhqnfsub.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gneuaozuv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbnqsjvq.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ganonnwwb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkobeiba.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fanxiaobao.xyz/Article/details/gpxuurjge.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkowknff.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwowbhymk.sHtML

[G03] 实例属性
来源：http://www.share.fanxiaobao.xyz/Article/details/glwuihhqg.sHtML

Py:   self.name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/grdbihebn.sHtML

PHP:  public string $name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gjeicsmts.sHtML

JS:   this.name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/geigwnwzv.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnogqntna.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/gzkujkpvn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gstmawdsk.sHtML

Ruby: @name = "x"
来源：http://m.share.fanxiaobao.xyz/Article/details/grucazqaw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gdjhtoera.sHtML

[G04] 定义方法
来源：http://3g.fanxiaobao.xyz/Article/details/gsadurhjd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbgkulmq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbckkfsb.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gszcjahoy.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzzlxtbuq.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkieimjx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgvhbcog.sHtML

Ruby: def greet; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gitabpjlq.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gsubvwzes.sHtML

[G05] 继承
来源：http://m.share.fanxiaobao.xyz/Article/details/gylibupmm.sHtML

Py:   class Admin(User): pass
来源：http://baike.fanxiaobao.xyz/Article/details/gtdufbiih.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeqcxvra.sHtML

JS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/grrxmyemb.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gsjgiidhh.sHtML

Java: class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwvnnkssd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisrgkphx.sHtML

Ruby: class Admin < User; end
来源：http://wap.fanxiaobao.xyz/Article/details/gkhqafgrt.sHtML

C#:   class Admin : User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyauorpp.sHtML

[G06] 重写方法
来源：http://baike.fanxiaobao.xyz/Article/details/gdomsjckw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdknlgtc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoaxzndw.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfnhctpn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjifxutp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdighdpru.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/grpxulogj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoeorvzq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fanxiaobao.xyz/Article/details/ggkljvfrl.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygzgcmsm.sHtML

Py:   super().greet()
来源：http://baike.fanxiaobao.xyz/Article/details/gyzncaxcc.sHtML

PHP:  parent::greet();
来源：http://blog.fanxiaobao.xyz/Article/details/giebqzypb.sHtML

JS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjuzydth.sHtML

TS:   super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/ggywxvjlq.sHtML

Java: super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gaiajdber.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapqqlguk.sHtML

Ruby: super
来源：http://wap.fanxiaobao.xyz/Article/details/gdewimciy.sHtML

C#:   base.Greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvgshzgo.sHtML

[G08] 静态方法与属性
来源：http://3g.fanxiaobao.xyz/Article/details/gomjbuzpw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fanxiaobao.xyz/Article/details/gypgdwktw.sHtML

PHP:  public static function f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gejfuxspu.sHtML

JS:   static f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapoxwraj.sHtML

TS:   static f(): void {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxweenvlg.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmqgqlwkv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnehgcndg.sHtML

Ruby: def self.f; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpawlbzz.sHtML

C#:   public static void F() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gshxhvdkj.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fanxiaobao.xyz/Article/details/gffbmxugj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvahfwsl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsnuvfwb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fanxiaobao.xyz/Article/details/gunxyrpbg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpercoto.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gikbxwxsw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fanxiaobao.xyz/Article/details/gbwmnoekz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grlaceqrx.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/goaxzlnsj.sHtML

[G10] 访问控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwsagopi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyeksryk.sHtML

PHP:  public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gnebxeadx.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fanxiaobao.xyz/Article/details/grrnogvnp.sHtML

TS:   public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/ginwgyexa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqngdiuo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fanxiaobao.xyz/Article/details/gnltnnmkt.sHtML

Ruby: public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gggbgnppv.sHtML

C#:   public / protected / private / internal
来源：http://3g.fanxiaobao.xyz/Article/details/gfjuwoien.sHtML

[G11] getter / setter
来源：http://baike.fanxiaobao.xyz/Article/details/gvoudjltn.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fanxiaobao.xyz/Article/details/guuryvvce.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glgfbutec.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gafzirggh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guujcpxni.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdwmtzxt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiiwohro.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fanxiaobao.xyz/Article/details/gbooxxufn.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fanxiaobao.xyz/Article/details/giucugarm.sHtML

[G12] 对象转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwphmvqlk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfmywzgv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbzvzjsi.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyvztlnzl.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjmwwfru.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwuctqxso.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyyzbohj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/grsiqhbww.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gflsborxl.sHtML

[G13] 判断对象类型
来源：http://mobile.fanxiaobao.xyz/Article/details/glvropzlm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlpejyci.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtxmfvue.sHtML

JS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptkltdyo.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gzytchnmp.sHtML

Java: u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gihpralop.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fanxiaobao.xyz/Article/details/glqxsqyyb.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujdmnnmr.sHtML

C#:   u is User
来源：http://wap.fanxiaobao.xyz/Article/details/gbplgmxfe.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrbsgzkm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fanxiaobao.xyz/Article/details/gnejflcnv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaixjnvi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtbffhjr.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fanxiaobao.xyz/Article/details/gblftnyvc.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnvadrxtf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrlveoad.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fanxiaobao.xyz/Article/details/gyhplgjxe.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaovglgf.sHtML

[G15] 枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gdleywxxb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfrhfnhh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvozpkrqz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fanxiaobao.xyz/Article/details/gzhnotsua.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaugviht.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxredvsc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/grktnawiq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkvlwnsm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztnxmaid.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcldawox.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fanxiaobao.xyz/Article/details/gsymcagqk.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwmjakaz.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbynbwuq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwztwupq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fanxiaobao.xyz/Article/details/gclwrtmvt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzyjufuz.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fanxiaobao.xyz/Article/details/grtsuoouk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gcorabqrb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbofnvtnb.sHtML

H. 异常与错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gqpxdrhvn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfmespxp.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtcwpoil.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/guvbuyquz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gildgnchz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grvcnqwvz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/guotpjdwc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlmtdbnw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrsfchep.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqounrjxk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ginqxkygc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhtatejm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksagheyt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggfugwpnn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcwrgjwo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkywlzujh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeyhurkh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fanxiaobao.xyz/Article/details/giherslmn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmydcyuhw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjouassc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugqxvsuj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fanxiaobao.xyz/Article/details/gkcilicbd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gxwshbuzs.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuzaucoy.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjmkegoo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gaavcgbpg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/glpfpurze.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fanxiaobao.xyz/Article/details/gjdyjpbun.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdjuepcp.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmugxxsik.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjfibtzr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gybaagfcg.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtmypeaxr.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grazdksyt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydjjjpvd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgocgexl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjzbxmoc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjuevkcb.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksxjubad.sHtML

Py:   except ValueError as e:
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaqcteuy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhjpmduo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gguhxuhau.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxisyofjw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvuwcgvv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fanxiaobao.xyz/Article/details/gnaqwybzp.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fanxiaobao.xyz/Article/details/gazbyhlep.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvyudbyy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/gyzvemuua.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fanxiaobao.xyz/Article/details/gyubkolrv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpazeqvcx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmciduwt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gyrmppkwh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/geopefeov.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsasuwusm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlgbjkcu.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gsrnwqczz.sHtML

[H07] 断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkvvjgai.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fanxiaobao.xyz/Article/details/gfdrwmnqr.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gchpqlruu.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/ghbncdnzn.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhrfbant.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdqeprvt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fanxiaobao.xyz/Article/details/ggrelujfy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fanxiaobao.xyz/Article/details/gwppkfwha.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/grsyauffs.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gohnyepyt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/gzadzfodf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvgmkjly.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fanxiaobao.xyz/Article/details/guaqttjfu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiwipmyy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcanmvksy.sHtML

Go:   err.Error()
来源：http://m.share.fanxiaobao.xyz/Article/details/gopcnsbvz.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrjedzlm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fanxiaobao.xyz/Article/details/gtrvcxdzb.sHtML

[H09] 带错误码的异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmtxqbma.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/gzynaszsz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcmczqur.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fanxiaobao.xyz/Article/details/ggcxtjbvh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmsmpncu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkparchd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gnepcceci.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokhclgny.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gceughrpf.sHtML

[H10] 资源自动释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gubcuvfuv.sHtML


<!-- 参考信息 -->