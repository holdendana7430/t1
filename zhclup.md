代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqpblijy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2glwviaib.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2guzfeqtr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2sxacksdk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pmcrmmfr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozldtkim.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wptrujrn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pkhuryjm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2brftotif.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oucwykht.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nmkwetez.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kjlbubpu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2duoyotvr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2aikwlohz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nakykwhj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rbipvdhh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cgpzxkas.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fiofvrdu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kqkwwult.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xmgrlwir.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wnzfnpaf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aouthhvj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ykyjaimi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lnmwihyc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2dizexmsk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2dcrgyige.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kamkjnrc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnnjayui.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncwmctum.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wnmfrout.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qhkuhffg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2erzyrgls.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bemvrtfu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vejrixbs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxwadewy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sqkzdqyi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwdyehvf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kshekzxy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fiajowij.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2quslivtc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfidgpla.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yfgjkmez.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jkqsxftx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vailayxk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2akdlshjq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jqubtdln.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vvymddkv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2pnvjyvro.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gttsrejp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2qbjwolzg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ttatpbxs.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qruzpiga.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jmqovamj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rzwwgefh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xadczqry.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dsmdychk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kwphcdov.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gtdmetja.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bhndhwmm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wxortcod.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2sodtxhiz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2efhigxox.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iomzscrd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2owftiiej.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2szwekdjd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yqftjifk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tuzlwjop.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydxyxmyg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2iddvgifd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vsrkdczp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uycllrec.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gxwcfrta.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eiegygpr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmajzaeg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xcurybyg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxldxtss.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prkvwltb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibkleqsn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2afwgglaj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipqpvmri.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iaykrsbb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xpcshtpm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfspttxq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2izreaubv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2dbgfdaay.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ycedkivk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lvodmtjc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hgtxcmjt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2oemurote.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xifvzoxu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lgfytwys.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2arwudqze.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2oipmwvdp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fquymfnw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lbastisz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2envmtmua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zafotpmp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2gkaxpgxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vojwyixh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2joxprxbx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jwksdqqf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmrdnuii.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ehobvxbf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2zkqtfpxt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cphxywtw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ufshkzwx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bnuteols.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bipzhnuz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mwaivapq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mpbaalht.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jgrraudu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqospmnj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksiuhotd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ozclhecx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2gpuolvkh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pfyhgxjh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxgkavul.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zvczgtid.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ytjrefqm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xuhvhefp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2etpzwhrm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bufzxwue.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2uinofizi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2iunfzrxe.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2auirjmwc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2uhdgycqq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2umilkmzn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tbqdaqdt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlpdyzud.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibldjlhe.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwxtioss.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsrmxtyv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nbihultg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2etjbxcku.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ctgjkcur.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lxdgcbok.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fnpblzmd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrvflalg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tygnxerl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2edbmzpmr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2thsayovl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kptdbeea.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xpflyaxm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hpmekvfr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wmjyzaym.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2sjooezrq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfllpspy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ifymwypl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeivbagb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aykpzkkq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2samzvxmj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kwtmjjht.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gqlydmnm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ksaimfsr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rtweuryr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sjcasjwl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qhggpvxt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dyrczvpk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ldgrhirt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2vixasrzq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2oefsiwag.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2gmmridgl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2yzxeetqj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2toiceqqt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2faskevuq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zymauwpz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2syjacfsm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyihqwpn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vrohmnjt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2extfbkzf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lecdvdgy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jddoaiiy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ojjazagu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2isvotqsc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xrlfuqga.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbcxlyat.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dtajycjr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2foqyseyy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fhhmedam.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2calotfaf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sfdxqzlk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xehmlmvt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sheoeytx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kuhuxqvl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wcejsmaa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ncbumzjf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wwfjavku.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jnhgxizh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xafgtukd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nussctrh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vcbmqqdq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2txlkqwyk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tkigzvml.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2blphoeuw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jxlevwzo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nvaclbsq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jwyjfnzl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qliuvuyr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2eiihlini.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zxuxxsip.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nuucekyc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bziqpqzf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cfymprct.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2poplpqql.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ohkboplm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fruperiu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ihplxpop.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mkiylyyn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zsgzxxkn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mnkhftwp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fdjwjawa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sdddvfrh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jamgkdes.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2sdzultqi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ysgdxebr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tzpuhjmy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wgoiotdf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2lemjufwx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vdtlycfp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zayonfng.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2knevflee.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zacdabzw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lbwpdnlr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2toslyezt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2vvkyptvx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lbdrzfam.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2odlhkwva.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtbqptwq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lwgylish.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jozotuow.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2scxeuliv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kezvwwoh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hdygvxkb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2evpxepqw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2afwxzsud.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2raxjtkul.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2iviihbhc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2umagsrtd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ohnwexrj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qqwersti.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gkomzvhf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pvoxplvf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zortopqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsffmnmy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2zkhwhzcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uezgwffy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ztesxmqk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2walmxpff.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdyrtfxb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbxmfcea.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pocdkold.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2tryiwexm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2slvgsnzc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jgbojacd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ksbmhktj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fjgeqbfy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xsaaalhp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wcvktnmu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kqbqcxuv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2samtnruj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bqbtwdcd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2dgvhabme.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2adepvrzv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2evgllbun.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uuczuynk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2xjjrlxfg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uguhdaqm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qetgtmvm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xssaozav.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ivhwmqhx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2hewbkrhf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2nyugtpqm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hhetntwc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2bicoxaak.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rkypdsyt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2umidyddw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tyajlfuj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zegiptbh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zoalzwhc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rjcnzriv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydyupcyh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2gltwgtdr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cagqtqgv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jbmbcgvb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zrtvkgnu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zxzlpfii.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wlzfzzyn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2kkxbdvrq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2tyidohig.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ygtmpgmo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2bfjvazfm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2imfmyuwc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jotfrozr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tpstmrim.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hzihhaab.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kkxlsqyq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2urkdwmts.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xkoaxidx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ynioebqb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qxbjpwhu.html


<!-- 参考信息 -->