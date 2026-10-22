代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kptoowyy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2txbskldk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ywuhwruh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pmgjqvlc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gcakvlth.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qrgkxifd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wchyfqdg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2eixvvric.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rwyxkets.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ejddhfgx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rdkjddxc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vsfmqqub.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pdagfvfy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xdutspyg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hdlkgcge.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zmmpcjcj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2myabbfkd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wtuqxezv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kdmtnvco.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltkqeugw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upzeggic.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vhepqtcj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pvuxjdhk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgwqczkp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjjgvxyx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2swsisfxr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owwaddci.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gvcxqneh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ogqyxqnk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwylnffq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2odatojms.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mghqnoiv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2logbpaqw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hugfbotn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pnknkbye.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wxovpjxc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yzwxsmud.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ppbkqkpr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cvwijodc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qcjxneao.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2yigkqyqu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2gbjftgbq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2nwxpdqhu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2frtvlkal.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2cblquqzq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dfilagqe.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rohmanjf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xdzijgub.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bgjzeuqw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2sicrvfyd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2whgccfrb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uopxgnhs.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2yyqablbc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dipeoiox.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wfebfmle.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2llwlxxgr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wxmgaspj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gljbxdmf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vdrduhda.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwaoihon.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rbzxrnuw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wcllnyvz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2favteqmc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hrlfylex.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgeptbzs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvqobghi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xuahoicl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upscsetn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzudsuvz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nlvamxtj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2brihgaav.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgzixzhn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2oiuptjux.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhhlnutd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rlypamnq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jfjtnlbj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2dyxntkrz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxokpkvw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2lttykamn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2sgwgfglp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wsmlazat.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mdynvtjq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2oifjfyqp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nhuptjpo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2khqzovhu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ctovqgzy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rytetvuy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2nqmprqbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukbhgvyd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pakboexh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcbyxtbt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dcjrtofe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2gqzwkjgn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjrgqwdy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxtxiesn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjgrsjgf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qilkwvcq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2orzmedyf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lgyqazsx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eavhjysm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xvaroyqd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zrchgmhq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2sxpvefzv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nrveldef.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tqsekhqc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxbazusr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nvdlrris.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2geyquqwc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ukwllutd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mpvdwjcl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qsuggeyd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fcbfdmje.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2okqigxle.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2fscmllst.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kkyyimlx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2kccaxxrg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xepcrxbn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qhnfhqdz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hjolaruj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kfjicrdh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hryfqbdv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2adhmxnnn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2txpmgzqa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bkshfxap.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uankdcwu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2faiathjt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jpwnunqj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2faduxain.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yhfmgdrn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eisyetpv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmmqpizq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hiliylet.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2beyjfvah.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hflxolus.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydfhyljt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybenqpfh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2klgiezut.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wvdrikmd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rzpbirov.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rayxyroe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwrgpfng.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ibmfakph.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2fklqvlbz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gmonmoix.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2lyhyjkvb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2uehbupjn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2kiqprzgn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2flvkepjk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2agayxdkj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2irjtdicj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lqcoksaw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dghqnhne.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ycdganpy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cjumjosj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2squycwfd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2koszowrp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjecgyid.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2remnqjqz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2acprwojt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iolyvhft.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2muamzope.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2syiwjzuc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynywxako.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hcaxybyb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ryratbbn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dbdtomuc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zpabdyyg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2kglmgnrp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mvblkxef.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2diheabaz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2gvxvksbp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hthcsxay.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uqkefleu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2cademsjy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bzjaetud.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mhyegnwl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bghblbbu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pvpgmxog.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qllnhyjy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bwbzzypo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ykmsxixs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2litjlreq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bwooavhs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2apdrtrgx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbbzwfig.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfcvpogc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsyloguj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2noirxxpr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uhisxupz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lruontju.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2qqpikfcy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xqnxnjku.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hynphuqr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gtisyxlz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2roxnuiuf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2drzoftvl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sdbscunw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wcbhqogy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vtdabdos.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mpwpbhdr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dnbxtpzm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2igslixai.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yitjalih.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sqexwhmb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vciwsrng.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2yyvoyviz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hdiyxgjm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2sermzews.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2idthhskv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vypuaswy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2cvbifhtl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2feafvwbh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mqawfzmp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxyachix.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kafoxgqu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2luyembki.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jyhtrbyf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wzzqeyoo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2esxeegej.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnkukoul.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hvlzrnur.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gycgkbvg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wyliwzld.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gkyxzrkd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wircabpc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2acufmdaa.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mwsxusuh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gqsrlscm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wpvtgzwg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nglruiqt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vlxtelcr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mqgziqih.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xgagthwc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yryybagi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pvlcfnsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uztlrfzm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ewzbdseg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzqlyuru.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2uvhunflo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eldhoqcn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfgewygg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eksseqwe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgogsnrt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mccxiewk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fknacrwp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vdonorkk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2sciclktr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hifnumgf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2lduqzvix.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdotdklx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lvuokogm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vftbcnyu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2guatrzsg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2kcywoiuh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fdcqenlf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjyjdfjl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sdlfnjwn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2csdvvtpc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uhxlocbp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oocxqokp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ruvhxmyo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wfviqjbr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2iszfubji.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2dguyaidj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rxdgnmif.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lpaekllu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zpfwhwas.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhuyszcq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ynvgxvcp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ywcirjbe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxjwzvcm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cbvwlotq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bujnvsca.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2htsoqwdf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fmxdisqf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2solkzvor.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xrsjetfx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2uhnybpbk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iimnyqvi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rloigmib.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xquskajs.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2kqfoonfs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2gmtbuhri.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ohjqzhbt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jsqswyli.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dtmyvpmc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qtvnjabk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hhapnacc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2orkqiuny.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2gxkteaqc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2jhuetrgl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2haapqane.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vmwbwnkx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2xfswdgxg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kbmeeijq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dwsmavoa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hqyophrw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fvgycoqx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2kbxmjhja.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ojquqxrh.html


<!-- 参考信息 -->