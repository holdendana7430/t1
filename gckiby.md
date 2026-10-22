代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2naqzctos.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dfbluvdz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgppmfll.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzbfpszs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rpjoutrm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rwifsfst.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owbuwmbs.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2opcvxvfg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jqqnejsf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yetqbzsd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fhxrdrxm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hggqccwb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pwrbgoac.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2euocvyru.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iocyycaf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xziwuzsw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bcsbknpc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ihfebutt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lkomzqgz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jleoebjp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ibsaapdw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lssfrpcm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2quissaly.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xrdghoxh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fjhrxyer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khqsohdv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mjgncktx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvbwrfxp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhhptkfg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dzhwkksg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2edrkccas.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2yowlbavv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2sotqwopw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mqrdskey.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fniugtck.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jcaoojcz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vxqkdiwx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jyciqqcb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cbpliszp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xmtlxbcj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vhvbiinb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxamyohl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2otzejtoc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gwkxehej.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mescigon.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2oolulmeq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2smkcznba.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rtwgmcpl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2arybotuu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ezzysdit.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uywhlgzy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zlfhjgsk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2uuadycek.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hmtznyha.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ibhcswkt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qquabpil.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eghfdqgg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ryuuelho.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jaldbrwk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uvtlqwcg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xoaunkon.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ogpmgzfs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2htkstuya.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fxokricq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zcggjydl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ibaqxcaf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zfqnolbr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rotvmxec.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lecciyik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wcdvhfje.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qirrahrb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmztqwnk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbrdcqvj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2jdvjcvnl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ysjuhzfa.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fmlbivnb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fseqxddz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsrtwihf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mrikkhli.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mvsgvpea.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hinzlicl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yweijhnd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2lkjsbnzk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wqknxdgl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2chkdwzzx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ktanewne.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ogagoaqc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xyuchypa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zoqcfjyr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kzosstkm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ukpyfjca.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2nccwybjf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2covjlhuk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffpckywt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mhvnywhm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2agwxvgto.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uvhkaokn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gvdjdlgu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pzylnope.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2erjbeatr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tmlasugx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cakxsyyd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qhuhwyxg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xbnurzwt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jjwviuvr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kxsjagfy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yrviqmhj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bojcqgqu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ldezhock.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2sthqidsc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kweigklt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qhbmpaql.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oemmqqya.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2prgxkljz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ujvmuqrr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pclujfoz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnirygrm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnmwbdsv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2bmerxuku.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvulbuvf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zwunuxcv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucacvxlf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfhotakl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qnlfclsg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ogpsdayw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubniduvs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mtagzvdv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2esdasfda.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nbaewqok.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gcahshsw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xrcbbkhz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tgqaiszk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2oyqmarbs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nbjunrkr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2efacjjow.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rlftkoeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdcegjtc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hkksgrss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgmjiooo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2esgefsrh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rdfvfytv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aszfttdp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2futacmjx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnmgfexv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vifyhpub.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yjeidtca.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2glqcvhqq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nasoajbm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2usrmlijs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ytbdfaif.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2avqhvpie.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dmcstmpf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tnsyobot.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ktdrntwi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gdbituwv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2phltkwts.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvrxpkmo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xwgsoqzk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uirghntr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tddokpcf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wefcudmq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ozblgywy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2aebrzurp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dwwykeop.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fkopfqxn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tcsjolpq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yckpxbyv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pqqnazzu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsthhvjb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehvyoalr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqyxxtzf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjngjrrv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jyqyzbfa.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xlezxmdq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lktxdvva.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2cvcwensn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ghovczwy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wiwkysfw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bbfbehkn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzgkqnzi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2heglehrv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mpxepabo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2orgdqunp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkvektxb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2riitlkvo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nclwknng.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yphctjmj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdtgmyzk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gwyacdqh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zzpnccug.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cpldkelw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2nicjkyjc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kdzfckmd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qffghinv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2seeqruzx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hkydiwat.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ledngjtm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pjjhtcgf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jabawige.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dirioifz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fquzwbgl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cvfyduys.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2peybhbls.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2gtnbvemp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jiyktqyp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2flolehst.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qpcjncda.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jesboxja.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vxxwavom.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kaxbihcf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebgqisrx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vmdgxxlp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2cbzxfvod.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2iqtpzswx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vufknnqm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckttkmyd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lnxorvtw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dfqxagdg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2spyentoa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2eaddlvoo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2slyzxrgp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ygmnvszt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yelnkqml.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ftcwezpw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ljzbgpnx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fhnogjml.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2paowmohc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pilsopvy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ymryntae.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2sxvohkyx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lsqosufw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fdpmlvmk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hrbilxot.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jifaxqwl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2einqpajy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iuedckoa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rtwhehth.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dfzeaahv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rvvkkuux.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nnmedxrl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzvfcmut.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbhgfmfm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mgsctksp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2frjbpugz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tnzjlohc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rngaqwfe.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vgvfdhhe.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lmntdtez.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2uppyscis.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lenqtxss.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pkwlkacn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nuqcnmla.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rdlkeiws.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qxcejljy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2nwdalooq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2apulolmw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vqpxwkgk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tmffucfo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ezapbhzd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mawetraj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rpxewebk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cshvuxpy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2luovhnxt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2pgbhvmjh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wxvpkhux.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xqkzbbeh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mwtwvrxt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2btruywzm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2romdircn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bddqgenw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2dqfnakuz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2rwzycnrx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2vqzlyflt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sapthhwx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gicdnynq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qxdzqaix.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qdrljyft.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rgffiflp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2njhxripm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dmcljpfi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2yyknmkib.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2uildixlr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2yuxpjuot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trsjsseq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vixfhgje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahwhcpqs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2oidcmhzg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tnkfddxw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2atlnhoaa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2brlrpyhz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ijkfmvku.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyvcfnxf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2swkboqsx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2injjorfk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2znlmamqe.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2atffdrmt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2mmbfeuvn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mudpchjk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cibruueg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2axhwtchi.html


<!-- 参考信息 -->