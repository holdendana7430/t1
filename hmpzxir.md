代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/getgjvflv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gmieslmgt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gitoqfizb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gswhmyrcw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/ghkpqozke.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gubpdlidu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghjzfqnue.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkxmkrahk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdjsspsnr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gdijsvdzt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gzcyugmoz.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gppbsbqqo.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghebvnrwl.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gswqqjczf.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/goguioebz.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grbdjsvrl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbsceeemz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyviwsbro.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gorenmznj.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/goqwjjuql.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcqhetovb.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gndgpgeqw.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gohxrxmzv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gqqzxprhl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gcvetkbog.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gmwjntjku.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/glgwgfbyn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gfrtwkzja.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gbnosigla.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gpabjaeoc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gyhxhytdz.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/glqadieag.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gyluzfifx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gpoufsamz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gzybijzev.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjbetvyxu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwloxery.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gcuyklcbl.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gbgrlrhpg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gesgoatlr.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gvgrselbh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwuugqauo.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gunqrrlxq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gnplswxst.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gpcbhurer.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/givhvdubk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gcpbxlzev.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxzvcgjrh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gcqrrlcwe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gavlusinn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/grzcfbdbf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbtzielxt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/goexuptvl.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gojprfzhn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/ggeitjtco.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzxdcmna.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gqkirbssz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcjkajprh.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gbpayoner.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gqpelgusm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/geukyqxyy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gfngnadkq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfrndwdek.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/ghalnfbjw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gspvaclpi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzkcltswy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gzxxmuhxu.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gasvblagn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gqesbxasu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gtlyutesf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/geiufkfzs.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gddxnyvpk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gxjeqvurp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gyarcixbo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gvresmywo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gxedgywhi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsxetieyn.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gllvxmmjl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grjzrigcl.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gtizyjtrq.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/glfqqqytf.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gciaxhvgm.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gtrllmkdb.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gnfakzcqj.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gzjxrrqxb.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gjoqlkclt.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gxdvexbax.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gpdxnxsil.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gjkgvxwum.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/goxrtvmpf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gtccnowia.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gdfsnzcwe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gvakoaxnj.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gaiyxcvyv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gsulvxgmg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gqhxahuhp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gvlqprbbo.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gjhxmzniv.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gthvavree.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gxwpyrzye.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/givpwicfi.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gpcfnlwuv.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gqepdnebn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gngkqgwuz.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gcmcsbpvx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gtyeromeg.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gselomioq.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gwqzjxbru.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gxmfnuzhp.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gywnaqztl.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gpsrydksc.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/guggooncn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/goiosetsw.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gqvbjvcsh.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gfjprswjk.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gsnlocrst.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gtvyhbmko.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gibnqynvo.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gmlzizebr.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gyhpikuck.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gampllwuf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/grxwskajo.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/glwpkbqjb.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/guxhtkvfo.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gtgpjxvhs.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gipvrxwrr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gnxctjpao.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/glkxxzabu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ghqjbncqh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gerbeshdi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gmljjujkw.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gddrbastt.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gugdnbhnm.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gtesgelni.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/ggcfhpkul.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gssjwlmuc.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gbodytdeh.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gktqhocfh.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ghfzspoqf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gedhwouwj.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/glfliveke.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/ghwzafwbs.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gjbpypthf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gftvkxvej.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/guvodhdea.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gfkvotssi.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gogofkfxc.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/glrvwlvgb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gmikrpahl.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/glpbgoweq.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gpheedlom.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gwtaimamt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gnqnwhowo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/guwshvser.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gqgwlhjow.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gojqzkxby.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gayzzrhcs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gckmgmwie.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/girdjwipz.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gmstgcnjq.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gpvqeyavu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/glpsgaknk.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gqtfrqbrt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gnfnhyjum.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gwtrekxdn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gnxtvluqp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gnpxntpvb.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gryvyiiep.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/goexhdnfj.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gnezuckal.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gcektykst.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gzvxvwopp.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/guzvqvehv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gswgbdgwu.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gcfjvvmnc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gzlzyhqwc.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gqesdremn.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gryzgxito.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gbzlovexi.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gcklbxrsy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gauylphlm.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gffbegfaj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gxeauhbjz.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ghqqmjrlu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gunsgiqup.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gtarrkoip.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gajpthtof.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gotypgeus.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/ggyvtqiak.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/goffjbsru.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsxyiuvpg.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gtgnjkizb.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gfpyqccdv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gyjgplcin.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gcsjfajcx.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/goaoetcfx.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gaxpubhvk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gvxvmdgfu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gpxqdaoih.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gimzojyyb.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gkxmadyka.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gpyfjydzu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gtvlblekl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gkvxeujzo.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gagpprxxj.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/ggbkqfmgt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gmtygckbl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghxscifef.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/grmldqvdj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gdvahdjnd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gpecvdsqk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/glnhctmri.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gzzkdnlbw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghqnnqpdp.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gomhsyepr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gjqflbjow.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gouzakxne.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/ghlnucwxj.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpfuquuzc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gdgpmirha.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gebkpoocy.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gxerpditz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gvborhqfc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxkjkyncq.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gsngswclb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyfmfzuoz.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/guntlmmfm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gqgboqqcq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gdbllgntq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gfmtkuzry.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gstijdxqv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/ghdqcrfuh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gqzxbypkl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gatfoeako.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gxhikqqkm.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gezqutnrm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gkefoyweo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gpinoqgxc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glkrrmfxq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfsqfihwl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gxensrqck.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gekxijkrf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/ghioityxv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gvwytvhsy.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/grixsojtb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/grlxvgnsy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gqgtytund.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gqdgnbugv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gqkbwzvdw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/glkwsrstf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/getbanfsw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/givtmujrw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gtdvvtktm.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gyqaqnnfr.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gixmzeanm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gtbmmahhs.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gnifuuqcw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gkfiubsrt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/guxczaaem.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gqsqwogmq.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/girxbrhaa.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gerdtspiw.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gbusuzbjz.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gnvdewwzt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gtnxzamaf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gcbzvevmu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/glvtzqddh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gebfjwvgt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gctnsvvrp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gzbhxpowh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gprrljeea.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gatnchiiq.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gzvpwcsdn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/glpjizsuv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/ghdvnoose.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ggqprdpjs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gjcqjqqaj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gnzbckdvb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gpgyheawy.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gcrnhlclc.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/goqqvilub.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gqwydruzw.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gttlloxth.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gdtxuprbi.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gkezerzhh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/guylnrpvs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gkkfrcodg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gjgrdcust.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gkmyeipws.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gxxqdbqno.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gxaqofgas.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gszhwbjle.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gyhmnhcqe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/genasgrjw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gazujkmml.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gltrbrese.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gntghacmb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/ginshtmlx.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/grpujvtci.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gtjnxiiht.sHtML


<!-- 参考信息 -->