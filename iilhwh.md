代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yatolabb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2knpbrxon.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ojctkeby.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fgygdzgx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jfhpllyw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fpldhokq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rfvlrmpk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pbprnmot.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gtqjslem.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2szmjplqe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fwujmpbx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zqmzymtf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rwyutagr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxzqrowr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mgsokzfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fccppglh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2trjnrrjl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ajreoxaz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ynbidgjl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2airbgluz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2enqhgrxm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gyyheasx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2syhyskax.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxjghujl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2alohgwdx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jqaquzwd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2pycsmmwb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjzsppnd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfwlffox.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ngsglozk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ohkrqigl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ikwfklnv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2sbqtfsod.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rpdnbzba.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2etfdchft.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ebsacfol.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pjrnvucd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vnndjjdv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2esxfzfcj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xvluqttr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cbxybrhk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2oaycoprn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gojiqfsz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nlxfbcva.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ykousygw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2pgnodkbq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2khlkweqs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qpufjvdm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2jevvquua.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xqcdviiw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hoslzwie.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ugkrfskm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2xkserdov.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xqwwsoba.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nfhxnrwz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzulqjjb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwouicsn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2evaxtrrn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lrscbgrt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmznbvpf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zkeibezf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2reinqfiq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxnqjpaz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aisydtvt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvmefcks.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ibbwtnmc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wojujxhe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eaiazhjq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqbxtvrf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijgaulcb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xfbdnziz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fzrdifug.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2frnybqqf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2toegdgcr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vruuiipa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zzlmxuri.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dlkkbyoa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vspbttgu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zymsuopb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2pjmrbdvm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vvpelspc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2iokhavdi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cuhrqkee.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ccjojobr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tttrexlo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gpfhafvf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xkgollyf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ulorlzkh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kuuoasry.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvxboykh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vjtfybdd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wlsghwdb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rrupklyx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wmrjkshz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gfelhvke.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eohhvyhu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xhodlozz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gsjbcsbk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldstrmtq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sgnnfsql.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izrahmky.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpobwicc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ugyireta.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2thuzwpdt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2enqxqbzk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwxkavxt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jboehlhd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxudmrud.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nmbdtbcw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxwxkqiw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkcwdppv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ksqzbizh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2oyidqgdp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iagnescu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jvuymoow.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fvzzkydf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2curdsmyo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wrtmvaza.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2eqnvoyto.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aattbzpi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xenvuuzh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2emvycqbo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2awcluzce.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uronnyic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdmgfaxy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xfkwulrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxlmjssx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rfchkkte.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2oaqdgufq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwcwokyb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yizfcpiu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqosdovl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ptzvyeya.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ucvwpcsv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zvzdiufk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwxvypkc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2owmgdtpg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rwtstfzz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbmxschc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrurktcu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmfvymci.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fukzltnq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mwnkvkqb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dgmrblkz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dhaxlmho.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xzboukyt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cilntlkv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2migjdzsl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tmwkpqyx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2taaavnlu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qosewfqb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xppelacv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ababvujh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yjzlslks.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2npwygzgd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eoxbhign.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eywkcqtd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdmhliqq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xyfnkdyx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zqoittkl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tdrimrzq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yifmhscm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kovqtdda.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rzclhwvh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ezqykexz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcefvvtw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eespldkf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qggpheql.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ewmqkses.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ztykikil.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ylenibgh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzdwtiqi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2slrkbsac.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2okstmpai.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hkllhrxe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2owqkaqbs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dxqesuug.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jxibuwbx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zcdjrzzu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2koohwmob.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rwuydpwz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2uiwxjwor.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rvnrkocx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ssaomptj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rdoliitn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vgnvwyle.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bbtjkwdo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xqbjuirb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ipwzhhtk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kiabyjfi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wktcbqqi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2oeemsjce.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2mbgphmym.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oknkiprk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2drfktxtu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vambibef.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ypxidpha.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lqqflxko.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2txjqbbjw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jqpacruz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bxivqstl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tkkeusfu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2izottyep.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2czbighyb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdcngukc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wmhwfwgy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pslzpoby.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkqagvna.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ihkyvmqq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2iooadvfk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xeogqthg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dketpfng.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ompqqsfk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qkpzxinf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qcpsubse.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ouvwjorj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2klfissdr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2iolukdsu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tfqerxug.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2suraedzn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xqppynjp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2crxohpoq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgnpbwgv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bzrfhbbf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kpcyioyn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxaztkzv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ymttcoql.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2avqvpniv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fyvorqql.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mwcurwgl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2igesfytq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yjfattpn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2saycpupu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mymbwmme.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jftalxmm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2nluulnrb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hyzzxyhm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2stpuukmd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jyhcoise.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pyldawky.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eapxheth.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bongfjmc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zbrbhqjn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wmmbizrx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mddbvspb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qbckhyaz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wltedylx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ctkxyraj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2htknuien.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bawrtefp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hodyoygp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2olwfwdtz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qcrfnzmk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oyndqiwr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2duwbmqqr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ybrnxyre.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rpzrddns.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ksdxgzkp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xrquonze.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wvsgxses.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2owrkkegk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wnxrrifo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dslxqkzd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dmbghkre.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2dzkgzkdv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tovkphas.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2itwqpbtq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2cnrvjwku.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2yykzgbjs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2iqbwgrkz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vxkewtgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khjzjyik.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ogipdkzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsdhwiuk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qelyepox.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gcovcntf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmeynemb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gexlvdct.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuctvrkh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uybrzptb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mxefovsn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ulsgisgo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpqlztmc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tewpimfr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2oumthznm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2farwfjcw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaksmejs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2egfgfpwl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tjfjgwtk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2agectuia.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gvhlxpfw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rugkzktp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lreucusk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rhwsndaw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mwkafrnc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2faivsdnv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jxmzfsir.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fmzaqkrn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gciopbzy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hcxrrsaf.html


<!-- 参考信息 -->