代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2icnohhkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yynhelwh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ptmsoyai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjowpudw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2utujopzy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2smtsivgn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2psswwhju.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jpdkarlr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2toodbwkq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ylansmul.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2eqnazcyu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ynqqgsuq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vacgmbtc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tjzagity.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2toivzgmy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bihtplbz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxiyyilu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbjdvhia.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xadfrzic.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hoezubol.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mihouekj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikrlaohz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jvmugjto.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qyayepmt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yhneizoe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ygoglygi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ymughqvt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kwxgipto.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zvoyvaro.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2eoawpspp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jqknctyd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2cecxvrln.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mtxrwhrj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jvjmswrm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2oybhlqss.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2astantvb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2mepnwwmt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lhwzkytc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2oyrotafx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kpdpzocn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2acuzywxl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2uzcktsgu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xrckeiza.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmxhncbx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2knsjwjls.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ovyjxjzf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ddqcxady.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilaqacrb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2buwrirsz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hvouaxcm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnectypl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yuwrxpzw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgfdyths.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwondyyh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ylbhvluw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhjgeccj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfklijda.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qckzwhkt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2smprubyh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zqbggaak.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wrpinuqz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cfaaeeni.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2onatgkso.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bhyrkqbu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2fvstjoad.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vsbxdqso.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ctjqdxlg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2yvjnssqq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jkuygxhu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcstmwfy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tovypvjv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mmzwzxmw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2szlunyen.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tcywcgjv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rfgpkoiv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2treokmxp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wvgxauwd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cxljpnml.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hplqsouk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uchibkzd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yottuzvd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mrcumdra.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tauyqvaw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hsmnzqny.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2cegwykdu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2dxoxelph.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjlcuogb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wchspjdf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzcondij.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwzvhtnc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rnofumzu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmvwgeqz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ousmqqmt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvbqamry.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ygyahvcl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2whwcxulg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2viyowkuh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hcruogfn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bufhisno.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hwrkasla.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fgakbrnh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2trwtfuxz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2dnfiqkud.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2scotzqdq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2diuxsvrf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gmlioyzx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ganxcpsy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dfcddtdx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vuwfczdh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fzkocdmo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2thysgott.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2einaspyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuvdklub.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ulhyddgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apdxkpoi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fbvmtlyw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2puyledxd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvesjeiw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2siskqsqj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vdjunqiz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxfggtds.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kycdidrn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2eflnozzw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oeiubcmg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tstdrjkx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xjcbajmy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wwqgmzbc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ssgumnwm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ootceouh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2akgxstbf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2pqormhbk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bokekxnm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tlttrdmj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fpdhgcuj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jdkclfjr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oybmtloq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ioyvnbhd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2onpjnknq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jrdusdef.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2kjowepir.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2etdldppl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ozhnaapw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jmtruhig.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mfgehkyt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxylbqqf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqauuaso.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpzzhypt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2whnrlewt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oyxarcoo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fjqqyqph.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2workdsqq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2cwlkhzhl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2scrrieec.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iixlyera.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gbnnqujq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ggqcexey.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycacrkln.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2gcixnejg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ydzjnqce.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkdixeaq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zlwgobva.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2torvbufk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbohhslm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2djdtoczs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqycigpi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sqtpfmen.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2litwckik.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2bhdmfcmn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mmkyixsj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2hwhdanrn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2eknxojhl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zsrxuzeg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rskwosug.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tygiishs.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rmsmwiel.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2geuitadd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fdyecjhp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2vllgghat.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rkoabrdv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2axaqvvwl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jubkomiy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2iviwznuc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlghjolj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hppelwpa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vjwjxers.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vbbfflhr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjlyffyi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cwbhhpyr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ebmqgvin.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjwybxjs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2htgneqqp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ctfbdhrt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkepyrfq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mwhbsbem.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ryrdfjjv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghlccdvb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2bkouvjca.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2cpkfhgws.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jturxfyi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ynnegzqx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qmiuiciq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2uprsyoiz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2chzhywqv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ikddvaac.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qatosorm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dfkcsgui.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mkrsygag.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zecrjebm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2twgqvrzq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsiatbgh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cxanbdal.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ogwawdqo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jfzotvmt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbyiigqh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kbthjrzu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yppojrmz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wrjhlxfg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lfzissfz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iowxpuyw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrbdvvgc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uddvilnd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cgoxckvb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nyhzstxd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gybwslse.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rvlfgseu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2towuflrp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nmgifkoh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tiwtclap.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2htmptewm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ggtuskys.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2unldbvyv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tkrqjnzh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fszfcnkd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wmreezrq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nytfarte.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2siassarl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vzozvkeh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rodxtvxo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gpwpvkaz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2owzdgiop.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xlwugnpe.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ozfmavcd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2umevlbyu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogloofti.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2zdkznbgb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jkuphzqr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2iqtrhfka.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2htufxepz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2grocjyzm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kulyqrvb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xptqqcrn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kwapbyvz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rbmtlehg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rrwjjgrr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xvzwakiv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2omsudhrt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2imrpaohz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fxvyivct.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uuoixghl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djqypzkq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2flbpbqbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oeqlgjsz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ybjekjun.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uirnjohr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2thfyjrkw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyxbnqkn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ersbqrvl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mokbqpgf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ukbwqjbg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jdrsmmsn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qeuafjow.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2juqvjkec.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wkyfxknj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mcemetzx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ygjsymoj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nqtrtdja.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hptcopgh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wpaugxxn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwzwvszg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2snkwcluj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hnkanopm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vlaesbeu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tmqwviib.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gwmhrfpe.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lvjprqyv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uxapomcc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2wybrontg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2hfjevrbm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qwvackfo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xgbhoqqj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2lpalapnl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnxpuiob.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kflauepj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2inxedter.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwbmkbgd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lkopsphl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jclppmhl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2iqvthbda.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hmzyhtnr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2irsdkeif.html


<!-- 参考信息 -->