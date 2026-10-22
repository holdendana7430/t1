代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekbzryuj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2uwyhlciw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ezaequyl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gjfgzaua.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2sddqshlm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xlizptmd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pklyrtfa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rwlmpgpd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vmeehgrm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zrmcyvxv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cclvklxy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gyipubpc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qfajmbox.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lkvdlsgc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hryxnnmw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vmhbypaw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rutuhkxs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xtzthess.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cxauowda.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cjgwdbhu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tjvqmwwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flioyieq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rvecwwoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qelzbbye.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vignhgsa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rzcwcela.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wncvukkg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2zojawaxx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iiyewqwb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nyeagdhu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dzjlvcmu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fszerdul.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cfouiknf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2aumywxxa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vsyariut.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cyhxttgf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pxamjkey.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfpoibdp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2amdycyuy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmtgkbu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2udmxuadj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cnkpzzyn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2isrendrz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vlndyhrk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rpswgccs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yjxxbcuk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zzzmqafe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qnnzwhjw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2taslvpvg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hssbiuem.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2afdpyeas.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2apjsnocs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bgbukcvw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ozagxvwj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tgbzzcav.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fjseildy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wvatglhh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zylgvczc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ycfxelco.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ekfaqvsc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yiigfkau.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lcsfrlwr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aycgporr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbqpushm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyjamcgb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nxckylzr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fdzruwsm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jupcujpk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxscuebl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jxgwdhqk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pedmedqc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nvniiyvl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exnpxjso.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcyqenif.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kmujutcu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vplripqe.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrdgfnfd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pparveyr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gfudpubq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nipirhup.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tdvzgycd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mabepwse.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kdbrmjah.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qckoftuk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2usaouwvz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rqwfncvs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2evveqayd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2oekyaqcp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xsolnuvp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wyyvuywc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bwomafcb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qefxpyfq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oaomrywx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tjktlrji.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2avugoqok.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vymagdoj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lxnnyugn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxxychxw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ufpvixdg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2florzxrz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dxdntnsj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tbpyazgh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ocozfxeu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blpnmbzy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dcwbpirw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rwefhwyo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulsxmifa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yttmhgcd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgtgulzo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwflwauy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ulvlhbba.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zaccnlty.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehmmatam.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxlfalmm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qhvwggij.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2churawzr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pfwpnecv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzfwwbpq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vakryygf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xwnzrefq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2nyfwctsn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljijzeqx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bsuyhgwc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kygwnhkx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rormjzcc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qrpwsfgb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wyhqclvl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jilsesng.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vjxsdzps.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2eaxkyiqw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ctnzmfcx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2acfiftgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuxallpr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hbowkryg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtkunyip.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2arxhntry.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2daghvtfg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2skecepzc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vfmxoukn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2zervfuzg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2paufiusl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lbtxzdes.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2yoxloogr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ulafafme.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2focnssxi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nhnqvqcz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvmanhle.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xdbavqrc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvmtpknv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlftnzu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rtcolypa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nayhwylq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qbjpxkhn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vjdsjpex.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2usqemyol.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gyvngmep.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ierehmtr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2msbdkecc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kengttdi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wfckgvle.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2djjrogcb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bltjmrho.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cqtmoghp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xkucwaxt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jcydblog.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmaibrrx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2prstqhmm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zofqjutl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hiqbugcu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2giqpbvif.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2umuezits.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wyvwcior.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ghwwkrrw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ajtmpobg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwopftpk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hxslujzo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpjtrajw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yrwacvxo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qjbesuuj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkejwlzs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dxicunfz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cqubpftn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eetpyhra.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdfcckxc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2txckwrhu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gnhotdjj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2alfygfvw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rmzpjqed.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ojkxeunh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2byezpkdi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wyrxelcq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2eheubgjh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xtsjaipx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qytuonsn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bbpgkvna.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rtrjtolr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vnsbomrp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mijbxxlm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xkuzjwsy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2uqaeagbn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jqmdyolp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rgxpfljm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rdaibwzp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2bzdvvvhq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wuhhrxyw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wcknbesb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vmdyjcte.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xvfdinxh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2dbshokvy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2arfwlciz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2anqlocix.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuzwfwof.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsayjntm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2odlnjejh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2iwrvxepq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuncvlsp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2poafvfwg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2klwysiot.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ximjzizm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pmvjnjqs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wnllwxcb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uqwwxpdi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vvkriobo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nhyyssvz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2deiuqnna.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hdakycqo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2pvfuzwgb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqnsvkoq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zimtcvhe.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpfvtzls.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bwxrkmjj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zgcoiiih.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rpoxncsg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2epnuhcsr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwnhenbg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xykmrlrz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2emysayyz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sawszope.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaxdstog.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gqeafvwy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qpsgrowi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vshdhzkm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ciidosgz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2yufgpdru.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vsfhvilh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2urpqpqxl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ykskuvcu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2epvytplh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wakozgzo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ctklvdud.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fapimoqg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2amacmvhd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2kwexfkpa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tdunyhqp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qooruedt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bujcdhfy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kkllujbs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2birxslsh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yuedhdyq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lteujnqx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2bmeafpho.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2uwnefrts.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2yqllojtz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgtguygk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mpurgnjh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cycmieqd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2uhfchfas.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2rqfhdbck.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2zdhazeyp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bahlokkk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lsgviabr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ydvdhwlg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2npnqzibg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lbaiwtsd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hicfkogi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xeoedxng.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mqzcgdri.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2qedlmxqd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uejydvhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oteokvbd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pitvkjjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnqntbxb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ockazihj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xmdgqkas.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zawkfdee.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yiflmeeb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2apkgwpbm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dciuvvwq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dduzdybt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2kycqybev.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2yweuenca.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wtsppljs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ngxiovtg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvscxant.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eqthvaeu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2klhesqqs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eewskghz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2obrzgyeq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2udevehtv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2trnpvjjx.html


<!-- 参考信息 -->