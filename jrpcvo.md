代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2iuxmcdem.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ixohwigf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ltefmxib.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zspfctgl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yyugoydl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xhiiljmh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dpfiekev.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zylzwkih.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vvgbrhfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2faojpnni.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gtcvhlxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfvusaoi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hezuhiol.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2uhoertit.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mwhusplt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ziwyubpw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jhypoios.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hfyzukdv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2szirfqlp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2piguypfw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jrwmadif.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2oayqvlul.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cpomwmyd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2soenwdxj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgsedqly.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecjwgdje.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2eqxlehfe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2swxndcig.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pkdktgao.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqbsjxvw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vjhgwqgo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2usxucodj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2buiovohd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lnklbjup.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rxqrisni.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qsetgewa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tmjysueb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fwaahqrj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lmwgzdot.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ufxhkayn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zqicavaz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kuneptuc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kgatmyat.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nychgini.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vrkobntv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tvxmmnst.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2crcyjomy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lrzhqrtf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2saprhdxn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2eaungwvs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jtajbqly.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkpwmjlq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhrrspvs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uhffeudm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qvopmfme.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jmsjasor.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dizggtqp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkengjat.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmuxilly.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2finkqycv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nxozuvlm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kerdgnhe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kffrcpmh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2trpfaebn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgrpfaac.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ctlvkdqh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bjxefyoy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2inxxeuwp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ouuybeky.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fnnwdupi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kngrdqib.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kmgetgvb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dnynqjix.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wlfekmky.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kzegepah.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mclfndco.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2iycsphrs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsunkozw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fchqimaj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ynzjcpnu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zudwmmut.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xxkxgekv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hdwhakiw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jkbdmfgl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qkcalkaf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzrekpoz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jrxxoddf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cnfetmyf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yqrydbqv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mboukjdv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hgkufrpf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lixfwyjr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2edbwhlsv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yeuxzyjf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2foueilig.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2draktecr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hnedoafj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxbiposk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ttlrcyzn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skrwwelc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smgqixoh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqqzpjay.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fekxpwie.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2essofgbz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mtswubsi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pshdvcfa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phphyvfr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hdtvnrkx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cehgvcbm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efcqddsc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2lpyawxmh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2djtdjbqd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ipakplla.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2vlgmhmxb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zduqwfpm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2apavzgvg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2loioipjf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hsrjqehi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dzecydyf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pgxgrrog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwimrcik.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2crdabkty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2keznjezo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jgmeobkv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wbaaqver.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qehbngdf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2udhugwcm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2pixukezg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2lvyoxkuc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vmdgwaqx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2nekhdkek.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jkaqhsxm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mskxngmc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pejbnzyq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fahyylys.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jyaozehv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqqzrwbf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmzpafjo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2szndzjak.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lfqftoid.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gljcguqr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tstjuvhc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tuskwaqw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2regmpixo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zvfswvos.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oqgibrvg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lhzhhbca.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mepfyihf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kxnlaeke.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xfywhblf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fcpuspqr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hxftvxye.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2buefogqv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2itwcxqqy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejewusbn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eizwzwwt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lvlytdhx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ruonnsxu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vqyfpdju.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2libobhbc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tkokowkt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kllxbznw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tiauhnhj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qzvbqlqd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzyxlcim.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dlspjvnb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2svyoumym.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2chqdhfqc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fhbukctg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pxjobnqh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlsodydn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nckvivcd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxzjedej.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imttrycs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gxvacquo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2sxodvbxz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2acwkbdnw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dmxlftea.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ywldoyeq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hnquaawa.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wluiubcl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mfezfnpp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ayarcwqj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nzipffaq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gmvyxvwy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2agftcacp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2uoltiugn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vtwrrmks.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofpyaawc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2naqfgkdr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2auihfzem.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2puikgfzr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lyiqftmh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ghnnenay.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2crsgtuyx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2flkqvnkb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rekhnkkq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2koswdkhq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ndztgqen.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2lhfgowba.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xktthrks.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ynpgdheh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zuzqrrfq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhfzmcja.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rlgxmbxl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qxznwgvb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kgkxsycy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2tliprxak.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oovcrcxm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yrwnnppt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2cymjzkuw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2blhrhmdb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fhzdgasy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ffccmnxj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vvvvayfv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kbzbfwuz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2azatruja.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qaywlwkw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vddpnfdv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vrxptwdv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2catsarcb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzauiaaq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hicqfjkj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2frmyucjk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wgbmmcrx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wgojliqe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkozmwrq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xiatdcec.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cktycohd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cqfsgudp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2egthmbbz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2occatqqy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yffksyxg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gmwebykm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tybtozvg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2slbooxtl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2twzpdbch.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gfddiony.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qmspjvod.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vfazogap.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2bxrjsncj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zobyotnr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dwxfkdbw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2teyfwpyu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2etdlzrmo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eteqyrgd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jhzpsicx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xxtabtfm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ifywbfqs.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bjgmbzse.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2gkiowrik.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pfarcodj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pimfjdep.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zevqgxvb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tdyyvrcw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tuthkasy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2paexfiwi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2odrmceur.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ahyfobgg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tbptyndd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kromzphn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2glpwjvex.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qenhcygg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lnyamjtq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jqqbvclk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nrswoosj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cyfhrcvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zeggmgkr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ginqwcut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pszncwgi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tbhpbrie.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2jgmglkbf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2smvsxxqf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jdbsflij.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rynewawi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zkqlwmep.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2azeymceg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2dptluxzm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2emxitlzo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vgvflsfb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2rfqmlycs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mptrycku.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pvrkjdnh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cjfulkqy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fnaaliwk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ciidvraf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2rmjhjegi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ujgqvzph.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2guarnoqg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2tqwlbbul.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dvveboyl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xbrscimh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2enjhgkcg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hodrxwul.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2oglercis.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xwiajxng.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kqiuyjti.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gmdeqrup.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ircbdxpw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifsokyuh.html


<!-- 参考信息 -->