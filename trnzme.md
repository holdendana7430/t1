代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2neetbjdj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2olwxrnsw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rwpaagdc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eepgsyua.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2seyocjln.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2buuioaak.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sxvklpqe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ortpyaot.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qorvxovu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ecvwwyci.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2umyetgyv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tkoifhzj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nnuqqrez.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oimnyzoa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pemnrjrh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lnclkjik.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2iieyanhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwbclang.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2igtmmtex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwsddnwx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qkmftrpy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2iadgcdqg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pppnupkt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2yqtdpsoe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ghttshva.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cweoftfh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vgceyrkc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lisveajg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2txapkmgw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wmddrevc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kycumiry.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bkpnsokz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iigunzet.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaojdzwk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pstskckl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fgbyialq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rouscphw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlcwklgp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ktmlmyrr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kfnoywiw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cfflrbxd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aqnppbpd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yhogsupv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zffwiiwb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yttmeiwq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ikyxfhfy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lytlugce.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xpzoasdm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wwjiudvz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vcqhbwqk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dzxtiohq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ynqmovwj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nuegopvq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sfboowyi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2prybghsm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2exskupth.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nykkwalg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2uyckwjcr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2taocsdal.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufwzodvd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vubywqpc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2idonzrug.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vvhkdqvn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wicpjkva.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdjbfrby.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gwnfzsvi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgnralfi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tbbolrbt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agfxfdhv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mifvllfs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pzjlmnsv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asvrlkmb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qdpvahhj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ojxorbtc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tvxqtutg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cywmndgk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wvfrpwng.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2obczrymx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lwluqzzj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2htyusriq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ykninlrq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2uyoujxpm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dyqknrit.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2uejvfatd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zajruprd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2lzrkofzg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2khvxivik.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dbagyjnb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zrgurxgx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wvqkqakt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zqcfiuap.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mhskrmpu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2aliwpklt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgostrwc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lrxlcifo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pefiqcwg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lrighkzn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gmciznrs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2osmhqkqj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axwvbvia.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pkdruvsh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ygtmfkqt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugjjtund.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2glskjpsn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idkvrxgs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2biptfyyu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2alzccxkv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2reiolyfd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jaspmykr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wunqaoyj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gzqeymlj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2doewvwqt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zgdeelif.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qykjqray.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fdkkyexm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2poigdozn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lmudeguq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pplggwwn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vghlgslb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vphgktgv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xdavihqr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2pxevkknh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2oiooftxi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2osuivqtv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2wwmhmgda.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2npxthwyp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ompekhqt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ufmduehr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzgsdgqf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mehqcart.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzbukrvh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2cuercbsd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kzaaxpxo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2yakirzkw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xntfinjq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovvlljxk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tilnruxb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2obbkmtip.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dhlnjiik.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nazspzoe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2iefmpmma.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qbkpxpwr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2yjrocozb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezwntgvi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wlaczcmp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wxmvouge.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bztrwolg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2rywxhawm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykufetry.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2irnfiblh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2iugkrnkr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ohjruacl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wsjrpwdm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aectvner.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2muijrdji.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wrzulauc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uhwfnopb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gkvwwigw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hhuxfrew.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gcoypsjp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zitbipph.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arkkcuxi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2llrpettw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ludztmbo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mzrflfkq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nfwtpisc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ficcpmah.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2umddonnk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2urqdxkqe.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bbsonrzj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtdcvcxk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2txxtozzs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xkebcqho.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xmnxqwih.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpwdaser.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qssgpbpq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2aperktod.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wuqylujh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uanmdtsn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uwtupljm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2plrcwyku.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqjjrnca.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2oxnwgguf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ypmtailq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2pemfufai.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zhkkywop.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yriezmpq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hnpwatwg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ngceants.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vloezwkv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zphvivta.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kndasvnz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qphnlteq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zyqhmaym.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qzrxrdho.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2oweeuanr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2mvjggdje.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bncmmmyd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2yfklnciw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nyrooydj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2recfdvzx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mhldgebx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlhiulhh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2spjwycaa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yhvtwprd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nnkbobdz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2bmwvvrjl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukreqyph.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ziwuirfw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ttkbsaxb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cgwwmuhv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jranzacz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lgqzmcgf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pfykdqlb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qeoqvoml.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2uriodunq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2grpmmfll.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bpcgqizh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gfrfvucb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lldeekui.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mlnmdyva.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2aqtvzmhx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2uzikupwi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwprpqzx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mehmnhzk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bkvgxtdf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2raozkawz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2apznople.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wmemhuix.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciixreki.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2emxznoje.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jjmpxjbk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2atgkvoqd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2culhbbjr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2makdmbyo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dvpdetiv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gvcvezww.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldcfsokl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jhghywpc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2snlyewnz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qfuldjha.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yiivyebj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rqekscft.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kxbknljx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zxvbldap.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2peenutvg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2xllgibbr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qbxaywju.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2raekmzjn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2skeyxiyu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2zgqhkqkb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jcdrxuue.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mwdkvibz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nheqdpcn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2oabikgjo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sjixkzat.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2aiujfpns.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sejoptem.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wwpauecl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkmxdaig.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2fsqogwrw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zwkjujvi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vwwufrbj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2cjdmdijb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2exvuyqbw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ksihuipb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2knewtgch.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2decxvndj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2edrgrjfd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2heyjjqco.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hrndvucu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2skkvuvee.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2htnzfhjk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2pjasescu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2djqaupmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jegvpvxt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2mzbvdacj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybnjxmfd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dyyhawtm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2iiwkyimi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bdaizckz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xucrskgd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2abwbbgqy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2aaihzlgi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dbduwegj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2sfgumkbo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2oobzdwdt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tqavqdce.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2otbmgyki.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vvbdiitm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpdjrmbu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvtocded.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lspgrqju.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2aptqfoha.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2poeamksu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtujghzy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xlnvhdzh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2efbegkzy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ktouhcxr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jjuabycu.html


<!-- 参考信息 -->