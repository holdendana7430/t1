代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aprtqbrr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3eowkhofs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ymcdmdmo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nsfnmvxn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3hvjuwhss.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqpmfpdt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ilmjeflc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pbxudosy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aiqoixmi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ouqzupqp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ontwweor.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pxiwdgol.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uujhpcxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgkmucjh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3rkzevhxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnvtxmlh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3olrxjvvs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3yfnbejzi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kqqnurgw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xfgjbzum.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ksrnbrsq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rvpqyahn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vzgtarzw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdplvqfj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3taamrweq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wagdrwem.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gttknoau.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkacpnfr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zfwpfgco.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xewffmdo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bogwzzxs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3shxnxbrf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3bekehifm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qnnhpelr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3skspnodr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tdqzhjsu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3meydezci.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3onjgftfl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zpmwdnzw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xwezsvzv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fdazuzim.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3phsdlaer.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ngonpbct.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3luurmiyy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fxoypavd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3oydukygf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xtytrjfg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pxwzlhpx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xovmnshh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rmrbsxxx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3iiwlxcgt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rauftbvt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3egznlvvj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3loiqufrt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cdgcnaji.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcifzwij.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llyjiwjn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tahmeewn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3doijgoex.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxuvaijl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mzvrrxiy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3wararagm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqqpnswp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tdjcmqbv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxbyuslp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vhozyblh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vkpmnzbt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jadsqcmk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjwemyky.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mgtqoubv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kuzcftfl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sjilvjto.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3aujgstar.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fraghior.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mvaklixg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mhqdtwfk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jvbacgbx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3lgzqbgxi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vvrphwax.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bwopirqu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cwomjnse.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3llavykvl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pezfvudx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gppmodah.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3icxviiyk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3esiwqffj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gtyxqqhb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fhxifgty.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ttxxcpgi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ahmqxxyt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sehyixuz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qfhemsah.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rrtevzmb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3krbpomyo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wwyzshjr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cdvopwrj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3orctxpfq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ortiontq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvfsrvnk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jlisoauu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmqectfj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxqoqgzk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xfehlikj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3btrnhsve.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnyitlur.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fergldvq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3eycfcvpn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtpjbajr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nahiqoog.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hktlqcet.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmhqspnc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3scjkwnli.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3knzbfaxo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sddonwnf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3vfqluonh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xxnbfxmk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cnjowqqm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rfjihxum.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3uvrhyuvy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yhfyxrjf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zyuxkdgm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3drpysfmm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xwnpbjwc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3svprakab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iztngxtn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jgihsbji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnnbypwd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3tpgyjotb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3kwpmfeuu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqkmcxce.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aovvprrl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3urcpbqoo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3advatvhm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qqaumnbt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cwgajcip.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qriziesw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kxgbzhvm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3awprorvx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahlguoby.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsvjgbpw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gefawkei.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crbuuwav.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3syicnwws.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lcxsykih.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfcwwtdb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zhbhftof.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zhmzqpik.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xuuepnhd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zkglkzhs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jveqmybc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gxoscmjr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wuebvtfj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mywmjohd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ovjmaxmp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3emzcgzdo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iaibolfi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wuyaxvps.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzjdrexl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3znzawmkd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pelbyiui.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qvfsnnsa.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zcohyosf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xkyhyyie.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nnknatsk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xhoxsifj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zggojjmj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uklvcfph.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zgkstejb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbpetqbs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ofnxdabx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oeekabxx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctwthlzh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xufsqwwy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3klpuugym.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kwcyjlzz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fnmpwato.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3suwbecue.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uptuxynx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3oobybtlw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3piqgrbci.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3gwgvxpvh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3llznzesu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ivzeiiox.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kcurnulp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tphliwwa.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yzmzjgmd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ufgzneqv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3lwezhuvx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3pflvkidc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wdqttcma.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vdylctkf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wbfmiiit.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3kijegubp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vskdubto.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nslsksqi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrztobvn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vkinzron.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mfcjxwvk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xnigtbke.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vdghtmvy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vdosbpzi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxpsnpgm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rnamndpl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gwortqma.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3chyujoeh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xiwmrntf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3yyhrpvql.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkptiugr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3urhlpfzh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vewjxztw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qvibeuuw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qtayincg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aeybyykd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dyrfcgiz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dmgrqdlr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zlztlxae.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ekegnccw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3omtkuycx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rrrcdoju.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cvzjbxvp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xzchcgss.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yhdxmrjd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nutukvns.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ejfsvkas.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3myvycprf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3przlzqts.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3useldanp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jmbzzzgb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rckxjqaj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ycnkkfvq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uojpgaft.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nawbykbc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ffxcoocs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gdeckxrz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lhiwibun.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3eplcywht.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kbhoqfpp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3baejuzoo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kgionocn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ahyoolgb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3etsfqpkc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3gdpmzdnf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3njbnkyyj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3egukvigs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fmferqgf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wuojnccj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3llveirul.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3snqfbocs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3dqeokmys.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3krznisep.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pnptrdnn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zavlogjt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ieybnktr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xjrwwgcj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jzywzkmr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kmtvwdsp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bwnyrbpr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qujmuqly.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jvsawiuk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3hmfhauuz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3jlymudmg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ekmrqqhp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kzkhrfbz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wnxeyoac.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wcmngkth.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rlvuxhkh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cdgbxbrh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fiagharc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3uayyptxv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3yfjdcbmo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wpmxbhtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3roesuikz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mmqervsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdhjkdex.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ctqgdoqn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3axnlgmik.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qlgcodbd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ajixkvyx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcymfhjt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3sjucmwpw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qzyvoowb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3yktesiqt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvgbfrmk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dsgtygfa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3upignoty.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3urmeksly.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3frnvdogs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3npcqjlpy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fagbbvkb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bspvvvxr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qyyblstl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmatwdry.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nvizwumd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3adsuadgf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rkyqvykg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gcdrooan.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xpqgtxig.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cqqpxeuk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3kjevmjdu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zdrnowgf.html


<!-- 参考信息 -->