代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zhbjdops.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yiruyhhx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wihjyndi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xhhxqvrd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cbbiogxj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kmqniwwp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3amfalmtx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qsngvgne.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jjmhkdgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuqndurc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wnfxurzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqfyerxr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikjcaztf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3egtlridb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oulxftak.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3kavljihh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dqalgyqc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fizxfnwt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gevvbuqv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3paalvbqe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mrjqumgp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ekqjwvmg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3sbgjunlf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tdkwxqzk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vnomtivw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hdomwvdw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yigobpui.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dpnwmeec.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3bvpsvfbw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuejblru.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rilhvsls.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zqnyaiqa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mbhwgmxe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3azgqtfpg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pommpums.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3klgbhkwb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ejgnvyuu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rmrwfolo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3amteyxtf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cmlvhelm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nncfwpuy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3afdgvfsm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uyylspjh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xrjzsreo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xcvgkaga.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3iywhkwey.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lwydavoj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ywempdjp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gdfrcoym.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dqxryggu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3typzyyff.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llhdheap.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjfixran.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cnjlprgo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ppaqyyty.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aaekqqre.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thiwhhop.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgngwnmw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvmexyri.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aamwtzwy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxrbtaje.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3isfrfaee.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aazxvhnv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ssajvgzw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcuveewc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3laumudqd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3silyjgqd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bnveowci.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kfknwxzy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kuiebrek.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ykwwukzt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3uvlasgek.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3rfhqeknu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3winwvjno.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lhczvgjk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3lkuateer.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3uleaesix.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tiwpbjbi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yvqbubix.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xekjchfi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xnquatuk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3atebwfdz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3rvlvukuu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iopvtefi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mlbeqhcw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjrqezns.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gylanbbk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oarshxaq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qvnxccnd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dznuylqt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ryuoiyrj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nnpglubc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gjpwedyg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3spivnngm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ignyekju.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vaorvbtn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chmsbtwq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tabpskrk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jkujhmbd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcemihpx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3azoxnpbc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjsysnid.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ononcgti.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ezkorrje.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ksafhiqp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkmyhvjm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkauwwdz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nchqrhjz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3brarzemi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpegqyzk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kyhmrbjf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3tmcfmkmq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qvudzkcz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wkzvuhdx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mzgvlbnh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tshfkury.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wwyebubp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xsqxnynd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wfybewuy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3cdsjegyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twtmgbig.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3aleqfrtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijupvvoq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dzoeyhco.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dluuhpsz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuvoxjko.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztrfrvks.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckeqvvqg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xyrudjwu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3sfwsbgjw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vpawvqrn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgoddevx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fttaaoap.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ebyxndgd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfeufnkg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrzbsxgn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jjxfsbkc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fiifdnzo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xyqjyvdr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wxwyrpxv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jgbbmqyt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3csxordtu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lawrbygh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3flkcctzr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cwykmjfa.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3smnpebwc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wwbhexgx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3khgjffts.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ugvveuoz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vhjtrpes.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ztcjkagr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jswidkca.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsaojyke.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnbyhqle.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esaaavva.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxytxlqc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pnleqszp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3chqdkfiv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3femhutun.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rqdvmnjr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3beddvslw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jjztccnk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxeenbss.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mnlfubqx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rcvjhcgs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vihxtqkx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhuqbddm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbmbxgrv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hubtetqn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kijszexf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjyargck.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wanvcuks.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qepdzqvn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwabghgv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rpybatfa.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpmsqmeh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xdnkxprq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bxedqrnx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3tldyehof.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3johygica.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ftbqoykf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mcasqiun.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fllebnqe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3tvrgekuu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xwvxbliy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lwemqzhh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jcofbjck.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3sdtgdvyb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ytlnbkuo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3swwmppkp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qekebbte.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3klyjghag.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ypxafkjf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lxvceodb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecoihwnn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rbyquncb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3amuwlpbg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wcfejhrj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3eqxolbfl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilaxgljs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vatgtprq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dhnwhgua.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3uxkcwfon.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytiaqrpk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3riglmqgx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ewzpkuuo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wkdbepcm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sqwtktbf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tqdgexdb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kregvzip.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zzivijgs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3firjcuon.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mhxfocyo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3dvtqaysg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3owewsawx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hlgvtuiu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvsttpbi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kygmurrq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xaarddim.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pgzkdubv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ravwrmbf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kcwgsqmw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3azfmejsk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3eskgyeyb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tewjwxno.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjhszwme.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rdvrorvf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3inwquwnf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fvtlztmr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xokgtscb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fcmtjlvd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ffejifxx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ojomjxqe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xppmjphr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kkyoybqd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pqpzqtug.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wgoqjsnf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bfykroqy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xudfphuh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3irnvbhlf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qryrqxid.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qlxxmyhk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3slpebwna.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3iccfgpdh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mrhrlbez.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3foemeodd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3airwimqz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vrxwiibt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gzvpfzlo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lswlekta.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3bagoareh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3llbwrmjb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3tvhdazod.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3knknkhnt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nzfojolr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3oocmwfvt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tyihucdl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tgkkzrzl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gzayvqwi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fdylrypf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3yknhslpd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3trljbhha.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jxbinnqn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xlljfpjg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3obqwouhf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3fcpzhzne.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vgjadvfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sphnozfh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3igfwfjht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsqzshdh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3kcllmjwg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xdzavaxj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3opikoccc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wqrzodpl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqqlxwec.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjjuciyz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rmujddna.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zbnwpvff.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3zkfuqsub.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nwdndftg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bfsrcnds.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgprcnbs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqmsvwgn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xusgwepq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcabkljl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3bfglnudx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3lerunkbg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lskrlxyd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nnmpfxae.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bdhjlfrt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uaehawem.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nnzglslj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qywtoche.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aqrgzdkw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3etkneyfw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3rvagyoug.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3skdeyzxf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3twcxitna.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3eiewvbtk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3crtggzpg.html


<!-- 参考信息 -->