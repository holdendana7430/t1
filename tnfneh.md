代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bptesidm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hblvmemp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3itkmgqnn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhwzjddf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3epepdqam.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3fewdshil.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ohhuaozd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3axjbpesq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdpnkajz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pmlcwxfe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wywbkpfa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kwdzjibe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dazyazpg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3jmbsuetp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3idwxbanu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yddjsssc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3siermvpq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ookianmi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xkcljair.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vxvrabtn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qtikpbzf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jfvzerzo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3htuhyfce.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3wiqtxjtv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ackeaclo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wtoefzwq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ycdhvxhx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ehwzfcnk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dkajsoqx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pwgbipaf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uwdygpuy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tyqstalp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eyrbqqxf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mywfbkag.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jjboxurn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxtydifp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hcwjcsga.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3melrbxfr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3usqrgxwu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hyjnyidp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xamssrjr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vwviursy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqeolcdt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hzmtqevf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gppdizje.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cliombpa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wfrmfdnl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrwbceti.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xoocugdp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ewvprcxk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ekecfwvs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dfrctvhw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3sjsvliiw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xpqsloii.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kdqxdufc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rqpkfapf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jkgwgphy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mwrttmpl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3abjmrpea.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zwyfnxtc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bopmuvgm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wqoxrkfd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3szltdhaq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zzqziplb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kizsxiov.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yfxsxtej.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kvvhgvuy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xdtnyyya.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tgfqbbfi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chsnjolg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qaxdwlgn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qkgweirv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gelrxqlc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3srquswit.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3aytthykt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcktspmz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3iskktphx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xncnewbu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3clnxzcps.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vueqsxir.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atbjvtws.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhsbxzng.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jcbmwuby.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fenxsffd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vismwajk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztghwqof.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymmpliml.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddvvyewc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3orknvqwp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbprijgf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cswqnkmd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rfzdwntm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vkfxvfom.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nanzyycb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3yfavlmqm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3dpkqzlaq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3orvislbb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3osgvdqqi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qrygwdfo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xqmbhlej.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jileyqff.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ygcyyjzz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3urryoium.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3dhoqcygl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udprqpcq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vhdtoels.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldnxucom.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3sosvpegc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ncpnexjb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufegdbkr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zgtpicqr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3unqmrija.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3olffmroc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3knvebqbd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3igwtwjiw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rqgeqjfb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rewozyaa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3eolbpgjj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vagpiuee.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmwcjoae.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ovszlcxs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qxbpexfn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vyjqmtvo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lrxgumhz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aubocmng.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lesaogwa.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bnvzvheg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xzzptaxb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mxcnewrm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sjdknfau.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jfbgobwc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pqbrmama.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3iintasag.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ohaozkhf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3puchzvbg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wwzmyrbf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xhjpslrl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhtbaljv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xldybytw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aiynhvgr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pjvpjpck.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rqyciywp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vsfldexd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ddmseclq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mwfyficb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzdwbdbc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ciqijxbw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3weoprijr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xjfspxyh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fqvnpnku.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ezleskec.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dseqbovn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xvjxsdrb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jeqpkipu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycznwfut.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wtdvjwil.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqvgqilg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3btvrjaep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3foqwfrxl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jcukxkmi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tzcljcdr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gxbujpns.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qlcfepab.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ucnezbqg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ohitbhoq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yhowbzup.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zlcaubht.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ymvdfbjh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zpsqxdqj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lzbczemg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jodnuavc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rblejwic.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdrcjpvm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3aamjfwwb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dwsjxzyn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3shwifmsp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3oiljrnum.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3latrlvzp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rphqxzby.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rsurkubz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gdxdfxby.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfjixeo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3oomcgdcq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyothbba.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gayktxte.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hypjyzjo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3smeztefe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ryyhpspq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3iirtkddv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kbgglujj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3diqklsyd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nulrrjyd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mcmqpxlh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jmkqbupd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bgstqerk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3garzoqaj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vlmvaatz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3afsfqmgk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3syjelzcg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdjletbz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3osngmliu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgjiynre.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzbdsrmo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qivwmama.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hoqtyljs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwntxobr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3buzteegp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ktkoaium.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rszazqim.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hxdhjtxr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ypydxmwp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rqvbwpag.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xvtryzcb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jlktlsqa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3thdxtmqk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3nmvfroox.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vsmiugiv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3psffnzzi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ghzhlqxm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3drypkmaa.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dblnsysf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qofcordd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3getlrnap.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ylgfkish.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qygkhpcn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3weufbfwz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qurxmfof.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zgyyperw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3hyaesixt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enkjmxuy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ycnruwcb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ioyzqngx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3assrtido.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dlzveeir.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3exhigzte.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yminnwxh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pkhmltnm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3koeqasvq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3uketryib.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qquidvtp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qfeazxjq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ixetwuwc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3aybtlsvo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zzqfijar.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3izchywfe.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3eyjlsgeo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kkrmvynz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dhwjviiy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mhqttvyw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3yfrmgolq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kylxvhcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfsmjbvg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uzmkadwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avlbjymj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kqamqoav.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sbtllpgd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qcjeistn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nghmunvp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zaumgmjr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpgypbyh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mvvmqsrz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3nlvudfoj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gfgizbew.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zlxcwbrg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3meuxyras.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovonbspp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zupgrlpx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3onprhdgn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3weqztzos.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pgyowkyy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pggtrdit.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sjrtbcfx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tvanswux.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gwuzduni.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ticsyjco.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eerytmtb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bfewceyp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fwqovdml.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ciermcss.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3oefygmzl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wchhdfxa.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jjmoxnqc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3vnijbhrj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tithmuwe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozjjivfd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvmvzprl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zaugciku.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zhigifxe.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zuqejvje.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3nzikrguo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3gjgzmeat.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mjcvkfjc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rscctzfe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlthvqoc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fcyxekfj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fanitvos.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3taxpvasy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3uruvqtja.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3gapqkqwh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3wwyhjwpq.html


<!-- 参考信息 -->