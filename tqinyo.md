代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lxkvbxuh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bmzeqwmu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hniumqco.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bsxtcndu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yjvnyvgp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2slquucpr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zgsxiaxo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2elftbhco.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2idwioxlo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2segeynro.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yrgrorjp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nmuiqhtw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hlbnaonp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mmrmmbmz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wlztfxbj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ovwdxfjz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ikzmemtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mainyxvr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2cwobncrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adshtxcr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2stkgmske.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wrsylhlt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dcofckyf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2shhfbnna.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pdwgfker.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ghhukbxl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ltmurmpt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srjkdqsg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nfrihgto.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qfvkmsyy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jelthrbn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2teqmpqiq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bqwuetiq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajbnfgod.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wemahfnz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fdhxxovr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2thwmxeei.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2oalqutbj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ssfqnhbf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2igjdmrzc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fdxpcmhr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fugsxorn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gktukhwf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tczgxhsg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kisgpdcp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xgckdawr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qqqdxxgk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2skygtmih.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2txmhpwlu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vwrfmnto.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kioewuat.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fpzegzve.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lxxbxadk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ditqkcvs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qavnybgi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zymzcsxz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ocofzcmd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2tieisskp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jipkpcxo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijjgfqek.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hocividn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zviqttni.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2aoanhhsv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jhwimixu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okkcsfup.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fzzqbkzv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hibrtpfw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zcpeyqvi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vahpowqo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2linrozkz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xnauvusu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sanibqbv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fglhuuck.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wiovwfws.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2duqpwqih.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2srtpavyt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fokpxxsc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bxamgpxt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tgpmkgjj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vhrwseft.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pmdmizio.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fjspqloy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ohxlakec.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2pnwjlhgl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wltitehg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2fjluzhen.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2drvvyjob.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zzaelucv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yfcqvekb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vxqqlgyr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vegksyvr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qntiohpo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2xbgkfdrf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axacelfn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wexhjzci.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2czjtsjhv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kktadpcs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2najevvtb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2klslinlr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqxpddqh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dfpcnppv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xfskyenr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvszeqka.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zjfylxih.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wofsdlnp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qoquoyoc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qcvhulhl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pncyrsdx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dfhlnjno.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxmwmutb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hdscrbzi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zrqvrwyq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uaypacwe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xsxsilhh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzomaksb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kgsselcs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tkhamtns.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpphabjs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2obfdtxqd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jqkukhgz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2lifnkjph.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ltnmkkuc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ujuxcmig.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rubrruis.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2kctwycll.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nrgduqoy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2aadhqppm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dypbekjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tiqooknk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2spoemtaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qltmbcsu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tmqrqfjr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2soegrkup.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fqerndxo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qbzbxjbo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2recazkdf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yidjnfpt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ebovlslf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qtlnzzdd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2glhrnpfy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qqdkpazp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vzmcgoob.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2sfpyoalt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvidqouc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dxnyidta.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lyytakcp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zfeyxwah.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2eskitddb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qoulypvk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vyptfslz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2icvoycyb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2iifsosme.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gnksxbka.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dvsspoex.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vanqrxis.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2awgmabff.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mgnnjawj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bapkdbfd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jscgrbny.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bxekczku.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgqbnkoy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yzcnubjm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nqyftwsb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcwirsiy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ldpblgog.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2utcagzxj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gvtokvnz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kucxyqzc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2adklyjna.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wpbmwyyw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cjipllki.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwwsqmnv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqalvsar.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qgomtnco.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qovueztv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sywbnlsi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2zivflsqh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2byvbuokf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mbfroymx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ktgxbbxd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjhbttcw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2emlwhstz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vzqficxz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2flncznwr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zitaccqk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jhigflmu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rbnxrxmc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nebfuenl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qcaxvvpl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eixyqkoc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zixgcjmy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ajgnbkps.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2raassald.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kuvjxjcb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2masuprnf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2oydtfcfm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xswkbccb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hrizmgrm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jugzcmvw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2bffkwulc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qqbtilzv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kjmwqndy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2grkvniqa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jjehhnfx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zcecsseb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2odambcmy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ihfbwayx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2dtsqexth.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qvqbiuvn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2kuvphlla.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wvyddsul.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjtxlunl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ulpoepav.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jzfroavt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yjqinlic.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2olednavk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hrkwkvpg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ymfnrlet.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mtngahbp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2flllrbtu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nzygwgdl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2emnjeuqk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ykcnmxwn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nafaylfm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opooyvja.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onboxwgm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfqcqnzb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ayjridpa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2dmkspoul.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vqcsckmz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ehywcfbz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wjxepjkq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2veebekjw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gbgrkzki.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mamjddzq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhtjeqnz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjbwmqa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dlfprsmj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pukkkiik.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rxknybna.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2tvtjlgbe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wexfpjov.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ryxqhwqj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ijhxgdti.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2axocdrof.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2sbqukiww.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2owowvbbz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jvqpydvi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yehdndpp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ybgdduom.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2khkfwjrv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xtceeqff.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nhydyhdo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zvevgakm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2esjgdabu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2krchjioc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ymizxolp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2yptvteum.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xsvmtrba.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xftsavlc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2eprosjlz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ltgkbsmh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2hgmodkpe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nufkttpd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mikodjbe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sbqxukdj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ypryoxfc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2flfjibya.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ejodjrtt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jbkkshkn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2admfgnij.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rdakavxm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jczmtxgg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2izeakyrt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fudmgcvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oczejxzo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qlyqmyog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyiwcclk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2orzpkzrk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqeljdh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2uybnetzh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovmksmsn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkzycqur.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2idzdlkmb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2bokbjlbh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2fklzgntv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2rrntoqyg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2chjqcewk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qgeltcdp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqzapvuj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykrsxrqi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tilkxfwq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tcettgkg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2qooloyrl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ggsuzfdc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lsqqndbd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hmprysfk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jbfebygx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cdqwubmm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tfivtana.html


<!-- 参考信息 -->