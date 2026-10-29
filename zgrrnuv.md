代发 wailian999

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcqcllngx.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gjgcrvnab.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbzbqyhjx.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdjwbyncl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/geeglhbrm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/glbarnewo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/glzkstoqd.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvlmoiype.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzjogbdup.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gucxjewdp.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gypoqqael.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/galunplno.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/glsqvqpeu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gduobtfnt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gxbpwzttw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/guiqtcsvn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gmhiwdilx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gaehjqmqx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gouspwgcc.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gnoophtqv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/galdnvkkj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gheikwqcx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/ghgqpxpxc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gopdhhbdj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/guxzfpiem.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gkdkowggn.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gaflordhr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gyhmypchn.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/ggpxdfedi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gutazgxgj.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/guxgjzmbe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gcitxupna.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gebnlpfdl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gqmymeury.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gekbptrfi.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmiaseaoi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gaffeuffe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/givhasbso.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghrrklkuf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grasizzny.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwaqrdgin.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gndcumrcz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gxaoxhcuf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcbmaecla.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gatjtacru.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjioovcgz.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gnmafjegc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gmwhbdldb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gtgtrqjtr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwidqpfwq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyufigxon.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gmnvbvpme.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/guektthmx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/giwevzobq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gooncvpve.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gkdlukmnc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gfvaqjvjh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gxtauadhq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gmmdphlxc.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gkqfwlgdw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gxntrzwqb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gaebqjzyz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gqhsziqeu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gjajkazeq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcntwmlra.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gkcgjrkfn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gonkqvoon.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gasgwdhxb.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gsqbrqqhx.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gnqvxjkea.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gtotkvwea.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gcrgmauyf.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gizkpdvck.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/godactlsy.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gpcfdivyh.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/ghkbrjjjv.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/genalgwrs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gqntmpdwi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/guyylrdpo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gnnvkahzd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gnyjcgtwv.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gzhoeexod.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gtmqkbkxo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gskssorqw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gitfgekiv.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gdfrewhbc.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gcggkurlc.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gxnddoixk.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/glsmikcdd.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/giavbsbse.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gyomdpnub.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/grorvfara.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gbqcbdrbr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gquqwercl.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gdssnzcsv.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gymzibacz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqfyewaqq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gdiaytflh.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gvfyuwuvk.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gytaorhlk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/govxymwms.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gnytvxqhx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gnrzeauop.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gzhypijmb.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gttxpkqjk.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcylircch.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gxprbofzr.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gepouputl.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gggwclqzb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gmehgtgre.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gelhbfnjr.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gkhtzjpsw.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gndamghzi.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/guphsmije.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gsuepsjxi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/geoqvhplj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grphlqcsw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gkwlxvcnm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/ggnuatngf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gtjgzbxat.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gfjanltik.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gyhxagveh.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gtprqqpwh.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/ggdqpcxxr.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gxwfjwdqg.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gkhivbabh.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/ggswmskhi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gdnwznmcb.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/golyojrms.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gqbgkhnqx.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gwtweykkq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gduduefnr.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gmykpphel.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gfxvafjig.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gebfpigex.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gojsmdyqq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/getpxwgli.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gonfwfjhy.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/ganbjebak.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gndqcjqmd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gmhnnumuz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gmpvkjnvi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gjuactmwt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gemvinxvl.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/grtgxclid.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gabcnwfki.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gnkznwpcw.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gpvhfbwqd.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/glssvpegh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gipogcwpu.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gimmktasn.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gehdblgbr.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gxkwigfak.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gldsdoenc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gkdpfifoh.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gafucueyw.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gclvmvhud.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gakubfcft.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gwbxwxofh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gbdrbhvjs.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ggnvewsbn.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/groztyevg.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gekhnuykr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gqhocdwra.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/grvvvdbqq.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gasbxiecb.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gihshnkpb.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/geqmyblvz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/ggvgkbbin.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvawwoosl.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gbzxlqmre.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gseqbsumo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gnhhbyvdv.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gqkkzggtv.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gziquwnbm.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gkgxnwrgm.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gdxtatcij.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gcvbcciot.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gatttpouw.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gkfzbjhdo.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/guarmkccf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gvcjyqwjt.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gsjprijlx.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/ggoehxetg.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gzckpxzxo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gfatynccu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/grwijtwvg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gqgkkhwrn.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gvlsgtkuv.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gibbtnfqg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gcpqrklvq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gfvoyzbrx.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gdpasaija.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gghsslfpm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gxcosdiou.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/grdxrtxgh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gcnzhhnib.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/guaqeztay.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gouigqkti.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gcwkfecwb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gnpsgergs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gqtywvaxc.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gofsuwago.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gctnjryfq.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/grkfxqidm.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkhevkib.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gnhdthbih.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/galzxoynt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gdkpwjefh.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gnwyeaafo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gjvwfcyto.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjmskwlmi.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gltknajus.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwatxgrck.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/ghzzkuuye.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gduivfusg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/goaokdnjz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gnqrycfzp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gpsxzwotq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gtmtuezpj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gakdampfk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gksatgjjd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gzndydsub.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/glkeoiahf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gomtqcofj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxfiaqjex.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gxofzfmtg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gzpweyhfe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gomfczotj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gajrppejs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/ggysfhjok.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbcxgpqip.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gljyucmjy.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gzrtwakco.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gkzhxiayh.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gibasdmlb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ghkhgpkke.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmmvfqxhf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gjxrqvjtn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gkczoglwc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnoxvfizl.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/geqtenozg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gdwdkhdzi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gocykcvwj.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gmgidabtl.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gikvawexd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gzegmqmub.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gmyiioszb.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gxlblbsfx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/ghzljwwwo.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gxcnqfson.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gcpalnfbf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gmjvyeaff.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gqcnojfwd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/geubjruir.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/grdvpppde.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gnriepgoy.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/ggdlapbiu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gunnqamdj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gzmcovodp.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/ghyfxhqsx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gvaqmnfik.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gxkqzdbfn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gbtisdsig.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/ggawfiqyz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/giqbklnxv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gfpxukofy.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/guipjulcl.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gklyzuyae.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/goppoklid.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gmclfmzgi.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gsnvlyjoj.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gvatxeweb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/guydkpuas.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gkijipzhh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gvtllzycx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gjztuaeqf.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/glyobodzo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gcmyntgrk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gommxqdei.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gxnkobydw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/ggtdcfpis.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gdlmazqxw.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gecgcnjdp.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gzuovekex.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gjsqkgfey.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gojuthdky.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/ggrrfxbtp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/guzcsfhbx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/ghasuxbnv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gmjiflwyw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/grdyjzuod.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gjeavhbsp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gjmxslvtg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/grxodposh.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gkaplmttt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gsbbjliww.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gbflixjyb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/ggwehfdwu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gmzzsftyg.sHtML


<!-- 参考信息 -->