代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3iwuzpywj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3loaaqwxq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3plvngixh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzhudsxk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bctjiqod.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3krwngigs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wfmtbqap.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgkdsnnn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlptutzl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dpnqphfs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fkelcsvj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tlxewbbn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ovkjwsmd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3annhyobj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3spahzsui.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sauyxhze.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yaofaqma.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vxmtsotn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3yebzetia.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tlhmcvaa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3npnqusba.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ljxvwwyg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ijdfarni.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wontjfvm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ihhcmkeu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vyouohav.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ofmdabdq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lijgydkk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tqqngjhe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3itrhnzcl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jaivpdpj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wqacylrn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lpcrpzzp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3aajphkxa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zsymwqce.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dvvfvldb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3kcgjgflo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqumvzaq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kejkexle.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pbytcniq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mansgjsh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lifjdnta.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zxrxsxny.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3efaxakqk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xmgdxgjl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3bnqttjlm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cuopsxvt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bxfkviwi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkqdcivp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aerbambt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kjezlejt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqkxahai.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aoafldfi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uocdyihd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxfwmxaa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqhilaix.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3imohnytr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qokhljgh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dcpshnby.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nclhnvdj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3kuprrwia.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukhsmrmi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qghgzvtg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3sfjoztpb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3aydydwmh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3pwudaflu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3pzmmalaj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3eglsxhdh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rlgqmgtf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3thbeppas.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3itdfanmv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3pavqzqdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhdqcfzk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3iffxdghv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqipdriv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qratvfon.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3psdqkaqi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbamvryj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbyjdafx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3glpxwmks.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3auuxlymy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3nhqeioxs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cswqawvi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvzonyfn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aciquoqg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xjzcernu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yicryemu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijwkqjdo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibsumbbk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gkzxakbl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vpkuwyru.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xglucuzy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzqqqzol.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ahcpyhma.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dktsfafn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cwlvnnud.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yibxslph.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jmaicjvr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3pwhorgci.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3oiuzrhgh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cbziyjka.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dwguhkeb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mansmdye.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3amjdxyzi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeoccagz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gauktgnx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jqrsttwx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cslqurhm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fwyxhaqj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3izgxanrx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rwaoxhyn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3synztegx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3fmdldqzj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3codwomvx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uoarqajn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lreozdqg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttaehbma.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uidztiio.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fvghjafj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dzczaokd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3gjpepcuo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lwomevyw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3splrznmz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3illxkpkm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rbfjehev.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3akperjgz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rxwghnne.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rcnqcqgm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3nenlcgrw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vryjofzr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ttuthoso.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zunwaiin.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3awropnpl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qloflyye.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wfidvotd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vzydchhh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dimfnxsu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vbhaiyxz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ikkyhehr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vlmetbep.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3mpulwvkl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufxeiruw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmtslkjl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mmzpkyhd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3psxujqxj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3nbwdeiii.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3lvrwfvhg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3damymewl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3nyboivyr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3libjwihv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xmxonobs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjipelfd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nkktvyyo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ommfyafv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3enaerqqw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fzrlvrpu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fwxhntwb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qmorrhre.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nsncmxik.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ffoapxwm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hxnuiezg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3uzbxxaos.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xksxbixp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sctesmfh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3igfbqjqb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3sbbovilb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ttxdliwd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edqehwlr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iqdlepmw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3utgtobiv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjqzsjcx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yfawthhk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zgczmhnf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mipjejpu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kftemphd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hipquued.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieajumhw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3symatsoe.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3osrxpepm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3niestafe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jplgwlxg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3strjpexk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jqeehknw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3eerqcjrp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vbwfnkhm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3njjgmknx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fzloylcb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ddqhknpj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vmgvrnbg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3uncagudx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nnrizlsv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ajghbwew.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lhsqbvbc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3sgzhxged.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3udvdglzh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xrpekivv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jzzkwgai.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqnalkxn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3xobenqei.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vbbittyd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3pybilabk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ahqvprhq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pkvkwnot.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3nuptlyus.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3eckiyzle.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hzgvqfrv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zztwmzse.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jarmxlvb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3bxhnhxyu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lutajvzi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dbzstnvf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3oneojvgp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3yqswjtjq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3duihppyb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tlpkejfh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3adcwqhgh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jbhedghn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lzolnyfd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xxmxlicl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngkrikqh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hztlesdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftqckgwa.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ggkuyqkh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3dmeoixms.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3yvaqsspu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3smmznmrz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnbgnlpb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dkjmbyfs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qqpjprgg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3uepsxnid.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3njssunit.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3hpaaxezh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3iqumcabx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mjwklwae.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bimgwuhh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ercwgumd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpqzwxii.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zwxmwnjh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hgsrqkof.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3idogqnze.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zugmpidp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3orgsxcpb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xdxdlnzd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tbnguvrh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cgenehye.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qvxbnlwy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ozsxcmaq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3kjgqvieb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pgspxfor.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3metlulje.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zdtlscas.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hninfqzf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3biqrnsji.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3exdfrpss.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hxsjjrtz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3cromgyvw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3qnyztxrp.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3sdtueqnf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3fjtxvtfd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3psifttcx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ydoldbpa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vecltssv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uxgjeoai.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qipimtwp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3yawzxzqr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qlfcnemc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3puzyvezo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zsamoffi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3tgacfhbd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yqqcfpbq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ljstbbjz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zznidlju.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3lztbtqvx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ctornpzj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3udmyhnoa.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fpheyduu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ikajkzqu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fyhsnbja.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dhugkubp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3evbtrmlx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oqhlmlhw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3eynceraa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ewyprdgq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3evebgxte.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3twcfiwuw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ahcoeiim.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3nwaakhpr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3prwhsfrz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3pplgedjh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bfzqxriw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zsjccsdb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3nmybziat.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ygcvgetg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xxomkunj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ijgxsgyi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3jskyvthy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3relvxfjr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3gmzshedn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3rbzbhhby.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3silxsxam.html


<!-- 参考信息 -->