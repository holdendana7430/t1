代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cqjcxicf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2twrjgcbv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jplneahv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdexrrlk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2igzbzinp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2smdhubtj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qhwbalqm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ujxbbwnd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlppmidp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ldhhaics.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ftfpgfnd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xqbzhidn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bicflffh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hqqohjux.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sjanyiai.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mqogxtro.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wwtllpgb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kyfeugat.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yczmpgnk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ipdfcozm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2uigxnshj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ifoqdlto.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dzhjlaos.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2iohibfid.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2epvyktie.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qjowwfql.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pfnutapa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dzasddmb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wgnnstjb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cqipduim.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dhjeggss.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vvodubak.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zlilqcuo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2glmfegqb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ulpktnzb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yztyshqm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgcrqicm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jdgevspb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2usptoxwb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exakhhfj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydifmrsq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2txmknicb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fquogtpb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ydonwpxr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bpupkeyx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2grsuvtpa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2knadpvky.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kowqxcsm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snbcywds.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cyiukcmh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zsatmevs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pmzfwqoy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2phgmtrpx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yhqugbor.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rebfkfbm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vwqrdycd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bmlrmeqa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vioywpju.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ezenrbiq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2eckfnjsw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2avmoaker.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqeugjsi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gsppxmbv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cylwkvya.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hrrdgsqb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ujnaglmy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hrhnarzp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xnejpmcm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lolsxjrb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvbhggvs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ghhnhmkc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2oowvckwq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bahkjoyu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2byubpkio.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xuknwjtf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gyvkejhk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rqviiljw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qaaywhkh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hngahnvi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2onucgfsc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2naylvvrp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2klmowndk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ymhnyyoj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2voiatipo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewccwatv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwwebxba.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jecfinst.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jspuqghg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fnilascv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlgeplrz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pgvinajy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvyqibz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nmwyuqcf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kusnjkby.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xmwjbxwr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2avbtzmvo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2yapiwvkv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2acovzgda.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2iustokpp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uxexdheh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xfntqufa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2yzjjixqs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rfdypfye.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2doarvasr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjbvhheg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ullzlssv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnlvdnqs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uhkncxen.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2irccrqwh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbjeqnih.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ytthwycm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbrmtblj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xniywzfr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tejxuqun.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2yslleykr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zwotveuh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2igzfmqhj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2iihsuzal.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2trpwrcql.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ahqnfdzc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mntfevoz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2btvbzgvp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2sxvowriv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kjjxtqaw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2whhyqxxt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zhbqbidh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cnpldfuk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2apuygkxb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2grvgupkr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zakjfcuu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ajnzdsbp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dqaaxolg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2niyafjtz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ligshtbx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2popuwgjj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pxboehsh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxkqavyv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnlkihla.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtdnjwew.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tqffrryo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ifycmkte.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uvhurpsp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vhhwmaom.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tsqgterv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rjecvnja.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvaaqcoo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nutugbcm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mammwezd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gciopfrw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2svqmopkh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2oofwleku.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hhokqrlk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mluocwwu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2txhlzhox.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ulayermb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qufvjesp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhuvkyrq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dumondzt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rgfwnqll.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rgpuqylo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mkwoopcu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2utxbenlg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cvlgkioy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2otnidzja.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ajhhnxxw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rsgorxrh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cncxlcyj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nkkghmed.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mzntcena.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bbopoatv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2svplohfw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2nvenstbm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pteqxgdw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2murfhkhb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhlfbeoj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2guiykvlz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ybgguuzy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwhhdlkv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rrcjclqu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mqlgiisz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2gykqlxyh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhybmeoe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2icrsbels.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2upoxftzx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ddnejrin.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2aaemsklz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2phvlqlep.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytwskfzm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wfwymviv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zrkqglqs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2soofvwey.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ibthsgbw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hgnbrjzi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2xaqwhote.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jblomnng.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2isiytkat.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fxwlksfk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ysbobxds.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mrsuviub.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vpupwphi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwerakfs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2engonuek.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gjtbxkmj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2djyzlstr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nhmctwbx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yumlqzbm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2amcpmcem.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hlyqanzo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sjntoqpk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cjjvucqa.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mezjqvlp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uvmgumav.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sixroqow.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2umutmyos.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2aidkhotc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ukhywlgo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2efvixbhd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yszzutob.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rnpcsiss.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rwkmvaab.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2whryjnne.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ydvdfnho.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gakwnkrs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2cqjlmdir.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2lajgjwje.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2yfpnnbkj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2exnsvato.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2havvddbd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jtughbhd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ooujaodc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2rlhnefab.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fpuvbdhj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jafqyczo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2nvgrcfei.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzellmkn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yinccenf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wfnthcey.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2niepcipt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2npqzvjmq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hmgklcds.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2tgmsutec.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ujeavswt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ddxhegsz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2isuryunp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pxgzdyzp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqimcxwx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zjjlponl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lzktrdwd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hpkltswg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zmflpmmn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lazuzyyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqhjlojj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zhouewza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvpwiexp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wjlkhaay.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mcdfnqbg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jrloaxwn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hgtzhekv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gtvzbykk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2qmwxqkcr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2nnwnjdel.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2clcykitd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2avafiogh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2dysslcws.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2pbuiprxt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxljbhl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iocrukhz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbiuttli.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qoeqyjwf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2fylxavio.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2syjqwdoo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbpaejgv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fzsdpbux.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2uunhxmfx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jnejwgac.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2annsoxiy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vpipafhn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xpucrrew.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjujqbk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2uviupcna.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xxdekqpl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hmuhuztf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rstnplmg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxezldxk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fpyxskpc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qxkwlatm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vebyjizx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vvbmqckd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ayzzceuj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2pqhrjxpr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mmyibwgl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2mvzqjrxj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2djcrimhd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yatwcgte.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ebhwdlpv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2phsojnlu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2szodrjcz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2icyheifu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2yhvevjjr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2sktvkgah.html


<!-- 参考信息 -->