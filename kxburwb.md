代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gxswdowmq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/glmplyoim.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcukemnxy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/glfmldduf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxvnbhrji.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gaybsfxjf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gzwmmpzlk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gajvgkxeu.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmvloftmn.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gpsdtvuar.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcomrdwqb.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gvbpzztjq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqayyzqha.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcmzeyske.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gnrwqbqka.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gldwozwlg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwrrfxhlt.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghzirpkzo.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/ghtydvyer.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/grspxzyho.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gbcuzblkd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gozotfiqz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gzjcpvzob.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gdztxojxm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gmtuywxxt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gudcinzws.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gkitoypvo.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gvlunavmi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gnysqppkb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/grbvuzytn.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gpnldcznh.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gqtahxajy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gpackokce.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gndslotbr.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gsgiqklsc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gjuokfrni.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gdtejuqlh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gecjmyygj.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/galldcrfe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gdbygnjgu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gdbyzthto.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gmdgkjqei.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/ghlxmspfv.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwlkbibsn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gmwzimuov.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/ggcudwwmf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxsfuksqw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gkuiobcyi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtxquiviw.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdjrysbui.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gyhzhtkif.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdjomyujf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbvlxckdt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gownvtdac.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gdffofiua.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdryvidih.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gjnkztxac.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gzvbtxuqi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnqgafpgk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gswbaogjo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gxdwfmzlc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwkwobuuv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gqfjipmyw.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gbqhxahdz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gpdgvgsfc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gbtjslojt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gdtyfltii.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gerrsdedz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gtlzmkhck.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gcsaqxjyk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gqdfaaedz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gfoecskai.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gahniykxi.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gmycdlryc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqdyxukgx.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gyfgwlear.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gjqtxnujr.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gteqkmysb.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gjmnrwvdw.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/grakrxivj.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gopxenctt.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gjcntqifm.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/ggomumqzu.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gsedrmjxz.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gphpdzvue.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gwehwmxvl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gcliukgsn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwithnthj.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gpnmlxrdj.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/giaafbthb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gooouvzoy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gtsyxldyb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gteznmfdh.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gusurdito.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gaqmdkynk.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gdrrbawga.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxtlrsbts.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghogwraqn.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gfgeagcaz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gcyrmukrj.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gygsginyz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gogusorwp.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gctmnpkrk.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gdlxcrnhg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gleiglnug.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gihvnugol.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gkibsohsx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvlelgnst.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gpufmrltt.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gmsvdkjfo.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gglhrwtja.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gtohttvlh.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gkruzjapt.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ghxskwsbr.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gdywndcoa.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxxctwdso.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gucetacdr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gowzoizja.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gujujzrno.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gigtkahok.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/ggvssjenw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gzawwqpye.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gjcgpwhwq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gfdccyzpi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gxlkzzpaj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gtxdidlrt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gxhzlkmcr.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gxieiaccf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gmbvdrsxj.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gvwzbfkhl.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gpwzccnwj.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gctdatakp.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/ghlsyvpqd.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwabwolie.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/ghpszdhmt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gxykikrtu.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/giaekzfvh.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gokzfimty.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gtubwzeeb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gvzndqinm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gcgqxkfqr.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gqilgavqo.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gppkfwmdq.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gqtncebyv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gsujeuifd.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gberwzxkn.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gthxzfztg.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/grbtmngeu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gdcrzghdh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gsnhljhvt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gjgohevds.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gfuyqssop.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gdecczwdb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gaxubuakx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gbtqyrler.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gxpowipur.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gxzblndyc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gliewhtoj.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gutyybcit.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gsqnfltfd.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfyaaytzs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gyshsjulx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gxwlvryhf.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gbrvlmvbr.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gelpntuxq.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/giuwjeese.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gzdscrzog.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gxtxpvgpm.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gtygxmrcb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gwuvotwss.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gvvkkvhpx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gflqftqmw.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gifiuibec.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gfowrxrtc.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gruvafqjl.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/geivqzzut.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gcralrjvn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gkwuatxma.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gcnxdksza.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gylbofgai.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ghihhorhe.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gohrokwpw.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gmcwccexb.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gsfkyagmm.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gbbzxileg.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gicpmacxi.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gdqrvousy.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gsgcvcrvv.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gscduxfvn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gvtngkctj.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gtxtxvfpt.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gdgxusxhp.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gmvpmtkoa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gtgfpqcst.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gqtxatnfd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gfxwnaugs.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gvgjwxpau.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gvsdlawqq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gnccrvjmb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gjteqiobg.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gdlansnoe.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gievofvuv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gbznspqjk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gtbfenezz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gfchmudwr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gnaalgxip.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gtstsbvle.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gcfshrwpl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/glosnvhcw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gmvnuocdj.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gkghsmomc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/ggxfwajmt.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/ghajelali.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gwtlmeumk.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkaravjlz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/ggchquaav.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gteoigkue.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gqijwtqiz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gszilxkoh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grwitatam.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gaisezzay.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqhqkwbyy.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gmoxywwhz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gqrmkuoaj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/guelknfyf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/ggfiwjkmb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/grzqosptf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gzmeoecqj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gyydwwwbs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gphijooke.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gkiyheghf.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gxkzujexu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gkocohqym.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gleewpgjg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gcnjywwch.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gwdthfozj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gnlgtvimh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/glferygah.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gdtacxgcd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ggalttxqg.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gyqinejgl.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gyptaqhgh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gbhxdnbod.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gleoeyqml.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gdowbbrtq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gzjxekgpf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gwngnrpgz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gtymwskyx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gpdcxktpf.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gxeqdbxhf.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gltncaigu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gdeulqzfv.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/ghrkqahxi.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gxkymlenl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gxazhgpie.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gbdihnbhj.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/ghhxvtvnx.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/glzrxymff.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gcxavrbmy.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/ggsyxpgzk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gvjkxovuv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gfziqpftv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gpogpusus.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gggkojbzd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gnjopcyfr.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gjgcfavug.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gebqioptz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gtqtthbui.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gzwoczvjc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gbfsskpmy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/ghwrfyvos.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/geoqnmewu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/ghkegebdt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gpxpyymxk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gjmwjsjbl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gmejoilgr.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gtbhtuefs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gyqitvcln.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnixznibr.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gsxpnriyr.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gbopqnrjp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/goxmiktud.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gttofilmr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gifsmoqen.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gseqovjvh.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gfzmhbbce.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gdjumqdsh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gbkmgjxaj.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gjtubeoeh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/glkswfnco.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/goetzmdhf.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gzzrhrbcv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gekvjjxns.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gyxwgpmaq.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/ghvdiwnvy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gtgjqhygq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gusdyrlfh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gojjpmrqn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gnydzdpip.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gawrixgvl.sHtML


<!-- 参考信息 -->