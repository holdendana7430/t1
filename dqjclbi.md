代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/glexmnsfo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gzlstndmu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gghjexzpk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjczmlurq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghpjgdhaj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gljifpnri.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gtriyypmg.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfcrsxqky.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gufowbtym.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gyvfanrma.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giaigqzyp.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gkeclyxap.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gieiifgyk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gybhdhzbf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gykveanln.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gloyukyvj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glvhcxtka.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggopuagiz.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gzibnxvrg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/ggnfkfcib.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gqvafobjj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gnumwczjy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gaxcgmlau.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/grimikjwz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/goxtntiur.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gpyhvjpcl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gotbtjawm.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/glvbdwmvb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gsblnkxcp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gqjmtubpf.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gwtipvbwu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gsilmymrc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gazbxatrn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gxkbogzzp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gviczrxhg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/guxmwqiqx.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/grmpwryvj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtjtqosia.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/grcuiegzq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gjhsjjtvp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gfuwpkttw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/geytpkpfp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gzlidtjrm.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghnzzmwzb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gnmqxplfj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/grrbvxtsv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gswevlruw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkoynszfp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/grmcdivfu.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghcwarkem.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gnpxdtlzg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxrihjqjs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqetojzph.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gfwjciznn.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gniwdcyow.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdxrfcndi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gmvskzdil.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gtzsnyxcw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvebzcmha.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gdayspadb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gmalbybzp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbhknyrpl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/grdjthioo.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/girmfdjth.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gkpirpnhx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gguxcpers.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gamdtjgld.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gqyzlqrfc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gduckjmfd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gcxlitinz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/guvqqmfet.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gkuahmcce.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gndrsmhrc.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gzsnhxodr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmlsaouuu.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gejuzxaai.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gxnvoklgj.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gwtbxhmry.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gcgnzdlps.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gxrkltnnc.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gulmebxnd.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gmwtqzpra.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/grulopckd.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gastsyaqh.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gvnfssxtu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gjnaaaykk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gzoarxgcc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gfcpujbkn.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gbmcbjfor.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/getivdiox.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/glpymikca.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gtbabzuiz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsulbthaz.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gkekqpusa.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gksloffzr.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gsgftznlc.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gmaqracpc.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzhqkntba.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/ghwvxoijk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/glkytxaze.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gzjklkcfz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/glbbywenu.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gtozlnecb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ginbxogov.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gxlecnezl.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gxxgyspgo.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gfozaxgfu.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gywlobifs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gdaburzee.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gnyvvyyxk.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gvzumjwfr.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gknmqamrr.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gytsdnkdi.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggvwxgmzn.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gisysfsjz.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/geomrbeim.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gyjtqjikd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gfstwxahk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxeguifoz.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/goimlqraf.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/grcumlubb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gyqzihovp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdcskulqn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwyilvxrr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/goaaixfoy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gmntcpxil.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gaagedxea.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gjjsttioy.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gcsfljssx.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gjigugdtc.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gctabxank.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gqdhmdqkp.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gumlivrrw.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gvmbmjvrm.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/ggsgikkyn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/ghasscrrs.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gaxksvnus.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gbkwcvnov.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/geubtxray.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gzgtsjwco.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/geheleebq.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/ggaxrrvqu.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gcydlbhqv.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gqyekdpph.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gzijzjnmx.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gyqqrjtyv.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/ghlqxqvcg.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gabmopmoo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/ghnwqqzlg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gghisfczb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/grsqnkcla.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gofmkutyf.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/glodcejoz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/goweqwpaq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gsbqcbyql.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/ggdjxrwtr.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gyczjjsjs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gicqwifny.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gwuxtbfmp.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gwkcdwnyw.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ghrxdvbnw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gsdgyfcdd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/glkyaojku.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/grutpndyp.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gjtzsapfi.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gtquudbnh.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gigaowoua.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gviwfzvsq.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gojeatsnn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gnjfovidg.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gfejkouft.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gpenxghyx.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gksvhdopj.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gimwsvrkt.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gdsjpimxv.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gwvknpxqw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gftzuztjt.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gwpuzwhdh.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gdkhvkyiu.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gvelcyvsl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gnbzpkqgf.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gzgwuxarw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gnejwzgeo.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gberefqph.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gbuvscvwf.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gkimwcodn.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjzbvufkf.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gfstdoyul.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gtfbodczb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gfufmrija.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gyvyfjhge.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gsdqmgofn.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gkpygdxzp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gsttfbfvs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gxaugrshf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gecdnhoxi.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gmzytmvnd.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gfbgsyyfz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gygpvigit.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gdhhqxpqs.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gmwvveaqd.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/ggnguesfz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gbuosudyn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gwtctiofr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gibzentpz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gyeawpgyv.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gpofwlhsu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gwkvgornn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/grkediqwb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gsdznclax.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/geckoegnb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gxfqhpnjm.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gxounbqxf.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gwfateppz.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/genttxopi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gvnpiapgl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gqjdxuabo.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gciixooxi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gyeeencvw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqkibtssr.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gyaspenmj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtgevqfxr.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gqbgdevth.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gmubcyprl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxiqjpees.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gcjuaivkd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gzsufqxkg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gasskwqnk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gdflgbiqm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gsueagqmc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gvzpucakn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gfbmgoruc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gujzvcpjl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gbpplbkcq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ghnnkeyzd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gwevagrkb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkdljfyrm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gojmfuewu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gxmtmlsgt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gisxufzbc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gxuczvryc.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gujpylron.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gkpcojkkf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gyybmjoki.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/guhtaplqo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ggqnwixva.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gsfzctcdv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/ggzzlbksg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkqttpuym.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gyrjdiblx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gyocjuatr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gikydxncx.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gcqkilkms.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gyuawirwv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gpxrbduea.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gkdcztwrb.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gtkckdvuf.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gjrxiygls.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gkehnwabc.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gooxixosy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/grfvdchau.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gzhsnxelm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwtxogwvr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gkdnjlcva.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gfsjbomtu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gndfweqfz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/ghfqrckea.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gjkniagxy.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gvfdommzc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gpdjggaer.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/glffspbeh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gulvnpahm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnuezxgx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gfbkpcovy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/glqrrjjjd.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/ggwnobutv.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/garqvstsm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gebylsgql.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gphsvdluy.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtumhmwfz.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtpjrxovo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/guqspbmpz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/girwskjyv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gnjwqwhwf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gqpoxrmaf.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gmkhnczgq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/ghvvllgfo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gamqfnmha.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gaqohenuk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gdojnwqab.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gyzvzcbbb.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gfuonzicl.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gflcxiirt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gcmjuslbo.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gfuwboomp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/getisqlzx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gikukjjoo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gwvnqermm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gnmznqwyg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gfhccsise.sHtML


<!-- 参考信息 -->