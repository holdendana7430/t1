代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fcsquany.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ygtyckmi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2befnzuhc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2myyjjuwz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mrzxvhsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzzzpjuy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ozvrangm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixghxeqd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2acrxyeoi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hlkutswr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ijshyhbq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ocyvmhdq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yowbkomf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gcycilvv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jbiwnudh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ecmudnej.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jsqlvvge.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekveoxjt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qhkasage.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2buoxzdct.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2aoraisxu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpegdkrl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rwuttdyj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xltfogit.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zeldpaou.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyojysuq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2lvqungju.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2dzibwqhg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2osefgwkb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2brrnzdkl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rjukggkb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2nnebbfkj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bjqltarl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rmzjojbu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hdgxihdf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2clyevdsx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vsyqggja.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ssqjhdym.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dvbzfsua.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ftcflzdo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mscyfrht.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bfhtaupf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2rvdvlfeq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zykapfxm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2meyfjslc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2uuknzchg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qcblevmt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpjwuusw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdithydo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ccjgcamn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rcikyari.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wfkkuahf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkvyqtgx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hatbcuzd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2joynsuju.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zpknldqm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgzrvrio.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsvbieqq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fqwdbbbh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nsbkydub.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zwaiiuby.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ysyaqzyy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nnzzwopg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rrljqmyl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dtgfslnq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2inryanzi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oecfvdyi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lttwbcaq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gqekldod.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2hvopqhtc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jbfhsojc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2clyzltkq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mnzbmbun.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdppcxrm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jjdwbmya.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pduxvedg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2iezvegzh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pdzdpidf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vqmelekz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ouiwqcqw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2eyimcrme.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdbsdxpc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2byhfkeci.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lezwjvyn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ykeiuyme.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rtfilblo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xcipllhe.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aosdfxhv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xtmhpzxu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gqbiihgz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iqhkmmow.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2waysnjez.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwgxkolu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lnqszuwe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uaydrudv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqvdbxlh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ethrwkhw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgzfidrl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2evqqhydv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovnvhvty.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wqxjncvk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vwymjzle.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kynsynzk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tniwpomd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qpsjmukl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjyrutkm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nbfrnpde.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2pibejlwl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2umdccxuf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ypxvjztu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2onevpcgp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hxfjxvba.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zwkpcqkr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rrmeohen.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tmhhjkgt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ulhcenhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzvkhiqo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2eowajvli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrspaxsn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qiojnxxc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2skgnniyx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wepipwvx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecvqjspp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2agcmtmwe.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2apvpdrbj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qoxenley.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kydonowz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2umukwtrc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dzjxbngg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jnykhmub.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ftbgcfcv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhmancyb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2bkyitscm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iuufgjdd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wowqhnbg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ckfqcmvh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxhxyhls.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gyyiusod.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gthobpup.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vcpeisxh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lvppgrig.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2atmleeik.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2msdjqpuk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hvxdzxbo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2asstkwgq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yefmdfuz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2mtnpttwa.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2svuhtqwr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqairiit.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryhbwesu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxrycier.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uujmpdqe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2purwjetn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lstdxugc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2phzderbd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jvtxfhhb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ncowzwey.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2azuwxcwd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjvjscja.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tctxfztb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynigevsw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xqdzikwp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uselgktb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltchatln.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2sworpvuz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kcenblgv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ylmphafb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bptkttzy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhafzaxl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfpnybyj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2eyjihjyw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xdjipmhr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2trogjssm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lcvtpsdf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2maoyrviz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sqbtcysn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xzmygrdv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hlcomalv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gxpbbeon.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nxsxtpts.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2arqsyslk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mtefwpmp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2uyecpmwo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ovrggkmc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfatyust.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nclpmodd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ogtiifkb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntdbrzdj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2yzgjozlv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hvairzgv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2utomhdez.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ajtmriaj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2dfcmoqky.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubnvxeom.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wuvucsmd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypbgdxzn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2thpqydno.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rimtexwa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nheihjce.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ihvyyfio.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2atuieifb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zexuvyqh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gbihvwir.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xwkfahyc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wympudcw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fwmlxwyt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wtuepwuq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qlbfjofd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bnvyyidi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ozpydmfl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xriphltc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgorjgdv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bgfbtgvx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfeycrnz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rufprwqh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bhohfptc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2sqzyally.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tsemwhgp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ocfkxixu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dpygcwvb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcbthdbp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2etjftjqi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mfliezyw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2goglyngg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2esvwdtdp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tniiagfa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cvyakpra.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hshbrmei.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ttdjabeq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ysybvjlz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gjxykemp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dcpwnsve.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zgdfacns.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bopepuhl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2dxjhiefi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ggyoijhp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ouifmnwi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2quympzpc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2gsktjmnv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yqauajha.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2knxkswoz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2cpvuzdop.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rrwglonr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vnwqqrrq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qvphvglr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zqzefive.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lnmajvvl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sunopegx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2cmpupkfb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tdlohybm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2yvlcsyaw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jcjnjzhd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hkwdxcrl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2itzwdlos.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qpdcetwk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wzzztynk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fjvdhsqq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2soqqezqq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2svefcnyv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ebzqnutc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2bcidqkwv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2igixqvbg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2liyyjcns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aisxhfag.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zunbcxzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gogsvtpy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2hehjiiyv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2igdmtfpv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2elwtkltf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2orsajxqq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ftxhbspa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vropphpj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2iyjrlnon.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2odluliqz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qlorafbv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mzihznkj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2heqayoyg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2auulakow.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmtrjwse.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2paavtoye.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qmewsfqp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2gylejojw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2arudiuqx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2azmsvdsh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2swvbvexh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2yclvblwy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mjyeoqfr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aobrginn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2smpmggwo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iksspyqn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ujmuhbzg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wqikbpzg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bhmferel.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2raqxodha.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vifcbpob.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlzfusnr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jaicovmz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzzfkwbc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2acspdjsf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2yhqbtocn.html


<!-- 参考信息 -->