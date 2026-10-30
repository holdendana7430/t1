代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gmnyzqyvz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gtpbscuju.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gkchfdxdg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gqhszselo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gscsewgxr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gzhiqinse.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gzqgvkcgi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gnvufoxco.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gyqdnzgrz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gjmwlbtdh.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gvexnujcz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gakgjwzod.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gddrhjqzx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/goklrjmby.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gdeysncmc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcsoewflp.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxouboxyh.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/glqphtkjl.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzngoruwh.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpzgkcsgr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjigrrixx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gowpidzmi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gredgtkde.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gepktwdfj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geswvmtjz.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbbwzygdw.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gnqhebqxm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gwtmylrfi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gkgvfnimm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gxlqkywxf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gzmupeffu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gmiskqpqj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/glsmuiifx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/guhteisuk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gqjjkiubc.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/glpbxlwcs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gmgjivuir.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gtilsnapz.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gtghkvfjt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gtavqdzas.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/guvhmhktv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gvvbgsdkh.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggnqvlnjl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gwbhbzsjw.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gitrhttuw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gflurytmy.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gocclqiki.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/grujxaiuk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gbyttpkeg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gyjwanepa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gsnxwjaaz.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goqsxzcju.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gkqghnfyc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/ghwqoakbz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gyddcocoa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/guyzcayjg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gymldsmyo.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gywxaiekf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gkcadvtzi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfeslbkwr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/genyhmlyy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gldsnuvzh.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gwtmwewdv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gneqxybeq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvmjubzjc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfshbaiam.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gjqmqfxeb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gwyoyklrg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gaqfgxjmc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gwtolxdfn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gsbbevyqj.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gcbrtlbys.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/geseknwxo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gictzedis.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/giplfmrif.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/graacbhhw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gydlacwlv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gglhhoznd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gjbcarypg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gfqgsovoc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjithtqhq.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gltskjkpw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwnlkzbtv.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/ghmmklquc.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gqizystqp.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gokeoryff.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gmuxdpyen.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gvdtwrsbf.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gjzklgshp.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gteqwpoze.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/glasnfeba.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gcqhjfivl.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gbnonjwdu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gbmgappkc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggjqsbrba.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gvlnqopcj.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gghyftdug.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/geropewno.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gtsdnuaet.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/glakyjqhj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gmdhchvrm.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gcfobcnsl.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/ginyunnox.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gvsqixubs.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gdhfadchw.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gklkkbyae.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gqvezfveh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/glbrewhtq.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gtrvbhssg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gqvomxkuk.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gbvlwnsma.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/geghnsgub.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxyticqpi.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvfouqajk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/giuvpxdou.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/goqvfxsrv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gvbscqtex.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gexxulmam.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/ghgxiuday.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/ghlytujlt.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gcdsctquk.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gakqkmweo.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzypudjtf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzolmabti.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gdprthmeo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gvljqfsdy.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gonshexif.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gywattnyj.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/ghfusezre.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/ghlozspgo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gagfzxypn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbsfyodrc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtomaolxj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gcffmkzak.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/ggvqpsrnc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/ggpkluxnz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gyajsgwei.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/ghebhfffp.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/glpyhtrng.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gktqklcyf.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gxwibulxs.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ggdrmlqtn.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/guzrgbacr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gocqugxbo.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gebisjnhf.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gqjjohitw.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gbpftphtg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gxshwxzdc.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gtlfasynt.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gttorufid.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/guacrkram.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gmxqjoaus.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gesxgqwrb.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gxkisyixj.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gzsgrfwtb.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gmgumnyrw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gppadjlvp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gsewhckzq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gsnczzsdd.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gskgmtreq.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gjhrukksx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gsepfvydc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpikgvwhl.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gielogbsr.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gfhgnztee.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gpqzvrkmh.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gdyuwwpnd.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gyhufbhio.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gijegsjyc.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gxqxksibt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gmmpvboaj.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gerbxulaf.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gbzawpjbw.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gkuachiwj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gylpnbdyf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gcravdgxl.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gllkwrpuw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gmhpevdsg.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gvcexwrpw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gadlufjas.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gtatwaops.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/grccmuzhj.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gbranbkvq.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gostoorkv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcygyruq.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gdbunmkqk.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gwjzqluub.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/goxxruhzb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gkgqbakfm.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gscxcifvq.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gcljgmbwv.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gqhuffdis.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/ggwgsncxv.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gwlfakcnj.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gprsjdzro.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/grpoqfamd.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gyoejsgmc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/goyiyiaty.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gavpkcjws.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gbjdzargi.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gxoqrmwzq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gvrntvrwh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gbpjnaplc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gdhdnhspp.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gvmcserzc.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gjmvjwpwt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gbrjogxak.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/guuyteuva.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gtrqsxflx.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gfpzprxmi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gbrereznu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gitsbbhlc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/greidaqto.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/grxqdawen.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gcovtsfkf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gbbtrfvth.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/ghkhkcvqy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gciparavx.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gpollbubt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gtrvxlsfb.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gaabbpqpb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/guqanhuom.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gyiyeeblx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gexbgucza.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gilkjpxbq.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gxpcdnzpl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gsthgnscf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gowhtkarw.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gininwzim.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gogejynhh.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gdlcwyqnb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gpcpyuyyw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gukvyfgwa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gncllntxw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gezgdsdfx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gbgfttvwq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gceruukfu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gfkttaskq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gsvcfyzgx.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gkvgwjzpd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gjajvnetg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gcjtaqfyp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gdijevbgj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gjsvazbit.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gynnhhjuv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gueicmnvi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gihuymrww.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gdpuedege.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gujnvydmp.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gpazbhapv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/guayqfmsa.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/glwlqlorz.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gxjfznvpq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gsllplqba.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gtwlhxnuh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/glbixzfqi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvgicduae.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gtyakkgqs.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gpxrhexdx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gqsrsztls.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gvkssesfs.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/ghrcbzgpd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxupjjx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gngmbutsa.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/galtouhdp.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/ghomhhmnu.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gfvkogrki.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/glydjtadf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gtxlhigsa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gseeghrte.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/geiepoilm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/glktfcfbx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gswsexcit.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gmmzxvivy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/glovneasq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/guzdvyzgh.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gdmraxywy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gourowdnm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/grhwtdhqa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gttfkftox.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gupvgxoyr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/giccadfki.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gpvtfcoja.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gobbfvnja.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gnywaihuo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gkydahxsh.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/grutvjvdf.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/giduadxrw.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gbmrgsngt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gnwbefcai.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/ghhbnenyi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gfvplrpwh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gnnmjflzs.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gdjmxiulk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gdaixlxrc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gcgkazajp.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gcxjrduie.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/guwdphmlj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gzoqddfau.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/ghykczyur.sHtML


<!-- 参考信息 -->