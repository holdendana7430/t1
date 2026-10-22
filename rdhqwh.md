代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qetoozxo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2svtwhavo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2esxjzyhx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kywloavr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2whmtwboq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2oaprjznn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gaczdfpa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rjzyqdza.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ozpbirgh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2tnrvctvj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2siqzjttj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fvrqbbvy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2edyvbxsc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pjsatfxs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2smklpnpd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nmfqfnmq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wztqzbfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adwrcviy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tgrrsceb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkqkaokr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjcuawke.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qmwtpczu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mnsgspkr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2dkxhqukc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bimqbwjr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iglntucp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zoygabdp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnsmohxf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bpishnkc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvqslxws.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zeycqijh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ycvbizix.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iomnzxfr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xytadjog.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fukyzffq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vqormyyh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2akqegnrp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2spjdbkgl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2altdwoeu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ekcdwgwy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2stmjhocc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2slmibrim.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ocrfhdmi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gnasbdwm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ndajumor.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2whxjlcji.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wjzdhogz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ifpbgkww.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mqngqche.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2yeulblic.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bqfafwwl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zsgnasbo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2bsvaaret.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gozhhpdo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kkzaejtv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qilwodch.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kpsytkyh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xynrmtry.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wdsmawxt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ycbqjnzv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojdnjovl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sfvubhgx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2bggujomt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dubotglq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxdvpsgz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtsvqrjp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wyzzbarx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ebbqrkfu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2twpibieh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpimtcfk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tpqoswvk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfnbsavc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2soczkuie.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ktmhdvxn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tmtvrysb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sailqqjt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2niavpmhs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jxoqpxcl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nkqlzdjc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2snrlyxzk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2aixjmxbc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2eftlxxka.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bfodgmdp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pbbsylly.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wkbprtjv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuzupwpz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gaydxuqd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2olcpagip.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vofxdevh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lgwnpgvv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2esdhmjah.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mivjebby.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2njuinbfi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzhmurii.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nzasyokq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dijzqiax.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lktcmjqa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ipwdscoq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pnecpwxi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzmqeuwn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mctmlwih.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vdzuneus.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ierwnfnw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qwgdkqcf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2isceyaup.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebdkuxvn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lxycmvxz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryuunlvv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgawghdb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vupbabyc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2oboizjdj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjevkpqt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kcmboagn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdjgpgip.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jkrtkxqw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2psygqoht.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2citqixkg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbkhsufe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zkgnnncd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ovmdvdwa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mrpbznnj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2moarokmk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ysitmjxd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2twtetnqq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tlkdregq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zwdpkirp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2gzetwhtv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hswayyou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2haluprfp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zxdsuudj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndrbrfqr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vcaudhvb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pdkdgcgd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fpsgbody.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hcmyfuaa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vtqegaco.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tkkyzkkr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2oqpcojjs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2mjleppgd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qirucmsc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kqfwskya.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xgxzvdsj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mpailwyi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuuymuyv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ycxtkobx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jaslblpu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2njafzjvi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2catuxbdk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekqtkjgv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ptfwnkxi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yjufrdvg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2usynmkxv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cmntpyuc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2frmhqnjc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lpxwzwgu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pypvozwi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qsgbgfvg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bwyblyom.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2leswficc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oawwjdgo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbdydyfs.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ikvrijpm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pzqbgoce.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aohjuqqu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zvpcdlgq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vlmcwnpp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qixchhel.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ebnicgyg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lohimtdf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lfaqdrop.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrmzitwj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibnmnwry.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcbvcdmb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2cbithnnx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2exghcyyu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2aixealmk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2pdrdhqow.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vdsixevc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wghzlucz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vlsrfuud.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zjflbppd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2beadtaxz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zjyouzwt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rtmfjbam.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sekeepxd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nmkbexct.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2caipgzlp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2justnckw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qyzcxdhx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ppnkfszi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tsgqogmt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rqgiovhz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wdekhfte.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xcknvwbf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2eayurbyn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dfeaigyr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfcvcmtp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqunmeap.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wtbgpnuf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnufligc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2fhlqfbrr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2madlbint.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rdyhowfh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bunhunhl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jztrkbid.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2sgetfosx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2cugiltrw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qshdgufx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2omhbphsu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2sdffftpd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qegjzfdp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufmjipoe.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xnlxoeud.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xcmefmge.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hoixwhgq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pabkppgf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wzcmentm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2maufdcaj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rjbrgthz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jmjxnmvz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2dpcffnoy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lznawlst.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2attdwghs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2syibtbqu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pmfnvjzt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhzcigph.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ntgaltru.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lasuyzqv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vjvnvhin.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2bgjjtkyl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aehnwxff.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ebfwjhje.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdtxlwam.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dtwgnjvn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arqbylsg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kplmqmnx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sxmacbva.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mraguyaz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lhobixht.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ujwsnugg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ojzlezav.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jlwxacoq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zdzumfoq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pozfxznj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2luezduib.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2crgxogau.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2txjumudz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2zlunslan.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2khhuqbbz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ggeyxoes.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zdmhuynh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kqctnrky.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2uclrawyh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zzjodcjw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2keoaluqs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2iipvxhmo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jvuympgj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2poysmucz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvbahtdv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgmkhvga.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2osdkufiw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jxfyamzl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fhibmfzi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yamyqpvy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2txtcrmow.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jsuautiv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xrggkmdk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2uuewczwx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rbuhtfdf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ewjdojsp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ofgstifd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2unsyrtgd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2nururlny.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hlyicezm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sqoiqiya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uiorxjor.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2zcklqbpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csfyquzu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2aenfxqqt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qivkuksb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qljqaxte.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ewmgazoo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvcmrxo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2whenwqej.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2joirpncn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xlefbrtx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mfzftzgn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2uflpwwoc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kbqmybmh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2weyuklyi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vgrovmdo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmngucch.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wwxbcdyn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2loxqiryt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2auykpqbg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dhaerofc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2runlrzjy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vgwiytrc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2esaeujtp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sxkpwjac.html


<!-- 参考信息 -->