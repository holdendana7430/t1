代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nldfcvxc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2falfwrvh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qrxlmgpl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uybzfsgb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ucaobole.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wubwtulm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2znqfpltr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2niirozmf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aekpauwm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bxlodzqv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hbcyydqp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ncnntzhh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vbftemih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gorrcvnf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vukkjfuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujxldnbf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xfbfnclp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2txjwugoq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rxlgscic.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2tbonjufu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ewsrgkga.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zytolkfr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2axrcgxnk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owmvznxj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aeuuxcqx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtjaqlys.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qcciayxm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vvrmorev.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2otzkqttj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cshpxmjf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2myujsntu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kkfqjbfu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2lrmxllik.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmukgzhk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dxrlcnug.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nkpzdfrb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2stsdsitu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cytrietv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kuuqychx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2eaizhfjc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2mwwdfwmm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zwwoehpj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hlxiakqc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2oinqsoxw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kzxclwoa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wmvarvdh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ofrgzjjh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pfnorlzz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wvpidqhz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ksbesprn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lmocvdjr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2utpsbbmu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2cwibukcl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2tfliiziz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ukjxwrgg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oigftnqy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjuxkhev.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mbtryaso.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ftegalpk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzyitgft.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bcaykdfk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2vjlfvvyl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kagyztvw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jeutgfbq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsntcsvh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2huixxkaw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rnslnyiv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2izypoizg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsbbgqpj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jsijkflj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rxaspouc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dwosscph.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rxhspgff.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ybaharsg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wldmkowk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2esmebpnd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2fadcpiit.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ebzjcqvg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wfevjyqh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2dhbdiwqv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cwgfrtqx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zvjpxmzp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xualqwml.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fnmnvyjt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2abpqtlzb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lpswnlul.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qnfbdoum.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pqgdojws.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dvgegkri.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nasgxiux.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ofdckkln.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wsiidklu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2eamolwxs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nicnokcs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2izqczbld.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2acnrtvxa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xxqmvpxh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wjatejrz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abmrfmui.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vmbziseu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjkcbmao.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hoztqyvg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2abkovseu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ictpkdyk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obovapzc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbqwlfwk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2colvzbzg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmiyxaie.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hbvhwhja.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2heltvwlu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hdsnguzj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2egwicigu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xbhhyzvc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvctfwry.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lgbbwlbz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zagutbrb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ziovezfc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qdidyftg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2huwnzayi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2mzfnppoj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2sacmypxc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mfomzdxc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fhlercbr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uifmaaiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgxcxtoc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kizxfkba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlanlian.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2plmeiayw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2aokoqyax.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdtgqwph.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sygeakwa.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2stvexrpp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhmdeaev.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lcoryocu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2twznnqyb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypizwcbv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kvaehnja.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zfdopzzy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2swimdtqn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avckzvtq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nqoemghx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2djepwebr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gbjxsegu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2akoeaiiv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgbcwqor.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zwfrhkjd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rumzobkh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rhrtjaur.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ebacauxr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ozsiavdv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2uhocrdbb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2embfoosu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lzafngyg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rutgosnp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2eiuowlik.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vmevvfsc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ypmjkryj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ksxobbfi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2clvkjcdd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gbtmubzz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pokyzmnt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lnqvdyaj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bihrtjvf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jnsnxxkx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mtbcxcsv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxrhddym.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bymcqorh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttoftoqh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vzpctrjr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vunvmmky.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2sfxobcsf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqbaqjoc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pzuocrij.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2osdvdjus.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiuypbdx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jraicttf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mooxhoqy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oastuotn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kiosqhkp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mnwpewzd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kdfavmli.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nkgsxnzm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hcstnpkc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2omtqpkeh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gjfrmxch.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rfbuwovq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ovfmexwl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qlffzbsk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lsqdswhm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hanlglhh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jskfiumh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xiprugwm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dehwmedm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jdlneqzc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lckavzay.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lizgtmpc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2piptroyz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zjkoxrcl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2orhzycgx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qutlmgxw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2enqloezc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2snigdldh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nznxadhw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkrwzsbe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lmvvolyh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nhcmixkt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fgukeszk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2acixsvhh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2dvvqjnsl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uddhkgds.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2duortqaf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2uvisvybe.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2juarteqn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lxsslvmy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mqsthzeg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rkpaxmgi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fpdhrglv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2iitwmcgb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qolqanmu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2infromyu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpubeola.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lahlvisu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wobhkruh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bqawvjac.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mtpohluu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ddfmbpps.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cbmoedrq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wtkmouws.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2biycakqp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oogmmlkl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dpnccdkn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwckewvt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xjgxwhpx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oajcwdfc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vjsooptd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wncxhnjt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2flemfxia.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bbgqnjcf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cagfqnlu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vaynusrz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tupedjun.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xhjcstfv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yliefsdd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lwpfpolh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rfjxbmzq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2taewxlvb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2rqkgiket.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2rgsqvwqc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vcjyostr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swpllhkg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fyjsxgxu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rdfbposw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bthkipwl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nlgklqzm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vhwxjjui.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwmophqa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dcbhvrhc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xxzkaomp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vcdydpbh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2zfmkyown.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mbhqckst.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yaqlwxjp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qtknkuns.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2boiyutfo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nvtiaues.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lzmqumei.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jkghjkbu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jbyimoln.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mqdsnaos.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2actsjprq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2skxyqpvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upgoibse.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zllasmsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjqqzvpx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2srretmst.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2awaxyuui.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jltmxpst.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgajcmct.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ahrswhuk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2spbykieg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mnvqndkq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2iawshywc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2wviezeoq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2yzwdnips.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2clbnhqhx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jubyxmcm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfflpixe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sturmlpl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rvjssfsq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zsnoqruv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qtswitir.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2arhnkzya.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fnarkjbr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lffdqdow.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ooyvbvde.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2alnuwwrn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ttaeqfdk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2arjddyrv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2yfxhhrvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qbwpuzzc.html


<!-- 参考信息 -->