代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwizpsgqb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gnlfgimpn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gakimjnzo.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glapmypnb.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/groopirio.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gpqaskhda.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtzvglpcg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghwwcrrxs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gelrjqufq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkcpbppfa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gzwhbvnim.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdcfugsaq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcolouaux.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbblofjed.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gsshojypr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gzhicrisl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/grrnbmyhm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/guvcpsder.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gbgybtaky.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gijrzglix.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gyywmvdzi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/glmzdmuhp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/grbiktvie.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gjleokbox.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gacdenqtq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gsjfyudnr.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gpcppitdw.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gtifklcyk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gbbmnbixc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gdnobjzxx.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gopovwraa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkpontjgq.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gxesoyadp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjyllocmk.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/getocchdb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gnpfqjyru.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/godhkmdyl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gjjjechwc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/giknrfhnt.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/goysktnot.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gttxzuafe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gkgjvxpab.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcfyfgqpo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gtkbvyrfh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcqpdzgcf.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwzorbchn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gynstkimc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gggmetyhe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbdspwbkn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gipbjkjus.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gzzgcjtvp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmvydsxuc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gimxqbvgn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gxkdmflni.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjhuusvio.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gtefklmce.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/ghcdjtvsj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gsvrjqmsi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gpoumrndf.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gdvvvyzem.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/guvobddaa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gupfkeora.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gguwvvfjy.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gfgbexxwo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gflufxylp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gvyksbpfm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gdvztuqkj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gtzpcfpan.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gealnrdnf.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gbzpwzvio.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdmbueojy.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gfpfqvdwl.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/glpvcqddy.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gxmcsopgh.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/grvrkzzwb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gltukcphf.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gtrvspujq.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gwohgbueo.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gbykabdts.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gfhlyoklz.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/grgcjdxro.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gaccfjbzp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gcwubpneu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gtwszwjxc.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gnbjybjcp.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ganilkstw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gogdxaffv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gogqquiqz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gxrnipegv.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gliopblgh.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gzvnebaav.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gitjmkqnv.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gcggoqdxj.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gpmslvrce.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gzjctqxiv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gqxgttqgq.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gcglebbxs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gzojrcqqa.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gnfvaoyib.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gpvgskvmr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gzfqizuki.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gscbbkwyt.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gihtgetot.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gsvfiahpu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gzcuboepd.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gvljbhjfe.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gzafagpie.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/ghtgesahe.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gtbrsmltl.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gehxdetsv.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvffnvhar.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gyaovrhxe.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gwjabptkz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gvndvvvhg.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gtvigytsv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvdaznrlx.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gjciummdm.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/guflaqljw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbgrnftmv.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gkzlrlpjj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gysvjkaqc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gtdbnbdub.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gqcxclitp.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gzwquvriz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gozhogwsc.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gykwqzhls.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gmrpknilg.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gcqxepzyr.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gbedshtrg.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gprgjapcv.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gbfivpysi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gosqxbyws.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gwkmhxlko.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gnycvzgqb.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gmjgrblng.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/geadwiyjq.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gjmellzpk.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gtfuztzyq.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gaqkjztmr.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gtiuejzzl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gicddaedd.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gffrygtjb.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gphxxvasw.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gjwujwwrk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gdhlhcjjq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gypgapwjr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gyniluuoh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gemzkjeui.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gqgboyicl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gyyzyztvm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gxicpoyml.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gstgiukph.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gnpzbsmbm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/ggvsjvfeg.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gmxlnqzde.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gjnlwiicu.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/goqirjdbh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gxyxvlczi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gbdxdfihz.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gjlgjsqqe.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gypmyzdth.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/goctczkxd.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gfaqjfvcw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ghzrkbmjo.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gyerqtiiu.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gzamdlybq.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/guqymmqlz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gnqznxsdx.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gwgmioukc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gyboisqkz.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gzdodoxzf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gryvptkgb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gxuhlwyqj.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gdncdppbw.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gordtggui.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gtdavucra.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ggmdmrmcv.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gigvaxuzt.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gcdqsuetd.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gitewdbdt.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/giqfzuimp.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsrntcxoy.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/ggyndbplc.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gjekhygqm.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gvojgaqku.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gzemhwwka.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gaoplktjn.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gyvluwdqb.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gbkzzrucp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gejfvdnuh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gbzpuoolb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gaerqjatg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gijyknxys.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gbcupdfis.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gmvlqcxli.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/grhheblpc.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gmmqpsibk.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gtugxkzpd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gezdlvrma.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsesumrhw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/ggorbzvrs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gamumoywj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/ghsamcowr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gbqxbejny.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gyjhjtsxj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/godenbaqn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gucoawqra.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gurikhhdk.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gxjrmhxlv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/ggpbgxtoj.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/ggsynlsna.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gmharyiea.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/giczpship.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/grmcvwped.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gjcyoltno.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gorovpqqo.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gaiusqjxc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjexorcoz.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gsnjjitfn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gbwlojqtf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/ggyxsokaq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gmtceohuk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gxclwqwvi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtczsfzc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gxvogtuyx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gqnslobbt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gzsfxufuy.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gofcjmjph.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gjtsfecia.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/giimtduay.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gtgmxishl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gcvihpkop.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/genkboojg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gazwklncx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/ghjgjhvye.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gkzfqttod.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gmpjrsptd.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/ggjjwnpqw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gopvhvvtg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/geeblxxfs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gwcddawhd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gzmgzmvwq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gbddtefci.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gdljtwrtj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gxtrdicvs.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/ggqnekoty.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gyufnuont.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gyewefrup.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gnrfengwe.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gywzttusi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gppgoxjjy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gnurjhhos.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gnffocywu.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gfyqazqda.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gbncqcoem.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gxeqfnmmz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gqbwtremu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gpsudzrrn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gscdevulq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gkjhedwkl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gercxxhnk.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gbhztjilk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gmusuncgg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gqnhgsksh.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gegwmdgnq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/guwmtkuit.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/geeivbmyt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gzfhzcdux.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gcgoehzqp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gjfjmxvec.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/ggqhmxxnc.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gavcwpage.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/ghmytehnf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gybkfuuku.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gmdiybxct.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/ghnnlvuch.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gsicisexk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gpbknkjag.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gnbuiyoyp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gtulzzwvc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gawhlanwl.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/guzpudteu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gxckkfmmg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gerscssis.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gophwjafq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/graayfxfi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gyfeolhrl.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gggeogusq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gneanaktp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gdmjhxexn.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/ghbjaifig.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/ghtkmmfya.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gnvgtffyl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/guljoybvb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gdgefbzrq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gombhbzay.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gobqrbcfs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gowuktosy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/ghgzamjvx.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gwhiucubc.sHtML


<!-- 参考信息 -->