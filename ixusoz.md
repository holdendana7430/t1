代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2putdzdfm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmvrrove.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hyuigyvz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yvkdvpcr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2exuwdqss.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aouehkxg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2buldxtly.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tpupneob.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sefifuhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acsgcgkd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2kglmford.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otdhefpf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hptaslmc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nrhixpba.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2epaghlrz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mbmjkdlb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rwxvogvz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bjpajotx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2agqafhsk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krzqlfgj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vmcutlty.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxywpnjp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2hsdbzbsi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2afxiwbzd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2urfbkklt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbwqzxzr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wvhwctse.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2scwkucns.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2scabrfgr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmrxlfqi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pzfugjfj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2npjecnal.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qfsngrkt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hrrygkfp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2szteiuqu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lewydyvc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ykupukuv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2laqogkrt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2flspzxsq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwcjngqh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2irnslzzh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qmbywzyb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xtdgxaee.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pgyxpdtv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kaeveqsu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yxowoavq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fyjdhibp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2adwjzvga.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2cwxtjobr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2kmqfbvhg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pilaxpju.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gktlmuij.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2falkrdgz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sozrmecy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2prgbarhj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqejlbhg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfzpwdrn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2fixrlulg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bsjadqeu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ghvjlkmp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxkiucyq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqiekafo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wcyshkeq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgncdvme.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hudpnobw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fzljcfti.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rmbfdfuk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xsikatzg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cnxvgvid.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gaqnjnmh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qxkqclte.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mcgpoavq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pmvjscik.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ksstsner.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2itifpzwl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gfhbqctr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jqflreog.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2mqohrfnd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xkvqsxde.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qwfkvgur.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gjmagdvp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zlgsqgpt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bgihabgv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jrjqdefe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2czhhbhnk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvamgnuf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vufhldtt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wpshhztc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uwobsaax.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pgycefzl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gxvpqrgk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifrgkuyk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tdrqewbf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2oppwihac.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdxedvfj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2daxsqmbo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xyjepoao.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrvyzxwj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2uzdgjdbr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lnnejbkg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mdcnkqys.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clpwcwpb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcnvqxmx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wsdmdvdv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dcjnpipz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqnjammr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krbveaci.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2clihplrf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rryibkbz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2eynssary.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zehgovsh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2blitqopm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2lyvxuctg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vakofbqx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2sllnjwwx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ouorlvgl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2mfjxrudh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2pvlbelfb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ehrihlow.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2geebstye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erwaguee.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xzjkfndk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdbkektd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ngzrzilq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2clkhpbmn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dfjjgoia.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2drtaetun.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zybfyyqu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2irrvmnkx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dzbjbcpn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kbyqoaxo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hijlxaye.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2aseztnpg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qdsjuzys.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrjrnivi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiftkaea.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2astihpft.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2haakwpcq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2tqntpikz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aoumsrdr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ffubbiil.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qebfrhhc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qoogjrou.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mipuumcn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2knwixhys.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ibsettys.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wycdbpdk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2oddwhqdo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mgnemwli.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hdmdxyww.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2uegtgyft.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ijwdvuos.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgmxqewc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfzkegiu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nkfphohg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xtdaqzrt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mjjzqkwo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zazhbxrl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hinmsnco.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fdodumxc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2buzyrwpt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sxiuzsdg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jkvrpalt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2btajmdvq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2aqhvwqkr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ricovofp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2pmliatle.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekkbadsh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2smlwpynv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zjgghmhl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lznhphfx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwefsoqt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzcjxzvn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2egriwlus.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2shmfbbwy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jgkqedla.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2otamixzc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2svmrexaj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2nsgzombj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2eqmnegtw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wcfyansg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2skroceli.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2elnrmewl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2gveqvyfc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2elcsttxf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2xgwbqawg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2yurdupfo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2inairrwp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ynkbqgxh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dczcsnoo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tgsalvsj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwqfatyt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fgewrfpy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vfgmppry.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lydohikv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qzisrxlb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lzbcqbyq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mchsrqwp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2afrwesgy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2igopycdy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mspxutmu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2acnbpeje.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2duslntih.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qezpreir.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wduakaer.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2itmjnxdj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gqmzqmwz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2cpybqkrq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bbiyzxha.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2acxiqqsb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rizwpzdu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ugyfziua.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gawwekwc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2whanxgls.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hlcsglqi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2widpoure.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tkqvzbzw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mdvftqdw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vnjsgsfw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ktcgsjof.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2nuxxjbtb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqsnyhgv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bkbllxkb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lvryrqyf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpeasgtf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cofiqxba.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lurwmkpp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2arosgftn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2svwcsjli.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ibgwcexb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2neuusnob.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2piyyfvaw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2cgivtuaa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wtbfbnhx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bfaqctah.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dkndgzka.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jnsojmdq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2werekjoo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fojzmujx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2nexdtbge.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xsnbddkk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cwcxvhuk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ciminbnk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ykhgqfdj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ntoizizd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gqcialhd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ngjususc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zqdwhvjc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mruqradb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2smcqnhdy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mspmgtht.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aodzxibk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2deywlxxz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yqsmsqgo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2uwyesllk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2prxydelr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2grykqyoz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jrsqzhkp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2omaifexn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jwfnzyzd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rrtdszps.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dywupala.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lyfcaypr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2njluxxkd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qaapqrdo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ucbczgwi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2czsjppjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2janyumxn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2enudkswj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqqhipez.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mketwzxn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sowatvrn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqgkqigj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdjzbkkp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vouqsewc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwkwhnlq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2jbkldybw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hmtzphbr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qocauzxe.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dvhfhvkb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2rkersusx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tmthbzwg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfctmglc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dbhsbgbk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmwabftf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bftftwum.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zargxmdo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ioizecav.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sbkpsxqa.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2tpqyojat.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nwtbmqva.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qxhzbbxu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mbujkavl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ikiqniph.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2sdbelrya.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ubctrhrf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yfszzfje.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qrdodnwq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rofnmryo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvbaqegt.html


<!-- 参考信息 -->