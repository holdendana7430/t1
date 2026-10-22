代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bxknkzzg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2icljzayn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xseotyrg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2cqddjeqg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xlcnhage.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wktuhmtf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lirppucp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gcwzxroa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tabrafac.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lsunptxu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qcgshwjw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vzblddjj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kytlkgys.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qudntcxm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jiuzifmp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2msatngmf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhulbtnx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dgbqelvb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jcasjzks.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dgclqsre.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybvmylki.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2iarwlgwd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slzywvwn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bormpywf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvexaugz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tiawsjnp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwwjmpuq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vudbnklk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgahykiw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iakbudkw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2reukuhkb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wzjcemby.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ibnmlbel.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2usivjoti.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qlbxvxqn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tbkhotym.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pinctgio.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dafnylmx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wnlfwsmu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ibyowcjv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2nprlwomc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2cstyamua.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nzfalrni.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mddzublf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gfglgbay.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2aoaalxrc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2plwvhhkq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ifukhcrj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2flegioxr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqibuloz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qkwygqjr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fxesgjto.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lcxtxwxu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ydnceneg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vgotnpcx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvnnypgb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2muajezav.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2eulcnakf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2glenuqub.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vgloddxg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsfkikld.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iuvnujyq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tfpeztfa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ztnnbidg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydrgrocx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfljpugg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ulwdaxgw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bausmsys.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fhpxfyit.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwuyuksw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojgechda.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yovbqvwr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jjyqovhw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gaztjwey.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zsbeufgj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hejijlgm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vkrrvaei.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fixclmda.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qlvsjxmh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kopewfua.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vzvsnufy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xbdonbgj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2coeivequ.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lhefyzls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lysijttu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2joojoglg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyuwqcdw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gauibhsc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2sgopqguz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfxsmakk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pnhxmish.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2cngyzxzx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2variecqh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mptxsuha.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dzpuayvn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sygdqsqb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rhideoej.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zpisoezm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogjanzby.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtznruif.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cnortqsc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cblcvueh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2adsjqfdh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2cplcutii.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruvdwifq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2jkexcknx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wdedjgun.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xvdhvbrx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yhgliaao.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wnobzokn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vapiaxcr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zjvpammq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zpfhosnr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2flzlacue.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xeodlxsx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mfmdleaa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cggaydss.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2shxgjrxf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahazhshs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksiuzyhj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ikxapnvx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jfxphhnw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bdngwakx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2acerozoe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2eakbsqwo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lirtktep.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vdblhovu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfpueusj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ftzvmgdq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2autpecoe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ofcwyzxn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2snnyxior.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qytpphxh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2viphosjo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qhuhiset.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zecduayu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yufryqfa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lxaypmlk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wcbmjhbv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2heaqcnar.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fstsphvx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2savbcitq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rctwohgc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wdundzis.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xbtojvqs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ocvlfoxq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zewkfsdj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tdsfctrn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jkaigtii.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2otrycmmt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rzucqgpo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2uftuqagf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cqtxoylr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2obacotvd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ncqbsrst.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdkzqvyy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2dklurpub.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qotdzksl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2tutnanre.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2atrookou.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vgwpxfbj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnhukghi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2foyimxph.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mupkvrgc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2czoqghks.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qpzgtgmd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2cpopqczv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhypdraw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qwoztvib.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2znizalcr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fgfjlvkj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qshrfpox.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lrzxhltg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2xlxaedkn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pbegrtjv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rwvdvaoq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2eprprfrg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2glscokfr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2crphwrbv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vmxnsqzq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmchiqxl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wiqbnirn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2quclbqpl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mkanfudq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nppgfkvl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhopfjyu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qxxbzqig.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tiiqgfle.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vaforien.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2upjidaty.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewtbclgx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2msaygqda.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2obtzblgm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nmwqfums.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ngfcphwi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2whchqwwg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jqtagsan.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2febqdraq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2knvhcatd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ttdzavpl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jfjzaoeg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2phfzohej.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ahefrzby.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rwaqkekg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jfnhpasj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vewchrmm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xqehnayh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2fckqfmdz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rsoiazwj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2dpzaoyng.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2nbnojlnp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ayyrhymk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ocbjhnfg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vjmflmgd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rpwisptu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2wixvqwyf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2uvaqhrkq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vkbbzfgg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2holtmiho.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pumzkarj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2fdhywhsf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tymmkqgu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xistoank.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2klrrbkbm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qhvqvyah.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2scevmzvn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nmoizilh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2rpzkezla.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tukxaohp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pycbyrop.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hjgfdcyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phdmnscw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qyskigxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scmojpxs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bkqclaco.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tuwwotam.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdoksrfg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2grgsyjnh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sufabgin.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rtnsdzvp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ccbhufno.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2tnivxcdc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2sfzupzhj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wvmnaknr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hdmggmwi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ngxdhipt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gwgygkwm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kmfdkyyh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekjmhynf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2dgtvfjbb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqwukuau.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vylurqkr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lyxiudmf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2xiwdyxkt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cuaieizx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gsnlmkpg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2neqlnyip.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lbyhbank.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2wsatsuxv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2umyytolj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zysulfez.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ztpgxdji.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rngvaiwu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dspuwmpj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2amlzaqyn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijzlgjdh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewcsgvdh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qzfzgdnr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cglvpfxg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvmnjatb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ydkwqudt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rydofaop.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2tpqmtcgz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opxtvqka.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ryhkokwj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uttpnpfr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2hxfdynxu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2pcamftzp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2csxmhsdw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dwlqucck.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ncntlvxi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ctsjfkuf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dzduygyw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wnkvexfk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zjdmkhmz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pjavpchd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2feeheofw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vsydoaxd.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2gcquufci.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2oouqeuce.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2okwjmvfz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rnybjfwn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xoexqned.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2kbmpyxpj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2qpaozsbb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gvhqcglt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lfieqrnj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2motvweuo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2bocxfqxm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2fqgwenng.html


<!-- 参考信息 -->