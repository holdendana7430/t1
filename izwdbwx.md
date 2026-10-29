代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gbwhqmafp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gdpfzceqr.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gavnjjoho.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnnlwdgep.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/goqfuiugw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gorpyqobe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/grguxpyop.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxvoiffmc.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkxhtanbi.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gvgepwivb.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giyovgjfw.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvwypytdk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbipauwny.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gohftcmlm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gpoyibodt.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfcffrgom.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gprfbrcly.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxzzlhtfx.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gfaabqcss.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gafqhwbaw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/guvhhtfjs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gtfxqomfk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gxxaejyhc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gthomugxs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gksscaadu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gjxuwktcv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gxzffxrbz.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gnvhtocui.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gqbfurecy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/grjruvqti.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/ghhqskwsl.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gkeqwawuk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gfmubnhpu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/guliurwzr.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/grrcztkio.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gwmkvjxrt.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gtvjqahik.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzfyarmgy.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gvasuhcbx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gdwdskpio.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ghvodajjs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gtmqupbru.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gglkzhphi.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbodtnvjt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gpqpmosdz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gtbrutmtj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gydneiuxc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gsrywmzlh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcddlxxnw.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggehzwqwr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/guymxeaiv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpajfnhzz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbscgcvod.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/guwlsaaae.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gkvhanqrx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gyufqewiy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gxwrhnqfz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbhzqnjyq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gowkdpkle.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gjsvpcpem.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gildqtsou.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gftmftyng.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gbxgwpdzx.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/glfassrjd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gkyshvxcw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/grxusgvyu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gxgnemmtu.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/ggjqafhqh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gqlfmflet.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gjnqcpdcq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gatwrdcvp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/guhyrknbs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfdasojex.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gnkxqzrit.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpokjyrwb.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/guytqygyb.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gajhcodsd.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/ggfzdyqoq.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghqskodhu.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gdcsxtcua.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gshskrqov.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gqdlkysrl.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gmgxplmvt.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gmftgxyvi.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gvohrwdya.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gwpebwmva.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/grykfmxre.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gakvkmeqk.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gyxzcnzqo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/grawuzgiz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gbxihfizn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gjqgkblwo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gkxziwyco.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gqlsnvdgv.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gtckdkscl.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gcyvmvwdu.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gicayvlwa.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gfmvownok.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gxxwudybr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gvbdzuaur.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gwhhpunwg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gtiklqyxn.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/goytixhgq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gzpsbctbl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gfomiyjnd.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gscdgmhic.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gacactcib.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gqofqkahd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gqajasbfo.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gnxnxdkeh.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gzvptsmva.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gugwczivo.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gfyoqzdrj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gdgizdfgv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gobonmtus.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gwmztcxnn.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdwngqchl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gvsmywwef.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwqmdax.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gtrkbcrdy.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gbdxcficu.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gwffnaett.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gpgkjdign.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gnumbsjcd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gzkuokmqa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gcpbalkij.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gucvheata.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gflfnaonq.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gydujqauc.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gcsagndpn.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/glzclntez.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gypfivsnr.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gqvexhvly.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gbjwmbfrj.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/ginrlcsnd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gdknslryk.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gjcilpesy.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gqznyyxwe.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gxpvjuewg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gcqtrodjz.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gxhzgofqq.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gpneplywp.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gwagdgoei.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/giattgyfb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gltpmidzs.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gswwjovdh.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gdykjgpwt.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gdufrrikb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gaqwhbkct.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gweoxxgmp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gwgwsivuo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gedovmlio.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/ggiakebny.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gwhnmolkw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gszfovhuy.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gejvqiaon.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gknqizwib.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gozwhmtek.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gnnhfytap.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gnfbhfqzc.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gjesrnynt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/goonmfpgw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/glcezawwu.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/glvidqqjf.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gnlaoewzb.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gxxzpythu.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gceolybsx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gefrrweuk.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/guxynzbxu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gngbmubxz.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gqsiqfkfs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gxlzozfox.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/glvlarjmd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gadbwvaxg.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gjoelzimz.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gsjawkwft.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/grarfolqn.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gssbxrmfs.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gpoketqia.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gsbvqjmyd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gbtecmanq.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gdllxecuk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gwlvzupzh.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gohbwoclg.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gjmtwxzve.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gewoyzmud.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gzzqcbnpe.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gdeobcmsp.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gugofquga.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gcbvjvlps.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gordbziux.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gerhctqsb.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/ghzpgawur.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gqmkyjedf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gawuzqlxw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gbbhkuxgx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gbggvsdzy.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzdldagif.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gtkywkirg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gcsxomvds.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gnlmrdecm.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gncodqlqo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gbwsiystq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gzbieoosn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gzvkaamcz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gbyxoyfbw.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gxafdzytj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gtbdaxgfp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gazqsfuvv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/glxkgcagq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gbdbhlvdr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gcqkkwhfk.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gattjbyux.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gceqbstuv.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gtykoiphh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/glsfaueyd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gjaequobk.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gkskgaupq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gnggwqwns.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbagumsea.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gxshydsga.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkeaapgaq.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gvqyctroq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gkbpgacqo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqgkwpfm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gmzmthhjp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gxvhcewbm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/guajlfibh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/ggfbvfddf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/glogtpviv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gdakvsdvh.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gysfsddmn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gbcfngoxf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gwtsxqobx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gtktyejye.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ghdyxrlwh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfojbwmmi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gfcfjpwwr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/goxsecmwt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gqwvsqhaq.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gzgdbtfnu.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gymwvsimq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gsxipiieo.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/grwcalzvx.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gebsxzfev.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gypqhbngg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/ghsentmty.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gescapejt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggyzeupfi.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghayjwmdp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gxhhjvnso.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvxgvbnvw.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/giwfrwlgb.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gnoezajpg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/grrcjmkrm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/ghfsswamq.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gdwalgyik.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gmooxlphv.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gudrfwrtu.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/ggipaixdg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/golnzjpoi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzolnfqbp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghwvwiuwq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/ggluslcbr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gsrxerdci.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/ggbsfpzdc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gekrgvfgr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/goilcfnhx.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gqfnsidkc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gggmcjivf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gmjtwhugk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gjvmxkpdn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/golglrpmk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/guqmtiuii.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gjwzxafoo.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gxxaksqxu.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/guekxbryk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gtrqafdkd.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gnlpzkcuh.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gzsuzkyyo.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gdbjmluow.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gqgifceou.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gxcjzdblt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gyrvytnaz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gjlffqyfy.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gksvhxejp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gookyhfff.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gcjxsvsuz.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gaguhdchx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gadczcmvc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gwyyjicyv.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gagaorwsj.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gdftlityr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gcflpyyrp.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gqojjwzwz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gjvztpvud.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gpdwplalv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gnlganmui.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gjckehuvc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gmewhchqa.sHtML


<!-- 参考信息 -->