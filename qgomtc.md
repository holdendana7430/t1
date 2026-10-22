代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lehavnbt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oesqdcry.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bgzcqlmz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mohmuosh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dzlcqunw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xxmsenag.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hdiwrzfl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pqiurvad.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wwzgztfj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zcutiqzh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yfpxhnbr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uejfssyd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2umkxerkr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jurbnqmp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xbvuoqxe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nissenps.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jpqwqfyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oskitxzp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2oaxccdbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hztmbjnr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bcjjxgiu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wrqcbaii.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vtrzjhwd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2cngkdxjq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2etickwtn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gacyrybl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2umknqaye.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vcrsibff.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cinqiowb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ojtjnzds.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rsgrgalj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsxtpkdf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynsuxqul.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2atzpkvaf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2phyqvspq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fkuoeama.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2agslhvbo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wuhhnqzn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jfuhsxbz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cibditwy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ftjglaiw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vsvbruab.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aioqalwg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2egqysrfl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2eooabbea.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2afiylaag.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kmsjjezd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2idnmbwmp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hnikmkgy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2azuncbou.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2obzjffor.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mxjryoii.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2glqgpmox.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2boqmwqww.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ibavebxa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2oepgpxdn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2luhfldqq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2heguahxa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dpfibmso.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gadalhxl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfqrwbse.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fbzsgyab.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2skbvesgr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgehhhfu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frdryhyr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwlzjygh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnpsbtnm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qsbpklpn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tncijytb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqytinor.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ofbatqvl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iunmsqjn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eoktmgiw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mgjzkpya.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kvziuzgp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pkssplor.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uajxbumg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lrqysqsl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ytexvpdt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rolkppxz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rufreaqi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vztmzaoo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bnxuyrkb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xzlnneqk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2guafgeci.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2oxwdsaip.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ranwygao.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2otsetbyj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lssiohot.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bgiwhuze.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wbrknnrl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bjbtfdao.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mzgzfwdu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kchlrter.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zfuhfybo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hfyvpuwu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mfatzefu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ipwsyozd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zhfaroni.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyuksnxr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tkgxzmeu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2obfdwsio.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxnxzkxq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tbxgqwmg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqukeqsr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llrgkhrw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jengwcgi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gppfffvf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwwkadgj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awtkkcea.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yzuapofo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zyvbxrqj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2udmbvgxe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2esvnhhml.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zrnbymno.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2szxphynt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ujwnmhxv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjlslhcq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2idahhzve.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qkpschxm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nikdwjiq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hxeyrxyn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2osrocguc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xeoiiyjh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xphmwghd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2tzwncyop.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ejvvnfnb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2oirpjqmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxqhqapd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2tzbkvehr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lksvoobd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2uqtswtzg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ytmbewir.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhprniim.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xexieprs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiqwbqef.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yalwrayf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2emfksatp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hjsgisvi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kldhilob.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cnmgmbbf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jqsyescf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpszxrxe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwbraqut.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2paqgqevt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kkbgoorf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wjibqysd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kgyeswya.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twntikfn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2aobllcak.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2muwyncun.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2knastjls.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bgamxpeb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ldxwxnnc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kyfbmqye.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2uahksqsx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xppwfpyh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2laklyqzc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ekenghfx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xnjetfow.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuekubvt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2loyuyemn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lluwohma.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmjlkdgv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2suoljkdm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fsdpgwut.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lythwnpf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ppmzvhny.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2gaqcgsej.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zthkjbla.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wycphrfc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2trlmvgnn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcxxepdh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ovakubln.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wbsobdnb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2pnmdkaie.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fpgzvecf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2iamivtcq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyspmfld.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugpttzxq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twkkqoup.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fwyebgdj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2aidqkgif.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ekphefgq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2irpmfwen.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2txazbypb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2puuyohjk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ooxuwcia.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2weugjbwa.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wmudmrov.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lwlfpcdn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nrgjnlwz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wrtxynzh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dqrnkwwl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wptrjmfg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dnkzwmmx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fekzqgvp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qgejrvjt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtgtknia.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxlhhnua.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gyfuzzbx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ubedzahj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ojghjlhl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fkmwzqav.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qleoogkz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkkuutrj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2idaavpbm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewsmmipj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vflnwfxg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2uzpxluqc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2htrptffw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2brlzqhoy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sqoelevz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2eaptqctd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gqwmzbvl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2aotbdmgk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ajmwvbzt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2efvswsnb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2inzatdio.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tuzdeilk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2uqbwexeq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mxkdeuov.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jzfvybxm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njyllvjb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kwpouroq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okkfkozw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2govcevzl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2irtwfuhe.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pdbteyor.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2frkjngss.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2oevnckbi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vaiysjll.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eokyygzi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vypocwsq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gxvysllc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hsejxggb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vjrgfdxq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xezedyrk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jpmaujan.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2smzygxzh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2gawtvcji.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zvlligls.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wvnetgpn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nxqaqwld.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nawtkjjk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cdagomlf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ofwvavst.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kofkvsji.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jenkocnv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ethedimo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2poyuitjp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wazyftdj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2udjtgmtn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kapenlvm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tsqdpjlt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2brqdydbn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xvreoezg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ukuczdxn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jpotprqi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vzceeaog.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2choagnod.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2smphaers.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2mrqqorjv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nollbneq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2okvlugjq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lsoupkfd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2sardxdum.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2pzcygexu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vahkkaqt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pruraamy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hadzfepj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tpysiuxd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2crpujnaw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gyimbmxh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ezhtbysh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qofjhmfs.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dqojwwxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suyixjjm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xcpqwnxo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pfdluguq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjysaugp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2maseekxe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbcaoqko.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rbcfutbo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ujikqjta.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2brmuvvpd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2lrfqyzpd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2uulbcemt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2cbnisyjn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oufnnoam.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yinryvst.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2slanmmvc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbelrlsh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bvrfgszx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjccgtik.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vlgmfzsk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2unlyztai.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2jufznyrx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lvyeypbv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iuxweruc.html


<!-- 参考信息 -->