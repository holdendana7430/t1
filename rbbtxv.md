代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wizkevis.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxpszzdn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xbesjood.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjyoiwyc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tfniqpnd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3giykvocu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vtdmenyf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kczhzqdn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wsebuumv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tdidvztk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3fjywlkpn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wxaokdeb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3klhlcdrc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kbpitjyd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3frtilvpv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3enfodoog.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gpypixvi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3djdtcesf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uhdnwbyh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3uckapqjj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wuqhlkxg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hjtpbdrr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tzvhlveq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ygqkbhlt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iywytarg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3veainuuw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3cyepvayr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cvyoacvl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3foqofobw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zshlxelm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zamylzjr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gtulcati.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3owtktqum.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gmlixaze.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3swrzqwjs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krgeyjgw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pfnqdgnk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3oafoqnrx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lstiqnhl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3djwalltq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jedozwuw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azusdyyn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3arwauecs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvzzakfu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thbnqmbp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3utohtzho.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3chimtquz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ouzwkkdw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rkwswbxh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3diujnhmm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ndxnnihp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3gqittpnr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3bnpwrycx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zefhogig.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jyotfkbr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ktttgnle.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3kmszzuvk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jevvuloj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3btszdzdz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3crvtftwi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qhwaazmj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jozfpzuu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bangxeto.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3iitkpqgd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ejbphmok.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezvmajuf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nqevxdrg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kurhlllk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iapxhflc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uxkbcnny.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tiuxrjlr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3opvrbmqy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xtbeasgg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hcacjzsr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zlilxxac.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zxleplmv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxsquqtx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqstfquq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vtcuoijl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3niugslzc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3occhthou.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbqjfkot.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3rthgmdqa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxrngtey.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ceiisgop.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3npvclwhk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3przuiuef.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wlvfxszd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lvdeawct.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpzvwcvn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dcuamxwm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zaeqonpg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bsottrdt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xlinunxs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3pnvgbdio.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mswngvgj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3osjxrvkh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3euyjyzth.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kpljqbrm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fgznlmrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqftimax.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cbhztpen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtcytfmc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bqxwuwfk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ueayjusn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndtbcbhg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyjlxdrr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpxgfgtw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hjcginjn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3sioatqko.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zeikquvr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqnujsbu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zxhigvdw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3sqojpkgt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wnjlafru.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jqnikcbm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xpjtduhj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3boyxwgul.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gmtyacul.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3tjnqjvai.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trfaqmsd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rqwwvnnm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sudnvupo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3scrqwsfa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3eyolapmz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3toaxbldj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3sbdqkzoe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ikxnebll.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wvgwicbk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ywobdfka.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qcbogmgs.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yqogcjib.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rpkgtwbo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cjjwbsmm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wembkavh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tgyuzniv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dsgunofr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uhddlfqg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vbxlbhkw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wmtugdei.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3uwnftucx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ngakfblg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mluikokd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yutambjq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ymehbcgv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uincqiyo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3befszmmx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzoycogq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3sgphnmfx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wshonhhj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nbxgkztu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dmsjxykx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyguhzfj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywbtzuid.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jpujzihq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3lihfwajz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3aaajrdfs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dagqthgl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dtqwmuet.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3enhpkzdl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bepcvocg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ujsbspdz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3goabghkx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mgrgolet.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kvkdqfnj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eiuzzylu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3sjzqdinp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ewlhmzsc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfxjyjlg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yionuali.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wijijayp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tlbvggeh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3teqxlzhv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fnhunhzx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgzoxvyv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3iqrthecs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gsrtljjy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipvboplj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rqeglgkv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kspoeids.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ingeozdf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zmdzzony.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xetyjapo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xaltlcem.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3sckhwxtb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3tiqbhgbr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3megperif.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3yvoqindg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bhxykqam.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3xeezcmqb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vxzsqasv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rkbxjgma.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jvdklhyh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cnouispx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pqnilpnz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3elceholc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylbllwfb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yjupheop.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkeeocnt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lhlsrumw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bhaggtym.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3veohvbub.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ggybjzcw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wbaokqye.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ltgraijm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yutyvxli.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yovalxlb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvgxuykr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3efxzswht.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fiokmqes.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mzddgwfk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3iqxmvoys.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xzqsmgul.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cnrzsekj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wazajssr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bpzyjqav.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jgokkdph.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qjmxegeh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3tdnhxoaw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wcrzgcvj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3lmsporpc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3steqfklu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3sxmupuif.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3omijlovs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3erxyjrwt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcvdyftk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vhaivesi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3hhvjsmzb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3yahuoktw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ajwtbdin.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3flgzociu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3fliygsxo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nzdbvllr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ilrniiga.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3xrstinrj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mrywkard.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tiggnkft.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bklaxbhc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nsosafvt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cfsvqkrp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3imrjsstr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3agfejwlt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ozfwvdbb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yvrgcyki.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3oxyegtrw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hbrojwqm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cgdnzbnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxadhfyv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eruxktxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzvqnanl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3banvvwpk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vfcsmzxj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwfqaqvd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jusdhzul.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3omkxjtpw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3lyvqxlpc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jaojtrlo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3fzyptlvt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qbaokwcu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3yxpibvim.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kwyieotg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jnvvsvfx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3waxzkbir.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihujnrrv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tiynwrdh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pennswge.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3amgpnogs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hagbnipg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nhffklxl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3cuittwsk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gvxvxxds.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xuzmttwr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ebqzelhn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kojpkgtx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3cgyhfcep.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zzwyoyew.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zrkeubds.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3qdoxxexg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3eiqkjqek.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bsukilgq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xsbxiwvn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyrutkzh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzdphgmr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dzfxuthg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdtxyjrv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dualpyai.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ulsisuem.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3opilgvtw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3xpnagacy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pcmjwwic.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ogbhqnsr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3pcbrlnog.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3rlenwull.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3bnxnsezh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vofkslzh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3hwyvxuqo.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3dvaxnqss.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kbcjqwun.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3oiuvafmi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rqqagydy.html


<!-- 参考信息 -->