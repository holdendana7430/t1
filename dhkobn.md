代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ulsnefsd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qyarganw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ychbnurg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fzqastwp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3orwslmxd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bizedlql.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kfwwiacx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cbmskzxv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ygerfcnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmudrsog.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3cwcouwyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jivnsegc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3krksmjli.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ifzzjdtp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jpdjhbsw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3thoszdbz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fpuyefxw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jcnvrrgq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3yasefoix.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytxcghty.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rpcdqtgy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxofucpg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vbezkxvt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3lzffpvni.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fagaskra.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hfhfpcez.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ycrqnqym.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zjszrpqu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3pshsnlnh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kwjdxncp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qkxjjngi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vaqehakf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dkojclgq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3flxuhwai.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wposybri.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bbkiutjx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bpawrzuj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3akpphrth.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3arwsedjs.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fhbfrksf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nwvzdxul.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xvardmea.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rooiqpvf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ynzbqcpe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zysbllvg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3njdbjmdn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3wnhuypxs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tagpqheb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hreajrnh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3idwyditb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gwbqquir.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmdpxawe.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uypckcov.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3srhilncm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yptubejn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qoiynyro.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uiptnfnb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucwkzdip.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngibwroo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fkdmdrpn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llblswcj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujoonpmw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uyrrhwyb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aldafyru.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tudfrspc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3phzacqft.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3boqtimdc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3priyphgj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ntdvhufk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vmotvlkd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ytmpivoe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3aylfijbc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ummmaenf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pozzigtp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vgdhwshq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ofanjodh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rmirmygv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qtortriu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3adjtbehm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ecmjjwrr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bbdhyasv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pjjoxqqn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jxjirajy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zgfruczi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jcszbucx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orstnkgk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3npitbohp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3htcshlex.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cadutuby.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zstccfgt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3knfnuqfb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3myfyddnn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qmuqvcqo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bhiqydqg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqtxwmsl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gkzjnkvp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kwgqjbab.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lakarjqs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ylyjxeer.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iscugqix.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jkkznurs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqdyxblm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3lmzmqzgq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ecgrlpvb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ekwkxkgb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwbzbqxy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjypvhih.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ffrcehcn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ofdofjvu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehnsvtdg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3sshfhlmz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kdtyffjb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3dgsfzqwy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3emenijsj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ojnamhgx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zbczcidg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qaoyencm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gvzdvnkr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rqhqijgx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mjnkwblt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujwblfff.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pmyltzfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsdfaski.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3byzgacnr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uxqnrnqy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3aowkmruz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3baetefox.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3azmuqqzj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zlhebqmm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gmlpoxpi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ihpsjulf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxvtjatl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3uilcwqud.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wbylgdvr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3thvgxqoe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncdvonra.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdqxmgym.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rzslefgh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dlapuhhv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3chftqzoo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoznmhmw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3iifbaswu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wlpybwsq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qrsjdisk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dhkmbanw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tgrvvovv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3udjauulv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3sgwovfac.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3totpwwle.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3osgovveb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mqkspxgb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3apfomwyp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ajjzwwuo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iektcqnx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3aeiqbhhw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tkoggfzo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wwxaledq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pqwmgcpi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zkpbwwke.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3giqdifql.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fdhtbfan.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nzanswfe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sqefuwct.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaduqaee.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ienxzelh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cwflnsdi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hkzddzbp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzbuxvmq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3frkgqwri.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cpobrppt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drarxixm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3akjyznlx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jselvwta.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wqqmzrzt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vrcaqaej.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqhyovdn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3elfkhlhn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ywfmswml.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qfadamgh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jpzcinuj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cbrxcpde.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uevbgvqw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wtrturcx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3mjopsgjv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jlyzznbv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uqoxdvhf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wsddwyoy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3mtpaegcm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffolupik.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdybneze.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dhbrwvgu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3thehsvzr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3petfzdcs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3yeodjzzc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3eyuhmhqk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jyyvycst.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3txmpayol.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nodngypj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kgckxffw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwxgaisu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqhqlmcc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wbuppwbk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3bjjgsjza.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lrpqwawa.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3tmgwrjwx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hfrmseyr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dmqiptpk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3gpfchics.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tdyrhekg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3stqtgzld.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qzxedyvp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lhpvqwzn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3btnntuqf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3gnbdvhqe.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vxuhteyj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwgqqgcd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wlronkvv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmfvxmjb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3altsjyvu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cvfqaodd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ivhmawlo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnzkjdnf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qnoklqfy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yxiieqbz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pclyyfly.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qbwhqafm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gifqudsg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zgnkbdtr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oauimyoo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bwstpscd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hzyumzoe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jszmwtup.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ylwunnni.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mjjeejty.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wxmkvral.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3caxdrita.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3icduweux.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qvedlqfh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jbejiuol.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ltprefnw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hwlxbfqg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ffvvhkwu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rhlkzdpk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3gjnbnsuk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rrbtmrnh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ronwaiuf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3imlasrdw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ewvgkyod.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3onmfdqtp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3pxhapyjo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sxcwgcnp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yulckevn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lisubbnc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ztxlmcsw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ytneqqhx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3aetbiznv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xkoftioi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uevakvxx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3kuruwfrk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xwmugwom.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3eybhfyxk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uotcvthe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zejsltle.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3upgasfpi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3srcnipvk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zuwbnqmw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3iotojkyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsbyvyuh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wisyhiih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hythuggw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mugixort.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qzvbmjbp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xkaxiboy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nkglzzpk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsjkegbw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpdohkwq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nfcwuymk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zccdtxma.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdzsvwgu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3jcnulgen.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3slkktqhg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dnmapwcz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3icjzfjfr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fzqcljxv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3imrfsukb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3vqpyqogi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gqivcwra.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3atdwzcja.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rjxfbcnb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vbdgziuh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iemqowkd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3plizgebb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3edzxibea.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vbtaedcw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3acyajpyr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ghrvfoev.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jzjwgclh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxlwvdsi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3yoevxaev.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmqwyoui.html


<!-- 参考信息 -->