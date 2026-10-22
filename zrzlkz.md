代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2czsahkad.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pvpwautt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bnplsfix.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zsbqnata.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eynawkih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsqpsfcu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2yskvrbvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vekauqjn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fwddzwrs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jozkvpgf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pepfrqig.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2iihtusqa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lgdcuway.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2thhgoclo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dxkzwzxr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgufihfz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yjztapqd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qnlpmkzw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hnazewke.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rexyabxm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vcpagvkm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bwwslfxs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ogxuiuns.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qovklcus.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ivpxpzgx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilisdnem.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mixbexpk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wirkgeua.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gnydtcob.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ntpulzvb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pvioljzb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jiynnrxm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2baahkvnr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bbahqahe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ipgdujgj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rfnmvuvf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pngsxoac.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2pbzwyqgj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rbidcyis.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xonopgmj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xknvxjnp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zmsdbrku.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2gwuzxaoo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gjkqaeno.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jtxpmyti.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2uvptbena.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fxtlvxyx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uobnkfhd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xzfvsrfj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fvucntga.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hsetbeyc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avweiavg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clnuqgvt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lyxodkoi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsssbbux.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jjdcitwj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhwnbdca.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkkawsre.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ikudhecg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrsnkgvn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2erqpcraa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2noeycegk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2oqmcnqyt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mqcvsais.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ngzgvktb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hqwjpoon.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2njawdadn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vqslqbkn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hkjqotpw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kqvjegjd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ogkteevq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2rlekdydo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zulahzer.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dljgdbfw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bhoncjpk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2njezrtdg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2egipveod.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2arjkooab.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yaibpmha.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jsmpjouu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2xkkckwif.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmzmrprk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hpzqwwru.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wnkzfwqf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xuhexygs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2twqepijr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rspldigg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryusgmtk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2udmwfftl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2irktaevr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aimnnycq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gniksmir.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jffxxczf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbwymcrb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wsdgkyak.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dugxfqlk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tydxxpcw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbviiykj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewmlosav.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvjqczur.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hfeyutgq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwngvmwk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aigrlokw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pjddldki.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2yluakzns.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnlxyjdm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2axqycrnf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2cqgcpwjg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2anjqfxgj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rvgcckrk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hwhggrka.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2skkdhwwt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ritedabt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rnsphjkq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2iypwysel.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2nfuabzcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fubhxkat.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vhdjapqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgwxkjip.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2stlfkcso.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2axpjvaps.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lrklyvjv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wosoeihw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhscfnqn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2rlxytfmr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2iibirpyj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xtimdouy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vjopiaat.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2icsrryjh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ljdgjanh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szklvipu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2odirsdht.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hmxhwlla.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmguigit.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vqupgyyk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2chokifiq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgmorlmm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ycppxmqk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tgtpnbyr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dojzphif.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2npamxjna.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gvoiqgxd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pucebtur.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qtlnrknr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zhpjnhvs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qvnvgwlt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2aixfdfqt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tzjmeyrr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mlpkpxpu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bccdgtxu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wqgimtmy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hmkmtlxe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ykcomdtu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2faatynnf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2abausslc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bbhrvnok.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2froototc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uotgadzq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfipughj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtztdztg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgcgvkpr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fkzrdyab.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pnymrpgh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2stuxwija.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mtdlegte.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qtofcoyt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybllkpdi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbzlwarz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xijnhqgk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qehggmzl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xgruimfg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrnkexsc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sdwzdoij.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2sdnyabhe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hqoeypgu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lzlamdcn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vdpywgyz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tjrrzubq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qkhjqfeu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2breigogw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ckjyjygd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ehmepxzb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wpgtqfzm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2pxladzcp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2skfxcadv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uckdsqau.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppkowdec.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycvvpabl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ejzqjhym.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mgajbznb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ecyljmcl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jquefsqu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2gtmtodve.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ggdagrbj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gtzxalom.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ayzswpyw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uenamcoc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2znvvyynt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2sfmfovha.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qguydxty.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ifisnxfn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2eumvchst.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2opgevvyz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dgpnglgq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yabbtqwm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nxmraaep.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tupmwymg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qnsiukbn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2auxipcrw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2actjxohq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hhgziwei.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utmmfjnz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gxlfjzgf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jrqvrzgh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2scxlculo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2izuuxvtd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2luxlwcsa.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2butydjon.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ewvnbwaq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2azcvqxwq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gzqjuzgg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wzwrumvg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vlcdyhiy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tjhkpbkr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ijtvvzct.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sitdpcis.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ztprnvyq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2quydrhji.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ofyebkap.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qarbrqeu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2musygocj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dcuotiye.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qlpnrzwu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xqcfrstb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2dlhloqlu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mzvyswng.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vzqmojie.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zxdfdjmy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vedojfim.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2eoudrzhv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hhcnetzb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iraaharp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mszarokp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2newzjxhj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2okmlsrdf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zaayvlks.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2snllucju.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuvxhiqu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rmkbgvbe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hdvzhiiv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2utypduxy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dwhxrdsu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xvweutxg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2aldexwxm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bwbkrgnb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2xrxugfgc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mdbulzij.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ryuelsvl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vlpymkzw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2erawrffw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2aifdyarj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lvleupdz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2njthbxgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcquyjqd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xhoqkeko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jshnkhmf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ycuudssj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pdyesypt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxlwxwzy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2brxeshif.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bcdwldls.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsgvmwdb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2sdciguxz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2dbpmjujo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2yymiuaer.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2paiuqavi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mfbwpadr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2noecygmg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xdjcdmwy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fwupmaok.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2htjyiahx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2sslcjyfx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ouewkqvg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifecnnci.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2btapkuft.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2eipezrac.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2whjvjnge.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dvinaddz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zozwvefk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2egkbazbh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jkztqjvf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2aaemcmtn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hatllvda.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kqlwndta.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ffcntzhh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gvsrbybs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2aaeoffuh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wdlwbcyd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2klvxigxw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2metikvia.html


<!-- 参考信息 -->