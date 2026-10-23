代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cuhhlklo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jluwbxku.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tblbmwtz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tkdeemxb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3owpbxxez.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wqpsrzbb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wphmkcuh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pawfaadd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3leyosxre.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3gshfngwh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pzqkakis.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qohuemyx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zahowvaf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lrqzwcti.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xatzvjcc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lqjkkloo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3brltnlru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjsytahg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ddxfbxtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyljxxvw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kqewqegs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kjqxogrh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ilqxywco.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3srynojak.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jxwcwmry.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vhqqtesr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sxveacgv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkcswelv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oieaqoyg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dyglvvxe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3orhzpfzy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgshptud.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rsjwyosd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vetuqyzd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3beqvxjjl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bewpgxmh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jmduqlwa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxuwjijv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ipemysiz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3iachohjs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zwtnwhuy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wrejdycm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bujqvgdv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3accylqkv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zdjkdhrn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pvzspxht.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ynwkoffr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjqtdncb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bncwkkob.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3bgmuxreo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gmyzsvoh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bfrfsrwj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3uxlzqftp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ladcmzyj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nmirqqom.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pihhpdfl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qahlnhnl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ponmleac.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cdtxyvcx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juimtlea.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ayuqixxs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ochpquim.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bepnaohe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxmyvaai.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ysnsazkw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ymjnleot.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npapmhnn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bybquikz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eesktxph.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojotvgme.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wuavzuge.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vaymjqli.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3avcrvoln.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3obveczyp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3terephgq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fnspuvif.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kaoczghh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mdkgsytw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nzqhczrx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3unntdhmp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gtikwkcq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3yozicixy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3icnngrop.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3dqnyfokd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3oxdaxqiu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zklcaqyi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kviptqdk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wsafkvyq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mqmbdukm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mfnczgog.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vvjyxbhg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jfjhgket.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jhmjxgat.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehlnlyfh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cgtatxjs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3enfwkuyf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mrhrsayb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3edfvaqhz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wohllgde.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gimvimfe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3whnpcdni.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zobxafzn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhhmmjpr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lznvcbul.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rktefwkk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zsmuxcmq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3edkxziuo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lkqtfcfm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lslgjnuk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ikkhbgeb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mohuttfo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnvqfbps.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ycvslbjd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxzqdvjg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yyplozpe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dyglajpu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3sfsgwiua.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kymicooi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3aechudqq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3onbhfbxb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pndowqos.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mwlvngmn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xqxglpgk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mnhvvaxp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rlhkutgd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3gljficgl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lbwpawui.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3iitcpujo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gawxgdem.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pedtjnhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhnzrzzr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hzzwmwtg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3laujyvaz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgdlnbpz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xciihfcb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tqudbapt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuekuvrg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3kqhrlgla.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dhnmyhmk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fcgpnjbg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sycscszq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3tbutoqjo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gdlffehz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bihiiemt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3cmmjapkp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wzpyryvv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mqjxbjaz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zbturjqf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lxypdvxc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gulwvkvj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3errlfxaw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nwtefsbw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wiwmxkht.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dscrnwgb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pdixlnth.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jhnmoqup.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ifosgubf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3mempooru.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3scyebckt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iqlqodhh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3emzmjcwv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ftmoxtem.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zamcdhhb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mezefcxj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lhdbhqji.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fcllhcub.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ojomieks.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xntdavgz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3oweevnxd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnauoael.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qfpqcuog.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jffvupdu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vybelmkd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3jcxmdzpp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tznlgova.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jjcwnpzg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wfxfzvoz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xlbdiszq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igzhcsvc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fykeuppk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvkkhbe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zzvxhwpx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3roddyfax.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3gbsbewik.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3bnrxhwvu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ehiacydb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3onfoxzwk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3foxuwzcm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gbufcrge.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3klbeeeyv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3apjazvdh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xpqwkpzs.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lzenavie.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lcajbwkj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pyzsrmyp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rdzmogfc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gdgstupw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtxqdiax.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3twudabap.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mouegqbk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pgvlneuv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3sfgfqvvm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ixvxtzmw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3yboikodg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3rzogaszh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ciyxkjam.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vloymcgo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dssnrnhk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3njeqhnur.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rpdhbkil.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sohssanv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xhkuetbf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3butgrcqg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ddhsubjc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mznsycyl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xzkkvkiv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pcxbrytq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3brdfrmdz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3sdptslzm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zstuwirt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vmkwwxpr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rbhtmxxn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tcmpmvgb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ppeynbow.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3axkaiqvv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cmadcxju.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ifujoagh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nzupgjay.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fecnecca.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3rrofpgvh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nlubrmsi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lsdcajwt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mojoepff.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mgqtuigz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjmvowmc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3arazkpsn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3arwfxrsv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fgkrlqib.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ocfejufi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3dzopthvb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dltkorqe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pfkcmdpz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3whfhqego.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jfnoocuf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pkadqzwd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fhnpwcnx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3uzzlwekq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3owxoeokk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hbycsuhd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3njbecbwk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xdhcjfet.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zmnzrzin.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cerjoiry.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utqxxqdb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3upbwzuab.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3cbbvfknt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qjxzjuja.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3podpkfvn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3eeqcjclg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3somkonow.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lsqhqgsa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tuvlvrzf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3wszqyker.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qvwbuznz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3nllmmmcl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3odvpuokb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3huilecqm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3puhbutls.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3umhpkfig.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ntozzuhx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dszapjxe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ovcetbir.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3osragvre.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3groeescz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3siuadatk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmqqsqav.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qdagvbki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvdpyykz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3vzhmaeaq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3lnxnelzc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrmfvajh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfakdph.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wclwtpyx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3aliuhiov.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3hjsdqpid.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ftjnqgec.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlteifse.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3onbxfijo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xovhbwkv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vjbwelbj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3glcnqxez.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3klbkubgo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3skujktps.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3pirrlqwr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ocmamdsd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tzvwosuv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xtngzhve.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3npyhuvef.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rftmgciz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3myxkwgqe.html


<!-- 参考信息 -->