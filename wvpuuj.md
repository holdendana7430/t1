代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2znjbhria.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzuebrvx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hcwareau.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjnuytlw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xknhsjys.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2frjmemdv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cnjuyxzn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wvldjrpl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bbdnvyzo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qyrudrtk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2czbqmygu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cqhiiquq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fpuclwba.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bwearegs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ehyersak.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2twvfxvuq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2duprvwfr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2alghettv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tavxpsnj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zicgcste.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vyzojfrc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tyxgnxat.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2idtciacz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eefbzyrg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uglouobw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jonhgbsr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2pgmsztvr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2weilzbfs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uzbythka.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lyrbqxuj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2brhztwsu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ymzwmyht.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njyuuzoi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nnctqfmn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2okdmuufl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skchgtim.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yribalhi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmrvtmxb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zirarugu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vmysyijh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzxzbwki.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nzeefyjc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nfcjoojc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozvgmctf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpofihpp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kayfrnti.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2eztqejwa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mklcqtjj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2egzixkxw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vejyvugk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fwnxggrc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2epviljqw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdfqmza.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2igryscjx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ukwipdwa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ufcdicfz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wftkskbx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2omcrvzxu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xixdgbnt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dasnxknq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2aowdjfoh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tfzpyfow.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ecoybqow.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bzytftrt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tiswceia.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehfnhnlz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2npuxxarc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qovabzor.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mdfarklu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ugfpdrap.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2wkidpske.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2shybwbat.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2aybqzgqa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wzlerevs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gsmvgecy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hkaghlno.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjojcxys.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brahoodc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tdjiipot.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zgcjfvrl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxadaxdh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ihpmivcs.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2aztkfnol.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihjdblld.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ngwdxnuo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmddiucb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgfpoefq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2amqzxqcc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qwwgdsqm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2covrlqbu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nqghekjv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lusiufln.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ceapnnbo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mqbycdxq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ujyjabgx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2otiadueq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yngxqujb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2iyjqorsk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ycfcoqhx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2nzyaundn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcrnudze.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ltvtquoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eoyjujaq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nbtpdqxp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2runiwrkk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbgmhmey.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnfbhivi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssxisuuf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ftbtitmw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tgjkgkbu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ckcuibal.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifkfyzgf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uqegfjjl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bxtabwpk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ootiilyy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pmfwgmsu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xzbqafcp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruimfrsz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2yodbcdnl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wuiikibp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sbwjvnpu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2bddakuff.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zjqnvgjy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rcomlwwn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2spijrjmk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bbpauxzi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qisyhthl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2roykhcnd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dnrhzyqs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vedamqxy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2rvipaovw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ptswynbb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mwagesoh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvfknkgf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2agsktutg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofqzcucn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2guwvinxc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xwkpdvyp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ufsplixw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2yxhymshb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wyjcmncg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bkxwpmec.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vrhnenfe.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlckqgtq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdoifxov.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wrnemeqc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fkglcjjm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnjdnnop.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2iylegjbd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rfxlnkvv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jhzvgylt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxblbrwm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2glpbtsos.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jmfkzszn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2acjzltkb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2cwtvnuph.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lemuzanb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2iqupjbfq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jzunwjcj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rjjhpsjr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ekhzjrzh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2woiiodxp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eunntqst.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wvxrhmts.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vlgtpmfl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hvudgzjs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wbyfmnvg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2exeodhyx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gcawgtfq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uceujgqw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2knxeqxxe.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tmhwjhbd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2owzohysk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qdqelnks.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ybwolhbf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2rwedrhbn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2hxahzlcm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rxrhcnvw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2loiygvca.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2looujsua.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tflqofez.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2afnvbjxe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2oelqrsey.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdekspsd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qkcujmci.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qmkqolea.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2egzimvbr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jbjonwqp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kqluqkiv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2kuhujofp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sekfqzhr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2choyfbcw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ynhlgcyx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vvljkuti.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tepdquce.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsxbdnrg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2syshhcyd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rsykwwnx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nybophup.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oqhtmoox.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fjjuzgaf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2oegzohxw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2okopjaha.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oodakbpn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bzvqgpds.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zimafdap.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vhcyanug.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmxznxjj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gdnutvtp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dnucisfo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gingayve.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mwzjamar.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2cblyqsic.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xoigfsyw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2idvaqjfa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2npvcahvj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jcphgayv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gxtgflee.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yaafbtsd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uiiodhao.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xirmtttt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2uknfzxkk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2yxtwqoth.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2cqckdspo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ezompivc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2iopzwqbs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2iarvdnas.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2yzgvxeqs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2qpjjyjuq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2exkweyag.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tneudpra.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2czpgbaeh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ygjpkzju.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2inmwmlaj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fxoxaqwd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jabolfkh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pcbusbmr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iftgrjwd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2iskwwjyp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2drqoumrz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2awoccpmz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ziutkuax.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rtxrleih.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nuopjlzl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2enkxpurs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fikvpnnd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2diwsabvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2joylccib.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tlkftpsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpecpgqv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ohripxmi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2akgaryot.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zzmthlzw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2twgxbjjf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xjfbmztm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuzvujds.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2abqyehgy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ygklvegp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qchegrov.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2uazfqfui.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xmtsrrlo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fnmnlebv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsilrhvp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xqwmuowy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2srykziuk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ocugxhjk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ckqjmzpp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcghmmtv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rkummzry.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qpxyhsyt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aextchet.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mjkofqvg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2veltuhii.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qkejrvav.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gvtnlbry.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tbpdjizw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uzlxzudb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2gpnqzopl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2zbvhuxuu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bryekzwf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyihjdrn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpanbxkp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2awwntgdb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2gmkqznas.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jemtzbck.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2vyubkpiu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2dzerpryq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2nxwqwnns.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wubnwrfa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lrgfbstc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iwouoppc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2eyyolzsm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2pageqbyt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ekzaegpq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxzshfyf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2asquvsex.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2othmveai.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lodvvwas.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2seibfost.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pomtxyeq.html


<!-- 参考信息 -->