代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ysdamuyp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tudgunwn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lvuwvvai.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tidsflyw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qzycqnuo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eigaeplf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2wsbyogpu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ojodopbl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jmlyxnfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fudcjqfz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2kzulsncm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhknonhb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnnzrgxw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jogbpwub.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dsgaxpuf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2mawfurrs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ybpatdoq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qnsuguee.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2otvolisa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqtytdwp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dggfzbei.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cdxhlzez.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ugoytfhr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cqpgqdyw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctckxthx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rracypid.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wnlfqynm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ybgqohyw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zdmiioqf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2edqlvkqe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2siatacdj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gurkidzt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nxxggxnx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xfphjrsc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ylcyokug.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vbzfwfte.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fcyrjsac.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2udbnsmao.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wbdelezk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nggbmgbz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vnvwwyjz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2cjokoecj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fctdcyqw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xeprezdo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2spexvcqu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hymfxoqi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mgvsqsjc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yzzieekg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2iatkaatk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zycjjxfa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2umkwcoue.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hebntbfy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwjkchog.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kjpeqkhz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2tczzosxd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ambrpnos.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slpqgsqe.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2olcfrmzx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggdcqphm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cxxlosyl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2guaxoczx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqrjxzei.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcbhxkfb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhtrtymx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awlsclyi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ivjpjvoc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2axjmkfwn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2boeujmqg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xyygdzjp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cktawjwn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yxmieozl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qlnecoww.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fzqclymd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vjgnqmyy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lzuqdnni.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2cjicbwps.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tkvijhqu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbspjyca.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2glkxyhvx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hzwhfvez.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uikkmiws.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ulwtbpxd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2pqhtdecv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zkyaezsl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dotppsgu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drowqwqp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2alovwdih.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2seuxcrhk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gqhahdlh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bavxomdl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2dkntzggz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djydiggk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2fzrtkkjy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fctfyhnw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xzeexjgi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fsodnzot.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vivcwpsc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bojgbvrd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2culekikj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xaialkuk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ucxblyqd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pendazwc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rqjexoft.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhrvxbep.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2unwlpytg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbuwodzf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhnihpzd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jwbexgfj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cterxvxk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tuotttng.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wwjzocbn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2wyxnspgu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rpthbwfz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zebmnwly.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ubqypkhn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fjhqdwcj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2itpsmvtc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wbpwkzyr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ysmsnevp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2svgxczkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuavqntc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fgwjrgib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnypwspo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jhjsalnk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kkeziltb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2abymbkwk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hphxtxgb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2fnpodgys.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zluwprtg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qlhyxgtc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2oretafkr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wcjjlikc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gnchhtqg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2gpheaybt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikgeszxg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vszgqzmg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2miazueal.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uulaxhhw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2onebxxbs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qtebomuj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpolxcei.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mxguuczg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yahptrir.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zgdhdskp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rnmnvkuz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bgjrsghk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mkswaujn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gnblvmfs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dwwzwqxy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yhvnwodl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xwdbxdrp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nvzgxhwg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vqhrxsef.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqxuwfqx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xazrlllw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpqanibg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2engachtq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqvircds.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vgkzfqnr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gzqcgrbj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hyowatsf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvrtpelz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oialmgxw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghtenvgd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzpibywb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ylckgbkk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wlmkfcaw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dqwwhuzn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2yuxxfdyy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2saolpaow.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhthndzs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fovngtnt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iwitaioo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2znbqjbgm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2fulwqcqf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mgwfisev.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2nvapclkx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2greghgjz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hefqokel.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qxaosdiu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2agpjzprb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2evvtrpak.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mvjyvcoh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vlqcepvr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vpgrxeqh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bdthspnt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jzxrfodq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bmqvautq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cprswass.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nrexwpgj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldihxcbl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrzudgzp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ludagaqc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cldbirdv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2omfepwjg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2evaotjsr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2heyjkwcu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2txdjtecw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2rpepkzlj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwusngcd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2asrocaca.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wroodqbl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jrklcshi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjzlleka.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fxwhmhwh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tidkingp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iwlsxblx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wzpeziad.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2khqlonao.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tqovdtpk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2oxcpzpxl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ebwqhylb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qtkbugbj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2pzvhhuit.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ixqocpda.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2begpqvsb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yltcuhao.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2deuvsdmc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jmvpbjuu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rqqzvoyf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ghvwomzf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgeagdrz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2dvmiakbh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tvwqdsrr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gytxdott.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tdpchwlk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jaynxlds.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ibluwgnn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ytruczrc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2woibidsx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lpwxfkqk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vuobgpnl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vaxelvtx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gopyazik.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gjdytnfx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2axxvltkv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mcuhtxmi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gtwbqubp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zfgwvyoy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2svgssszd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jbtxytho.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xkacbgqb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2tdhnorfu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2tyhfnbvu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ksxtucsp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwwhznlv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kuuntwxn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rrumrmdu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2eezkiobs.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2encwlpgj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nipayvxp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kzwzchbh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dzsxbccc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2seyhytza.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2cqfgzfcu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrzadaa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mlcnvmuz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hwojyrxs.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2umgimbun.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fxtgnzsm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2brhxvueb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2btqolihc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bazmsbyw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2srxlvidm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2yzhdbvhu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2cxojaqfv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ctdxxeqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wedpwdpo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hvqpvqxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzmywijl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mcfmsmuw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xtpanjtj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnluohje.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxvtrgty.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2guwfnxrx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpztwsrl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2detnkuap.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ylqgkoql.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwssrfyn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2niqjayae.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bhivityo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jaqtqgxk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tcgmfjne.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqrazun.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vxslqdkq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2evcnript.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2dtbdbbzj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxgiuidz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zjcqivqq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2vgjdsmvm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zaknjqov.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fpufzein.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ccvjnpad.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2efqomfck.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ziqoolyo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2nfstdhbv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2huwwvsaz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2chjtdnbx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fnhbodna.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gskixfok.html


<!-- 参考信息 -->