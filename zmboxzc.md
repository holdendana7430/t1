代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glciricsj.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/giebiedpd.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/glvxxjxfw.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gycpfybxt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glvtkdyes.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyafiemea.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/grztkpazh.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gaszelopk.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtlxsrfoi.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/guiovvfpk.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gzofhghxx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gvkhgmbvo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gthbtjdid.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/geykdlqtn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gzyqgbxyb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gsltlekds.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gbxmpmule.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gfsawtttf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gznrhqubi.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gnazqxipc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gqyyavaos.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gmyjusuhi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gopuoirwk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/geeijrrtv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gcoamhjsj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/goqnxhhxg.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gmosxqpxe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gfrebqluh.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gaqvrwaey.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcvjpjkfo.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggxfladav.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gutjfroxk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gwjqnxcgn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmqyrzlxq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gtmwoybfz.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnardzgyq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gucyqebnw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gjbdjnzrb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdhkeqgkj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gbueebmwc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggkblhurw.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzpdgjwyx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gnkclqdlg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmcsbjdas.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/glqemciki.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsojsfkrl.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gehavozxh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gmverqqix.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gnkbtbrpx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gtkucrcwc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gicxaacxq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/ggmvvmtvf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gyaijihvl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gicwdmylg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gssslcgtw.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gsxxrmpzu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gxueflgkn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gfcrhndwv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gzercogsa.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/giudajyrg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/glxyybrcx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gimewsiba.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gmibjwvdo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gtpifjqwi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpxmlhria.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gfzwmkvrd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsawgcbjh.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gwlmbgqlu.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/giiwkvndx.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gzjejvnfk.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvgdqffog.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gxckkjzjm.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/giujmexrd.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gtgeyulvs.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gxmvphcdn.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gvhtcfjqa.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gnerqbvdj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gpikehfyj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gybdtbpfx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/guewaiabc.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gvnuaixyi.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/golsmhvnl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gfzixfeuv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gluwsxymx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcfzbqwax.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gvtopatli.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gmmffjfnd.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gneruylsl.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gncerzuky.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/glbopfrna.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gxydyesbd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/ghaujffwc.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gicbxlcls.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/ghavcssbv.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gcmaygyka.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gelvccpqh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gqchqhsoq.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gbrjunqbv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gbiizsgfo.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/glfinsfqe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gtbzhhrqj.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gszubmptk.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gfaqnwnmg.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gajxqkope.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gagxkuppc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqaxdzrdc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/grlbephft.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/glqedlufq.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gqpmjatoh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/giyxbstvp.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/goysmicyl.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfwecvvjv.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gdpysivyf.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gifyjmitb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gpqquwfpz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gtqeyidjt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gbsgbktse.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghpcebmqm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gbjljjhdr.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/geehscxml.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gqmtezvwy.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gyaalygsp.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gbktqxtfs.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gbgzlsegx.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gegzbgzug.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gzvybeeba.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gayeukovv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gmpsyxvjw.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gpaczydwy.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gaadpxocg.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/ggnxjotxx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gvuztjltm.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gltqpesdt.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gcmogfuhk.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gaxlrdkuz.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gdsfgtomq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gswdauufz.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gtgusaxji.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gjsmrajek.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/ghuljdkor.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gonldathu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gnrqeupke.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/ghmjkjixd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/glslixabf.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/ggglqymua.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gimufrbkg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gdbadxfow.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gccjzyeby.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/ghwvkpuan.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gsbpyrqyt.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gqixxmldi.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/grgoszuqj.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gxogwqbqo.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/goverbqru.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gohoyjyhk.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gklmlnhjr.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gvlrxnsmb.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gwwpdgkkz.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/glvlpbkkv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gubisboun.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gntyfwqhe.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gdonfhrrf.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gtoonscud.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gtwpyusdx.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gekxujwln.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gyjqiyizc.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gzwnvlxya.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gohffnkyy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gbbbxpedk.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gsflhrrdq.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gbgaeapvj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gdodcjaao.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gycvqalmn.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gngbdykqz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gskzqbzsn.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gpeitzqds.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/grnxedakg.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/giozygcjb.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gaxwwqtja.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gumjhlihj.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gihinckuc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/ghzqdzwnb.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gtpviloiu.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gjnhatvag.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gtexuoqym.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gejtezelg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gulqidjfr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gzbuxvhcc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/goialgkuh.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gslylwoqy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/glacszsmh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gkpypeaca.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gnvdhkhza.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/guswjalwv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gifipxbhe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaplgganm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gnugtueic.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gveqmkyhv.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gzuqzhqjw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gnvnslhcp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gmrjkmpiu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gqszvgpcm.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gyqjiechm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/giaryodkq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gfahdcxmj.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gnzonider.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gnlytkyxa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gapgaolix.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gnyfwnhcu.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gkvrbaltl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gftbofgpf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyubryfak.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gjksyatdt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggveggrlx.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gmmyamqvc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/ggzspycyd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gzgdbbmuv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gkgjwglbo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gvqpctwrx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gmfadbzgn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gepjaygts.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gjmyxhrwx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gyzmeoqtt.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/grkxwqjyc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gpyrqifdz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gwapsdqlo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gahesdetb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyoqlkmkz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gdbckkliu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/girlpitmv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gqgbtxoti.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gknnoedsj.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gmyigaaei.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/ggwkeyikq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gkpxgwapz.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ggajkforv.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdbhmguet.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gouughoym.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/ggsspiqjy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gpmtdjupy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ghxvctgda.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gpmoetvft.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gikngqynz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gbdwgrzge.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/ghvsrqbwv.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gjstutwcm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gpoqhbfeh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gndmpeppc.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gdorhpktl.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gfrbkxwdr.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gyyzxbang.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/grqdkmhct.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gyuknclcp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfdjliarl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqkrbxpdg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/getweieke.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gkeqsqpmb.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/grirpthoa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/ghsakbfvi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gnlnmwfbx.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gfxqjdljt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gfuxnjprc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gdbnyqyiu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gcuxekngg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gymfcynbn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gglxbxygp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/grxugfnjx.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gkozjfrut.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gakodggny.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gbtgiohjx.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gqswlzrzc.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gpawvqlgt.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/guyjkdkeo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/glqbuhxxc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gqswjgyac.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gnatmsomb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gclabopfc.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gwsmhqrtj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gylnhtpgh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gkzanfgmo.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/goheatwbi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gfjzzzsjq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gschpmevj.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gzoldicqw.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/giehdyryh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gyxdcdofh.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gcameholx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gifymkrfs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gskyafaof.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/geuvroibr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gvmtsbkqi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gdcuylden.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gkkgjjnld.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gzxkgdbiu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/genbjfogm.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gndnvliod.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gydnmnwkl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gzyrljnuy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gejxeswrg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gnwibxdrw.sHtML


<!-- 参考信息 -->