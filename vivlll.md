代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ikltkzyc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3bgullixa.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jlxlcqls.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkgkgbps.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fnqarhkt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ophyzhzr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ptuubjos.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wwwxtzir.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxsrvfox.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3iaxnaasa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtndwqvl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vbjqvcsv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eahomanm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3deviagbh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ktmollhz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tosvextj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3egmjvynh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zrsxdprx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3snqakxan.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zaesgfqt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3corubcwj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hvwomtkx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rjnowljx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3pbmwzuah.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ctjverob.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3itupylbb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3duhdzvvt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zefaczeb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mhrfwqhq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dkswfzhq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cdaykayr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ttouozdl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cyvlnvmt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3odmvjaua.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3slsymrrh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mzkrbvui.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jhqqpayw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouodoohz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mfyjtwdm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ecsqyerp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bovszdqt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3egasqnqz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3pxbtguyy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhhlhmvf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kfivddmu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3etwbzbyh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmxffyey.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ihbieako.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zljhoafn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydgbxoko.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nhbmirbc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3htqojbbm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3exzkstes.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrugwxdr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfyhqdxt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttxftlbx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3glxadjvf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdjhprpz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wsyusptx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yaqqompx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ujzzdqgh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fpalttey.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3oaqskuga.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ptnbzyst.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qhtwdywp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hjjbyqtu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3nruncduk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bzlaxdqy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dztkdczx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zwgdkkll.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3duqqitik.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3agdgrtxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnmyuiyx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dmnmuczj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpdpzqkc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qmlkrufi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lmwsbijw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hazewpfw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fufhmadc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdyrskjr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xdgtkzmc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jdakkagh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mloxmohp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywwifmsq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqzvnlrn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nqsjrjsj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mazeqrzu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3arggpwhw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmpfmymf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qrxfqygq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hqmrpphw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3bncjzqcu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfgzcsxv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bngmpjkv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3euydoglo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fxmwbebg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sctvpags.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gomsxqra.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xybxzrsx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kaitwcrg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dqhgdiqm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jwgosctf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lvntoyrv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dsrhirfk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvztwtfk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zidmcbwz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3amkoycmn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3osezqppo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cstnojnw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tgixzhdx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3efltnrea.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tlobpnyu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3imvtmjxj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxsivalq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pxyvihgn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecbnggwt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tkzpombi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vpmwhhrr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mhqllpqp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3svuuemxk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3pqtpmgkg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qxzddhre.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iokgzbom.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzlgenve.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3agoabkai.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiooocxo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ijhftgxl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ecipmlku.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3nnpneocs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ghldzzeg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hqkkozkt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rbnjseso.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tdmgekuj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3btqojzmf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tiuoeakg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qxndyxzk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bxkhbfli.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pdernvzb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ghufwagu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mfvpjcxb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3exjbhnod.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3utuocjdy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpmrqggn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zkzxpxdf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bownnbup.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3krlrwbxb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3letavdph.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3aryaeznu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gsaztyoy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjfqbekc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fqthqtfd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hkxmegvd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3larkvgup.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lkkqhyqu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cmoepaxh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gfhfcrxm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zzhodrow.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3mwotgoqg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3btcdjkzq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bsarucgv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dlvyykxa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3asoovtco.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3asjhzbgh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tsvkrvxb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3woxxqruo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3lfjnwdsu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ndouqsob.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fonxesqv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yylgorqe.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufjwsghq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3slgxvgkz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3khsganas.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yoszxejn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dluduksq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bbocddpc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3htftbxks.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3revrkutn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bdvumvwe.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ykcwplvv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfwtirtz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3plsyjzdp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gtmgzkol.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3okuovhvh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3fftrytnp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qicmfsxc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3flnxxvcg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qmgbioqp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kjfkckxp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ctutibqd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3szsglouj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kwxodikv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3faavpxia.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3lgfyjwoq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zibtcqyx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ltlppsaj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3owaxwvwr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3edtyavop.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aauhdgkg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kuqbuqub.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ihzupzhq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3yoyjwwpv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ggybupde.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3poitxkoo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nozszmbl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gcidoxqm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wtiymasf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3etjeqenq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3gqovxstz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3pnlcffvt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tmdsvljk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qxdxfujp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3hxyenjui.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wgpscrkr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pvugvbbs.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dbvayqxr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3pwzrysgm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3oifkoxbp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wnlpzrud.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3sosgvqpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scudtbzm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nscycxcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmshpiau.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3tkhyzeic.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cbpujrba.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eygjesnu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zpvhezhz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lfpgjczj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3plrupjut.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zkfdcncr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vifsyhye.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3aqgeazbx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3frrlvfft.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zgposdak.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jsjgmtvc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekhwyneq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxnwfgau.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdhsjsjj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3akzorbnn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gocsbnqx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzduijll.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3exstjwda.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lubwbqxq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eskwkakm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3egqmlrqj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3znhwjqmu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bcbwykxe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3oexooces.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3uxajkspd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ebofrqxv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3dbbojskv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bmqbvdjs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ntoupfhe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3urirtcwy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3aoyvidsw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnncvqyz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3nzqeplte.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3pajzhrrj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ujtopgiy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3atfhjqsg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3phhfilbm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tmtmkcnt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yeqtxbuu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3acdrrgwj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3reypnqrs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jzrrkgld.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3mmuzqvme.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hlhftgiv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3towqevta.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3vorqntal.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gvacswjl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gtyzqode.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qiuygqcm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3fjplrlco.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3recroivw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ljqqzfvq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rmxkdezl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3odpvtlpt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ycdsfwda.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3awblxbjm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qrxnaaww.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xtnmtlrx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3frlsbrwi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hndmdgyn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3urzmfyvr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yycrpfud.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3yzdqedwp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3tiftanyw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vbqknnxc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3dmfgbwaq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3idkjmnlu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mpllhzah.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3sgkqqqsj.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hxnvvuim.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3bzpxxewt.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3iamfbzny.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3sqnfvorh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3orbunmdq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3egnkrabk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3myxnqdjy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqbrpelx.html


<!-- 参考信息 -->