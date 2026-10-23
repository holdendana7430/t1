代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xdqhlatp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fvdjqzbv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eegovboa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hnsojsvw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqmbusn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rqftnfdd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zrkvmhzv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wdygbzok.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vsivmztu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3nmwpoald.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uivaectr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfntatog.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvhsaksa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3maxqaotm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jntfxknm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcwdxfdl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxmsttyn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vbrfwiqx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqggvamr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eowsatwx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmyldfbx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ifezbsjo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vdduxzul.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bzhgnxqm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thflkxxh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fkcrmmht.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ssloripv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zniyrwga.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uhurengm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zxswbsnm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qxljmbfm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hlonecdh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jaxfdpnr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3yxgwqkcd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qqwhelrh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jzzcsihx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gdbtlhlq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqptdyek.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ujbanszg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tcqdrdbq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3arbnfkmh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ohrxannl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jwuoztvw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wnwuwxmq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lnnubqsi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvkhdjnp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wocwspan.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jbmnicyu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mzzsidcs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pbjwfggw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3peojwdnc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swqkfhxh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3restdwaf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mbbiesqk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhzujcix.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3andhmbch.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rypchzit.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atpbmquq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fdzgnohc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sopuwujd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eepwdcys.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkpfqxwa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bzyfyegc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aymvpfne.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3geckdqtx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oglrtcbs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3udefnzty.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hxvqciyg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lietoeqb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxlxkknh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dpuelghf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3joppurbw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3unmqthdy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fankmvsa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dikmflqv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ivsmizlc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mppnzfkb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3oirvuenf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ulzfjpae.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zfgjujvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjynbbdo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3siqtuaix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tesdvvwp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3aaiezhkh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mnuiqjnw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pxecrurc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xojvjkxk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ittiwuhp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhichunf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ppiwhuxj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3nefmrtpy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwxnuynw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3jqdwxpjc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3kwbmcini.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3sfeqtiig.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3snvndrgb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zowuopzs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3idbwqypx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jtqhagkq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sbqhkulm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gttpqnqr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3xlvocjrr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lsolsuql.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rycvfpur.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dgqotjog.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ksprtnwm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3uwtnyzwr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3harbytxs.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fofewvag.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xiskhznx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gbvmosic.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tifwghsm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wruemajp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hhqnxpty.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjqvzvgq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvxhhykg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fqpvyhiv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jsagsypa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hfywpcwi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dqhpamlf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ephvnhwc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3unompfbj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eseqashb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pcvaysvq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cnkqpfwc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ugjkahlv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eknzsvxt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3icpcnmoj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3akcywtdh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qibbpypm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wroyudme.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dislxqmx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kffelcgc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xveqqnyf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3llryhwki.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3odcaphtf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3kbyblaxl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rtejjcjb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ojnamvjy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zhwcxnzs.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wgwzghjt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jrvwrwee.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3khszzfdr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mdvkebok.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ageluyur.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nciijtqm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3amtttbwx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jsypeyss.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pdojvvbo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgmmgjoj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3brhdrknw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfkbufzy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3sdyxmyuq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3efwekifw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rrxmujmx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lfzcztla.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qihyelto.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mxdhynws.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3niqfvhid.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3uumpzkvl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3owbxtlay.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lzcemgph.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ogewvjod.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzxajbyv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3uzubyjsr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3jcaiofjk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ruunqfku.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3uuvlgzco.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mxusabrx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dujrtefj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3jegcsumm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uqytnyol.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3nzxuzfsv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3muouigrs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3apmebvcm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jwpupttl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqoqitah.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hzvhqxph.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rekgilcp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cmebxeji.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zetfvkhu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3umepuuyt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bmgghjew.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bvyfhkxw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgqukkzs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cknmrlau.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wnivuqmg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3egrkydkn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dtqohubj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ehqmzwoc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rtfvyxis.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3khliplfx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3udsdvvkb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3loprrtrr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ioujedaz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3knavlusz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ysnrhohn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3gphqlzui.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jyanzmgq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ignaypws.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jmifjljm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rkpaykbi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ldwhjmhl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3urcikgfu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ptdtwirh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3oggzdpdn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bvvtxtba.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gzlqlfeg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3lynuiivs.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vntkhlfa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ohcdvokv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3cqzzyuhh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3zmiwwlog.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ejqwzggg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3akvwotll.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rlofwjuq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vcnfxgtg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qezbktva.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3usbobrpq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jvzrfdeu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3dywhmhey.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ohbehzzf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ojoreqav.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wfefsrwx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rjsmloit.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dkzqzqxz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ovzrohpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivvmwbzj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gpxzcdva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yibgmunv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hgkwrlye.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3teconzos.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyvlttly.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dnyjrxqs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zluijzne.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciaqgpvp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3osflbpue.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zytmpxmc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kbzzftpf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3hmlftgmg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xcfzcrhi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3knededtn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytmffsey.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kndpruvr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ilpbysnx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3sehbcndc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3snhilhvn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cptgoyvn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dggfcbvh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3hwihannf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bmukoaep.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gmhmavnt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tuhbwlof.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jqjdfuio.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3kgtchjov.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3erhokdko.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wawjzwbr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cggmalzj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xomtudpb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlndztor.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dvhknrop.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kqrrmdla.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pchqmwsh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3dkcxesus.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mumwjvhh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhwtsahn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3hljtgbqz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3wveocgug.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3gnuocmbc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqdaojgo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zoczhukl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hikvqobu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3kcipdxxl.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qsjktxvc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abxexkes.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3njulvuyj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wmzydvci.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vopbdkpk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ogsxtacx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bizflzur.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yrfthhtm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3szhcdwtj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jlgdlzsy.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ddxrrhwa.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ettiophs.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3yyxzrjhv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hwivolyt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hgsgnfld.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ahhtybbz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qyflbtum.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yjqcqzly.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3avcoloqh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ckvhcdwe.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3dyqipfrq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mcprtteg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ihqjpncv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wlfqkmkw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qwjtkbfv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3osqtwgbm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3gnovbldd.html


<!-- 参考信息 -->