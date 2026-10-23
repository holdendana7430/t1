代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bcycqrrq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pxjxbquu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dvjqowyg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oaehygnl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zpxzqujw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rnfnpamk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3paocxwew.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ogvqxvrp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fhlxzqlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvkzwegg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3tnpcybrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yoswqipb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3oqyifolq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gunpszdf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yypccuvf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3asarbqkx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nhvtmasb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ehxihllh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xnrudfjh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3isanltio.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3axukbeyg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vrgojszy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cjaneqrm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3apsgmapu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cyrwqvey.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvwoksjs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jtczhknv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3odwrhtnn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vjlvutrb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tsdjmfbq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3axmimbnn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dvlukqef.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ejicwpum.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nkyciglg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cbtczpvp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3riimjrzj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gveupraw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kzhvbpyp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mdglwrmk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3epjdpdoe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qznxafbt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qlvlrcoy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3miqkyvnb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nplrqkhu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lsjlrtlg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ttseydhj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bbanqowm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gogtvvjs.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3epstwxgx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qbchqpbc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cqcvxvvh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkygdaoz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imkqfmja.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qwnmvutx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3unsrquzm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evkrtfyz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxsixanj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbhvsmbf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jyscdluy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vdxpljgw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cilioejq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjlawrmd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rlprzjeg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sctmreiy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qyizuzbf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hyxqenfy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3yiomaqca.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kkixgkrp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3axdgpxvt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hbxzgnjv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tziluqlf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3uijoysas.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3rzpzisop.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fwpjwrlx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3nnvtmnoy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3cgxipubk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3usgdtnwq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzphsgla.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3csnogzas.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ltitmnus.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ynexccbg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kpkdxedw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fggrqjzp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jgrfegge.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ztomskcr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evsvfzed.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3isuvicdb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gqfcjwjh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3opodzjfk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ravdbvlr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ffrtpesi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kyqmcydg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hylqhben.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3anhyqeku.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cgmsnqke.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3irlmayin.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqefqdvt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krwpllfs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3fxgznktw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qacgzxxi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzbpeojo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cphekjmo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzfhlubk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdpkrqgc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fvvbmlbg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kiywtnoj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmdoeamp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xdvdrzki.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ozilgxib.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iyjisjpd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zchelflw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vegesoom.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tblvtklm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wdovdrgu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qmunndyt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kvvpihgd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gagaagpf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lziuthnq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vepkwzvj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3eejunukx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypbqmitx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gmtfqtmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbowkkji.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hpbwlrto.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tlkkzcdn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3smlfcdgb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilxikncy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pnkelqer.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3taflkluw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3invczibe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pdytgizs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cocvigqj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bujwufky.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3arwwxvrw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3nsfpherc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lglactgj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wdfdfjzf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nwluejec.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gqonkqoz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qlormyco.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmxpqyxh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3iqoduzvz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gpdbkqkl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wcmzolrz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bmvuespi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gyomixax.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zwawafli.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3yefdjvug.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3beqrdjzp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ehemooen.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3stvcnzqz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eyidlhss.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ayefwhuh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfizxhtf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbvgulqi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzezljrg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pojtvzbk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3owdqlshs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3amddiadt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ucxwdymq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3aavreapb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eouofmyp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvmaqxkx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypmjokyh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3syhwnliw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hlkwnpyp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zdrdviwl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuxknvgf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3fzsnjhvf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3khbfhfwp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3htomplue.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qztrqfmc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hfqfmufk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrymsczg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3iotadzzc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihvtwjzi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pjswscsp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dsjmgysm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qxgffkyn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3umxaeakg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hcfljmpz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3azjjzrnw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vhsnykuu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3sqhjhoqy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mjvqxqjm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ystntext.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qulybzwu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ksorhgar.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bxqvmyzs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3akpnzztx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dpscoswp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjrusxgq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3fksgywbd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tninckat.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vwiszexx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jtfkcrxq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3nbmxiecp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxzrwuys.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hztydpwm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvmmpvzx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojmdfubo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fewhvgvb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wkkwjuab.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3phhihdbm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nudxmuxp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3gvzayjcw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3geopcmne.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3btuthjot.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3augnmsys.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kltdoyqp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ppwbzdvt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hfekkzho.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bvibkbge.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wylsstlz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kijwtdgs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3elgxcayj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kumuxlbg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fugshjcv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sgtxmuxk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ubslskyx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3eyiqenlv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bpsnkzaz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mczfabgw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3azbzbgqo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xtnitejt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tjqqdapu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3najlzmtj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkyxqect.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zbgwnnim.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3exvqzlld.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sitmvihc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3feyswtvc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kddoqrkq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ygyeiagq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3afubyknk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fkevinhu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bjyqcaqd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3usnfeuio.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3aupogwvh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gurlcsgb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dibkambs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3slrhnkzo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gxuhuipb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cwovrusu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nzjauiog.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pecdvwid.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hsqbvcim.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gfqnhumh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fwvkzbak.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dibuliaj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gvrzxmbc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrlrbspx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bndlexal.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ofemabra.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qbfzjccm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3yvuasnhl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rnbirmxs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bwpvwmex.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3jbgeumqq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3iusflykz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pjulwauh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3znikvusv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sdxjbkig.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ipyczuqf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ymqwptyo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mpgxedxc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hezymgcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygwvahwf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sljlrgwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffoxjwto.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gjcgrnhh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hdncrcsc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eonjskzh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrgkdeyz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dutfzkqu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjoeywip.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3abopbhyp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hrbpyftw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rswewtiu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3flejiwqs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3uvxctbfm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxdxbodz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xpvzuvxf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqpxatap.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ftnsuket.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tpbhzbku.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mexnlsrx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtopccpr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dikvrqyc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fpjrtgep.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3efrlaniq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vkdwlgam.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fqyddlau.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sesqylog.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tcvrsyjs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3koejvpyw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vscpcfvu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3chagdxah.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3sfpcijvm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ugcifzsc.html


<!-- 参考信息 -->