代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gvablekkz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/ghwowlkkj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/goeimlltv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gldwhbmoi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gtlumkbqk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gybwidrqb.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gajfokygz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glttewtoe.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gcwsqpuly.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gcflttult.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gctpquxhf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gdazqvtre.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gtsubilkd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gtuptapvm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gejvkhmme.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpzcmpxcj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfozkrtup.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbprghmwk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gkmnzzknu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gvexjjluf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gzuhxpwtd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gqxckiunq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gfvcwbhbn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gxeafmfvs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gwobsbmrc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gooafeddq.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gayvtzroc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/giiyktgqg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gfhjribwh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/grhzgslra.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/grcswbmcf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gwuwkcsew.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/grjrpfqqa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gkynjnrfk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gewoiitdw.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/ggzdrndhk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gthbtkhso.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gothcsypg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gxtqosmsg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/galcppbvw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gkibueymo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gutcnbink.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gpjjwqgaa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gdfsathuf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gofxkbvda.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/glztlfklx.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzworxuai.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwmyimpnc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyxewrlpj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gzirikbgk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gbhmbrfbz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glrmypvga.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gobvhufei.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gzczsromf.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grwxbtavl.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjsrvusdk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggxiwbbtv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/grqfrzwru.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gqlsabirh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/giazuggsv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyzakjlxg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnxzfcmyf.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gystzlmee.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gyyqojgdc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gaecvyhpp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gwrlmsodi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gcmywvmcc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gcrnjczxv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gvczlgysd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gqowyrael.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gairgcwjf.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gpvysxtzh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gspuvismf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gwmkaegah.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/geujninwg.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/glecplxdv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gjxtllszw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gcwmfwnfs.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gbjyjkvnb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdbjxhjma.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gtaiwgtys.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmdadszbn.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gedaunufe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gyhydrwdf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/grqlcbhew.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ggcbsowsj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gqxdurynx.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gorhiuffe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gmswdkgxz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gpfviwzmq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gvgrlqsxg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gcabofeze.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvsxgjayh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvrsqabbu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gvxyuovmx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gxvhrktpw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/glwbiabkn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gntzzbjis.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/grbzqcetp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghdextwtn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gvvlvlfsw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gyjcqhhph.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gcjeeqpcw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gfadhvvoy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gntkqzgmx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/griuxqaqj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gxervmimx.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/ggjumwrwt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/glttqvcly.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/glaiqkmub.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gicyxizik.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/geksayapx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gqyxoziyo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/geqgpdiat.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gzwmwkraw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/glzzjfvbj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjujwgaik.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gyejeoiyh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gclytfuak.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gtwtkzmhk.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/giwtmtwcm.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gogphfjus.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gjvxxrmow.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/glktodspv.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gipitjwed.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gtbcvremm.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gcxrvzaur.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gfvnnmdur.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gwvqsuyrw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/guipmiern.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gwlafxwny.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gzeklssbx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gnlpzwaqn.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gdfmqqdzg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gozsicugc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjiobhpzn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gcjhrarwg.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gpsjvrihj.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/girbpcubv.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/ghfanjwuy.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gvdojnpwt.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gcbmnvubl.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhuzldzl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gxfegwrrf.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gykuymcak.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/guzzxqjgy.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gedpnupfs.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/geojdgosa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gmxauuqmh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/guxhfrqkd.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gbhloqoyp.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/glepqablt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/geofcbnju.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/giijlrrth.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gwucdfurp.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/grthozjba.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gsftgexnf.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gibwukutu.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gjqkkwpry.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gmwkxnzfe.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gqqqtmifb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gwgzqdkje.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gudoctdbx.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gyisqoczb.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/giwkdrrwf.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gowyfbrgq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gazuytxzs.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjmehoviz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gfhcpslsn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gliknqbur.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gunkydqfa.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/glruniibo.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gdeyptyyh.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gtljfbshy.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/glerhycir.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gzkbfyiby.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gajcpdvej.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gffkqsxsg.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gltkwmejf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gpscftewm.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/ggubbmund.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gelbqyecf.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/ghfvgtzbv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gehuoikiy.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/geuljvpkv.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gpiiaywcm.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gwllzphqz.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gojnocesr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gcditmzpw.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gxrblhnbl.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gjknoqzzi.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gomfmuxyn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gyipnraqh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/guiffehmf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gwahmkgxa.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gjvvwpelt.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gcuhayihm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gsqzsbyik.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gkqrdqmkp.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gkgwmmtnb.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gxkfhqbpj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/ghevlbkvx.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gfaedrnmc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gddmwimbw.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gjpyxslvu.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/glnaemwzt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gftbsvtwd.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gcajpyvfd.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gsoqpjdkf.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/globvpixa.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gzbsypksn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gayhwuntq.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzbzpgsw.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gflwloinl.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gnwnkwmdk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gamhibdxq.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/ghkmcmmzu.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gaarcqfqm.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gadisvvfa.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/glunhylpj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gjsfurlaw.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gaucbfpud.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gjteqwxxj.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gxvxapsfz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gsefhgojh.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gflvzsazk.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gxlssonez.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gxqhrjwsu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gfdjuctlf.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gzqjhasxx.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gweneecgq.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gtecridyt.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/grfpodvxi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gdzxvmqpw.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gfddxnsnk.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gasazuuug.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gszgaqhzw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gwpnwauzt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gqfsczyry.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gahmofexr.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gssmdnjmj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gqfmmuwti.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/govtxfxeq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gpfoxdpas.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gwxlfctmo.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjdbhhtkk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gugyxqost.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gljfjfyig.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/glglzyima.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gwjwrmgug.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/grfetgyvj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gvwvotmby.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gjvluerbz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gtaeaxnxj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gpkpkvagi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gjxzelcpb.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gdetudstv.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/guyqxrxmo.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gfgrmdrmn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gcetnnlml.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gelgaddnj.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/glgeyjeol.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gomzbassd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gagdoxbqm.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gfglzknik.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmiujtsne.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gpdyslscq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/giqdvesru.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/guxjqdhsf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/goehcelyt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gadptdjjh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gfhgjulrj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gxhhanvzv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gyrwtmdaa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/goflyimwi.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gequkyuoa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gpfeuslsb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghchxsgdh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grqwyyviz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ghlwhdqbs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gfjjmxtgy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/ggxytkqmd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gbxnfxzyu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gtsvnekix.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gdxqdnpgb.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/glgtevjyw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gdaekonkb.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gjgakvbsc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gftilchwl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/glxrbdjog.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gjcwauboq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gvyhlpmon.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gwucjovya.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gbkizltxw.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gnsilfhit.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gncawefzl.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/goohhjueh.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gwoaoexaj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gesrdltsz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/ggvabaxsb.sHtML


<!-- 参考信息 -->