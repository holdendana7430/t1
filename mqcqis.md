代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yasimfbk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qouvszfe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jcakougw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpuevbly.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rjrzvbpz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ooxjtlwc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jztwaebc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qpawpufl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngrexzkn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofxawzwj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vyeswtxf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lgzgmjuj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2urrwbtus.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2eubeyvpu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2pjtfrntw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bzeyudxn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hvmsymbh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bjyjcuxh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gkgnipta.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fmlppqnz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2pxzxsbja.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kvuazjuu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pobtglqj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2cexlbwlw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rsqjqonj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vcgauapd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ewkiader.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2oitnzlem.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2biqxarcy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fpexjtyk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2doiejmwj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rrtbmgic.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2pxxchfeq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qngzajeq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yotnhenb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujvlpapt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvtzbbfx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eumbatgz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qeicwzlb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bbfslfmq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkqagbvm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ghwfuncq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbxycveh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lveibwsy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezntganv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmrkxign.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fopqndgs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhggfzgw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubmqaeta.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rvqxfepm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ofvsdhvz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gcoogkfn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2breokcmp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2eucmkodt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2alrkjlle.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ozfrmwdp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vezcmzhd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ifdthyst.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tqmahykq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xpfxphcd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zykbtzkd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pjbwxnor.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ooqgxbbx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pyfcyzpw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ukulqqvm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2haiyzkdm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2mlurbtdq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jyvraixm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pehnucby.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqpzecec.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bymlxugz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pmvdvvba.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rzymlmhn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uubpwkth.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2slpixgys.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmoqesud.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dtezyvpt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xleohfej.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpvvsqkm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dzsfsgwo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qureugjb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jszwmgec.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2otlvvzia.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aveknvjn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rajkbvkf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwdaldga.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vavjboeq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnxmtahm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zlvgdnmu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zohizkgd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plemkibm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eibtntfd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ozylsoxt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxpheuag.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2cszoomkc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qkuyoyvp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kqrqpcxu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2dvxotxnz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hiraqgxb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2isebgdll.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rnpvnfsy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xrqdoxbk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mqivpliw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ropiobcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2toyvqbnk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zytxfrxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhbbohbh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2cqgrreeh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xxuxxxju.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcxvtsvj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2eayokyrj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2safixiti.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ppqvcztx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2aexgllqy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2theopsjf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lekqbpch.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hrzgxpht.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ptmafujy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lohztyne.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2trsqcrnk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgdnevyj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wjziumqt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ylwzwylc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vnxdayxy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuvovcyr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nvxcesbt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tccgllzi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wpgbfvcs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2esbwsayo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2difyvvmd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hbywuoft.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lulbezde.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2luifmnie.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vwyomuzn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vowuwiku.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fcgtklkk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kvjsbgdp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onulkzju.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpzpfjaf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmkbdqyf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2skmlgwkq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2blgyvgrt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rnahkojx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kpzcijkg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bmabmogy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pduqzvuf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtfuywuy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnyroetp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwwihzfj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mapfmryj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrijkcgj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gywxrdrv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jryzztpq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nplnpuzn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cinsdbfi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxnuvgfh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zpkyuihb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eaimedfe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pwlhsofl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zkyntndr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2eikkfefn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2hdwsgdeo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2mvptkbcl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yutaqarw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nvfeosuj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ukdunbwh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jqyoiask.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zrrobsuk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ifldujct.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2iotowuhd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2arfuuljw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ogxqwblx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzatitsj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ruolhkng.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xkxpaevk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgwwbhda.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2pjhwkckm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xetcccnv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hqlvbfvn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ssqherdr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2roonndwe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2qupstzrc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hzhxiyma.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2chkwcjhq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdawdvka.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dqiuwvxt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2krajkuec.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymazkjil.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ezsrdmzu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rybqjnsm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2datbtdcg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pojrygub.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jzzuosie.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xblalhsf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2eoqtxcej.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jvaehpzh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nzmfrakw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2khlgqfty.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2popghwoe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnupcifd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zncbhhxp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyxgwtyz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2omjutenk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bjvfwlxa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zkfxhoxj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2euqjxhzm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mdiwffqa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gyhvszfh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hpybedrd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mjuzdxei.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gzpdyycy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unaudiuz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lvrdmnsa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ezflckou.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xwxxgtzr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2stntewrl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nwpdtfmm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2calghwlf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nnbohyse.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vgmxcynr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dklmydyg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yepjlrfb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2romtyywa.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2aivvoria.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pcnpxfzx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pmebnpwj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mqifajhq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tkppgpwb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lpckmgnr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2kltrielr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ycszmirb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vjpapjdb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rnhzudgh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2rplcdkdm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvlozsdu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vblrdmgf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2agidtlee.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tiqbahxj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2mycrwkfa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bsvkqohx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2acvhscao.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ngqouqcf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bwxgcqnb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2pnywzlmn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ownucybd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kbqsjuml.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2alismxjf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nrrplmlr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2onarpjcv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2dvnndcuu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2sjgxjehc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqxykhcz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hndolnfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzvffiwy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ggstvmla.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2chfcnisr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtfeycbx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2recvkdgf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cvqnbffh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxorcbql.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2inyjdvuu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2djchewua.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jmhhpfar.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fjolhnyo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ykmwelgy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2laxqxqvk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2itjfvttb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2woksocbv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrezjmsp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ozztrxvi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fzhbjlbe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ulfotfbx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lxtxqkjo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2iuzdbadd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2awjjmewh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2plfjeygr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2skwglgtl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pslnbjfz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxqpbie.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2kxegmgby.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2navloeoi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2twklsfzn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2lxlrkbah.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yjrtnqyh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lnytwhwa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2whomukgi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tehasify.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fgrjqlrc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxuxxhtb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xsiwvivk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2muzakrak.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2srlymbya.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cqiufpyh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmylvtgm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mejyffop.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2umikmnrv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xqzlsfdx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2vzwfsobb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2agurujyw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bddczest.html


<!-- 参考信息 -->