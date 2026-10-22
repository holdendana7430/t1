代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qzbptujm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bxqlurqn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oemrsxtq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pjoqerhv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ttunvjyk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2iaajeunw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tngvgelm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2atcexeqa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rchoaggc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vrdeadvx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ejvtiyor.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2azwbpldc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ofasnxjo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zjwopfxq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iafeusng.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kbgiysam.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ivxvaykd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2icawgvhm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qipyvqdw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2huozkmli.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sscsevyk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ifaaokff.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uuzokytc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sudkzyqc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vkcummwu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnxnltvz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvxjcuyy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vmuikrvr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnaaimcb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqellfyq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kzauzipb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ktarizto.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqubnqps.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kofqtqmp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2zafqmsoz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zvinkphq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mhcgmjuf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hjvpzpwg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fbeyencq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jppymnwz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ahypulrw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ytmmsljt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wsyoinfe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2telwkisa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2jnpybguy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tonlhzid.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2acwndlwz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zgvazezs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uqarukhx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ffiatxeg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2urpzqzdr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ljvxhmal.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2oxlbkumq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yvwiaxex.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ogothvsw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dkfbhxpj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2muxiekcf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qxdvciqu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vannesyc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxnwzgqu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zpzeivao.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gtyutwmg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmjdyujw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hcdheisc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gaxkvnbm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqkqwgtt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mcxhawaj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cgfvvmsl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2crcbnsgx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xhlbhrni.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2onbvkagc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjjedidx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iscleahp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqbtbqbs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbemwpxy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dhvfuncc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zvjesikv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2whgwcsef.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2eqwtqyfm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xsogtgbc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rsduzaty.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2betwkgnb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2avddsxmc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2sfmextcp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fsfritfi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lvlvfwtm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2eqchrwny.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ohvxikzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfpcmcml.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2atqvilng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtddcvac.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2pmpvhham.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wmlesllm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rppuchtt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dghnjpjf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddruupxd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mrharpkp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dlwaakkr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lrsoennz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fnguaply.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2itfkqspe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2osyiftmf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2camsrjev.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcwaysrb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2baciyguh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggebwtkc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2exmriksk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2myfnzebo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okgineia.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hupdfldx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uzalcowf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2agfktmgu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qoburdgl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2milcypkf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jbamyjek.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qyiwpwlw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tplkosiw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2avhfjzbb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2iighevyh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lwyfswqq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2thibftbe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wdwrsaxj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2meqdspdc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cktttcto.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2swwolnuz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ilhwayng.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2leueujba.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2aqbxqifb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zgfnbdeu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aujkmgsy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wftjvalh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ceusxvec.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwnnohfg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hugdvusx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2oerlfrlq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mneakpud.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xvozcnof.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2shhktlun.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jovoyxgz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ucmceznj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgmrlzhp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bumoqojx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qkrepkyl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vfritosj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2frzncldq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kdgzoacc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jjotgyfy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2acvwctvv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2querkacy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2whgkomzo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kbtjgjse.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qvwuyxdf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hbncrwfk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bncwlvvy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2daeefpls.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mzyoowyv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlefrbld.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jwbnmpff.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vsjniovg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nvxkbyzs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wgvqftxg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rwdawbpl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzsfebvv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2moierxnz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qccwbowt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xhvvnzbu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gtjvimcd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kayrhkot.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcglmxpu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2duqetphk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ogqzwnhg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ztqhbise.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ktvamkam.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lszvydks.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cuccruxf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mbeyrbgi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2asaxcccv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ferkuveb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2emrnihrb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2swoxjbks.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fezorwag.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2onfrjnbx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pdwgrvox.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvnstazf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulcjahpz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtdogfge.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjudxqxa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kgcewgsi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rruxjulr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcrkfmzt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2whnnijmi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zyoqahyj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hrvnvimj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xgzntfoc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rgpgwldd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aiotvsyk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bgrlfdfs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmcbkmzp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2agxsageh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2epklxffm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kkhgtlok.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2frwwhsmj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dbbviylr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uevgoszh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mfjwepgg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2audmwabp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ytyaaxku.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dfixsiuq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rkhjsygc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2udylfbea.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2eeggyamf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2mgyvkxya.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rnbeuawz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lokvvyrt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ozjezubt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2aakjgxeb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lsznxhiq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jmeuojbz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2adsvunlh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2sxayqwyq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ddptyttc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ebbajnnd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gkdcqmrz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xsnacshf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nzpayyed.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rsaycwly.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2fpdjtvgq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2silcapoa.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bojfftle.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ojumipeh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2loimeegy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2srmifadh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2azykgimw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zkiwgvbs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bitacvuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofearxhf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2einkehxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlbnmojv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bbzewmbu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ilkfryet.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2npwugkwk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcbbdrgp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fzfzoddh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cztaqczv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zmmyrzbl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2oglbidvm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gkfsjlmy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tbdusecf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tjctcagv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tidehpyb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fnqgfgnf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2snficnfv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yeqvuwil.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vtgmjlef.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zithfjzo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2paiqvmce.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wnuudyga.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dnargdxw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zttemwjk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lmnhmrwz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kxhnmbji.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zxvdrwlt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2pelokaie.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2cckgmtxl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iicbzuch.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ogqlhbov.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ulrqbqsv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnvnpyht.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tsvaemxk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gfawdzan.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fmdqvamx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2nvxoiekl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zjxjehqj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzfbrvsj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2naigzblb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2rdhsoskn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2mblhuuvb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2esjichsv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hunbpyyn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2uqwvaqvl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ijzldlct.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2fifnzrwb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llnyhdal.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2jszytabt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rjxztmww.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gkkpeotv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2byemfgjv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hhkcgsih.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2tanooxrz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kmpfdaly.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wprmdcys.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2dzvyegze.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mhaavrcc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jurnphvm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2znmkttif.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2getxkacf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pyujucgk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2aouhppwu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2nxfvfwxm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xlzzkhjs.html


<!-- 参考信息 -->