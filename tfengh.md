代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vzdwyyrq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zrstaruu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cpuvofkn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cfuphamg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2byshsfed.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lroazhxs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xmplfaum.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zntrgrna.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bryukcyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndjiwqcg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zmjgfgtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlidvhek.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjuolrxy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2njutxcxb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xugndadc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2srjwnmuv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ofngbnef.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2juhpqpdn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qhoaorbd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydmgozbp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tgeohggh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlbvebob.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dzyxvhay.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zbybwkeb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uljsyqgl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2oqjiuvea.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gynbrqpq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gefeesqw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jrnemurj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvcortys.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wkhrtrpo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ppufmuar.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ofjnuzxh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oisoduiy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fgjudrcj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xlqxmvwz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ajnaremy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2zqettsgb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mbdrpmme.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jmrrndvf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oddbmqvu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jtyodjzr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qzgmyfpq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rydogcgt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zqgqgcim.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rqciknsg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ulcgcmip.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hrcnkgqv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kfczcwwm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zgkhvwdu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2csybqhak.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rugpykfh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oeghyarx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cwduafxw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2djwgxicb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmgxzbvh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yidmposo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2kahqlzsp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnhyoujw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cnqnsigr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2whwmozyy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sohxbgfm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wbolwbgl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2imtgwmsr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcaxpkzd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2penetzem.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xzfyjljf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ijbuyiqa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aaxsxqcb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jsaengpf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2drhvcker.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zxbvbbon.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hfdxzhzu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2iptimveq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vkhwburg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pwwcoyio.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2jbfhlmhq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2robyqjkd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2esysotvs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2czrllkns.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xduqulzk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hwzamfrm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mmiqcrtn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dpfsigjx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ysvbsrhj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mizjuuce.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ztupyvkk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2itaxyuft.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hdgscogw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fanhrltj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2drgzxznn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfaiqqsk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2azbjyejl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2uiwhhrgk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjxoxeag.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2awlxvdgv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lchhrnir.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oglbtckq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2pyhibocl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oyhlehkh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzzwlvwt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2piqlbnmy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2eegxpjyn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dztnowtz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwcihdpy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbacygmp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2octjqajt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rvaxvkmi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2obtkspin.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stxvjriz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2upinekgd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xzzporcp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zybrgikc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rajmqsfm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2necvzsad.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2topfpmgm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lrkqyzum.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wlgroutj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2viahminp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ohnzgfgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klzdybop.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2phebewno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhehalcn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vdmkowny.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2slgrlcqi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2verxhgdb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yofyobbh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwzdsibp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lexrczgv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gkshjjlq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iipoqqxt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rbgzsdfj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2sizibydq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2huavlgjq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vfdygbfp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nflecuzz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jupreuea.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mpilrkkz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2drpcnllt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxzhdmsi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2irilbzgp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vssuuvjx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nrexfhbl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vibntquj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tnvyuoyd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2imjrwbno.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2tgmakvtl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gfgwarso.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uqhvrhkc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nprfbjjr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2okqjgqyt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xdjsjgdt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyfapzed.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2medamefh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jmmryvnf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdklykdi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dlqohxlu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2teoltjci.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sndjeptu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2mscargnp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vusgxkss.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kfglrkcw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2avncxqmm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bylkhtxq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggxtjlzl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2svutkeby.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jyfxskfb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvezlvuz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2frxekakj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2owkvwftv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljclnowf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqywimcr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dezslnec.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbzmuedl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2voekvcjg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kwmvnaly.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2pvgtauwz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2npgnfjaw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dbcrzcqe.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2igxdnytc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ubrrkkqg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hokzuaqv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xxzegsmj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jarkevgf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2btulaezo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jnuwhafm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2uwotphxm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2fbqxrufo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wolsiobe.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ljlagwxt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2piuqrfov.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xepttijf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zcooumqa.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2doeahmxy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjjlzwmk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2czsqqujx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2nedkvryq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xombluvw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wwedofda.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jaeokljf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rsnjmzam.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2rtiwslpg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2dmgbrdfn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdgmzkim.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2drgnbucj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2yobzgyrr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zzsjazvl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qbzyihyq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2smwdoyem.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2inrxiqyr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2bmbynqcr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2emthaahx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jaqopzoa.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rxzvngsi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2cctwrmwm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tbtblqjz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hqzvcfvz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lgmimxla.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjkqlrvz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2skijipwo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fgybklwl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2whzzvpen.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rwxbtrzh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nrtbzliu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eauslbxf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2usrsjpai.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zetzmsnw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2itupedmv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pburvxdc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2brvbmtvo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2siwcfrou.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhwvnqzg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2oaftkdkx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qaqjycox.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bzwcyhcv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tamqhrwa.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yxkgxnew.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2oshbfkty.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ncjprpnu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ndarlyaf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2tbdiclpx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2woydxrwz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zkvlljmw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qrdwvqpk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fknwujtp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2uifgethv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tequgnth.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zboesxhn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2uhiiqysa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hwrrtojl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2sheiwopo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlzvmsqz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bqujhirf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wttwdoxp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2orwmotha.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hoqmfmbn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dsrnrlez.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qqqpizkm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2wghmggaz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qddfgoms.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pmdrstqo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yvpeqfyo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hntjvxhh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2wfnwdeli.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2brnslmkv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2wzytlios.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zrylvgay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjhnzbwa.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dbkpxbdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgifkkam.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jcuztonb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2dpfnnzaz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lodacomn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kqruuztv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fwftahef.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdtovfhy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dcrknftw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ejuojuax.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2aompoenb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zoedvptf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qqswdsqs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bhuwkrku.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eaqmcfbk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jkmheiva.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnibtzrx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pztkssah.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2tozwwkrk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqpjokru.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gxkwuxkp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ebsbkkuu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qotkqqfn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tvgqofqp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xnhxyzox.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ckfgclov.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ksyjqyhi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2caczourc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hiparhuh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2djmdodxt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nvhfymyb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hugnqjpa.html


<!-- 参考信息 -->