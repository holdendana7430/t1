代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3egproyyw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qpqnwytk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rllcmgtf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gjmztlcm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mdufmrki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lratvtxd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fdjjcaka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zazrjqns.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3szmizueh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zfozqekz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dassdiev.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3idbilrrn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xnbsbvbj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qqqwcgob.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fisemcku.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pfgurauu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wtxsnyob.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ienaqefq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wchxsfgy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsryxeco.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3atoqwatz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkeokibu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3slkhzslw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hjdcxttp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3bcaynvkm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qthgiciw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ayuyqfvn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hftgrhhk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lsbcllxt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bpugregr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wrsmedis.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ozcqcqcw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dvtttfvo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vjdyxiyy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qnvrsbvo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3blfxnhfe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lenoquep.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ihspqflg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qyugvmvd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pycxtjpa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rogaynvk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ispwjcrv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ofqczyjz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3sfqmocfg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qqoqptwp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3sedkstbk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fpecpnut.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hskpfiwc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clivtuoc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zizxqvlh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3foxqseno.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbqtpbos.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqosawfu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3oklqizoy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nnocpdze.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lgyudrjk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lluvivoe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtdmspvf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3irfhdupa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkzhqrse.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ysjfxehb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wxsejbnb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zzsqucgd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bxjdzgmv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tegcpdkf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3avucvkei.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tsqomtny.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rfjemhug.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lxejejas.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kixaplmn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3yedslpjl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3swtrlzxn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3urldswsv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiekgxcj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gterwccx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aarpsuor.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mggbrthl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zibhnibi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vgfkhhpk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cqcbufpt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3nqtnrrfs.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhivnayq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fcpqkciu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3aszfeqpg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fgziivax.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xmteflbn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rrmvcltg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbfppzcz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ggiwokqg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3stroedwl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vywjunlb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eptjltot.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qabbmtue.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljnnmwha.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3iqcykwtt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjdecbuf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnykamej.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbldafei.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bwrxawgu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldbamduh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrrteuyh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdddplad.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggrvvhmi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ywaopwoe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3chjqfgmy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vzdszfxk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xrmbvsrb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3okfmhxfi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nzgfcdna.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dxndjmym.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fxpkefun.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zkgoorud.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cbkuoxgr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3norfwysu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3amzetrzz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3agfezvrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cieryknq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tcvgmlms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzhevrbj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3updcnxzb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wehsqazf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlqripog.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3slwminrt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3nhvrnmqt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jqolteei.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nlzfoogp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3afjctoax.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kpwcpqhy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3orhmhxya.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ntkaberb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3nopkqcmm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqboedqz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3hymtwjxn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmuwtvwh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dwgnxyal.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3uozgnayg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3msvwsjua.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mbqdhbpw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3swfmzjxs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lmjmziya.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fpydijky.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fiyvfyei.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vrgeawkn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zndjbhhr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3obevwrdj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nvnjbxmg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kbaokxqd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xyuxuyfz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uezepvwa.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kwqeaphk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdsddpnm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibvuwzgq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bnzylgms.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fhzdyuzq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3prihfcnz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3iglrlgqc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3pklccqzj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lbixdsrg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyzhpfym.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ltwzgkzy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cxnjebkg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ppmsftep.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3taeoabka.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ebcstwtf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zaqvrdwu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fiqbzvkz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bfplvthl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gdnylxwm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wyxnwctr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czesthzp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rpbifxuh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nfasnqig.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ofvxcped.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vbofddkm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ntfpzhyj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fmytwsoo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3atibbrgj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hlqnlgip.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kifposab.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mdvglasc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zgqgkznp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zbusebbh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vgzeopkj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3nsdqrqvd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ifxrcbwa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlnglrsg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wnhirlnr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ftpldqen.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tqzbrtdj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3trkdfjdo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3elnpvpkg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3axinhhxm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3rncbsktn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hycttsfu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cmpglimh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlflkzhe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vlpeczpf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pmsqirdn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3lkykzfbv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rsbcxske.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mfzgvjhs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3eijwsvoh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3luiqjtci.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3mxefqyxm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pthfcpva.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yhieflat.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vfatpsvy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zrpvohug.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3pfstjzcf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gytwrqut.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3epwkkecl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fbqgmngd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3frpvwkou.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xpehlkew.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcfvuwvk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lptvqvmv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3htnxassj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xtggjgcf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kwzmninc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ufrbvmnz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3buvgnnwu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftrgzuml.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3epronqto.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ehxiwuab.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ytnflldn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xepdkbta.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gtoanemc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3stsfhptp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lrwgpgzk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3frpcpuvo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nxvlybkr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dbuyfuuj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xghjhfqd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3sdsvadbh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3uyloeguv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vebtidqd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gfjxbewf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fkjtuzre.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3crxwccqt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jqbfqalw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3leakxxin.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uerdoxmv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gctsgmjo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ksmhiuip.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3nlrfufmf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vfyzgpis.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ouyzdwux.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hpghpfyu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3thxnnigb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sgbkdqwu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gfpjuwns.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ahkmtlhw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3znunoxww.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ijubclub.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bepazzeg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zovymtcy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3egfvqbzd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ikkmaaue.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gakadaav.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ahosntws.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zfrcqlnh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zhftqhpp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nyqqlsbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uaehskmn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ijqtbvcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iifppwwn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ivurnbes.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3gofuujpm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xxptlcud.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bizrhoyb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hevdfqha.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3pcizuktb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cryeswos.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3szujmlnd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hacwqyvj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3bxmurezs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xvgdxbgy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3omxfbvks.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dnsxlqdu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhuebtwm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctdjxdvk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3onhtbwki.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ehkvvblw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mozmnycz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3davlcdvt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3cvagbaic.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wxqnwxxa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ujyrhtsi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qpmtovjj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xeaxukhx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3nhtzqcwn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3yoqpgmqe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3woxunzpk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3acjdebgi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bmybktgg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbtmutlg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3altbcipc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mgqctijw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jnsgjepc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3kkowvdju.html


<!-- 参考信息 -->