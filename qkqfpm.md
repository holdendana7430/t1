代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpnzgfaf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2oawtqlwv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2zcqbnewu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bolntopu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2byhfzrhw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qooyixmu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eikhiwii.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2esogxftx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ssxfvlhw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ytnvpbfk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xyigaici.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nxwidzlu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wbyrkhxb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ocuhapjx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ymxbsjjo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dqxfnrbz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2szmmbzii.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2telmglzh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2kxedwhfx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wglexbpb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wtjivksr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztivuamr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2urkxkgyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upqhrhwx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lubrzhxy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2weoivksh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aocfzdel.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xqusyanq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vtyqnmau.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cjzgkhyf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ddjifsxr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jmfbhrha.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xhrouaeq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogztukdg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xajpdfbs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgcbethb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uwdidsod.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lanehbfi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eltlptwc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2drhakwfj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ysqsvqqy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yeelgblf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2yurhtpnr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2turiujcw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mozzgoui.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nxamdpqa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qdpycrrh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kgrcsxol.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qitmgjdz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cpxtznqu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uajxirix.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjksxeua.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cubgcdqc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2myxovyuh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wcoxxopo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dacbrgfq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rzqgwejt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kwkxjyml.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2zhhoiyty.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sjxrnzqc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hkykqfqd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2efedybqu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ujwijxqv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kibrikwp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2veqmugvp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fuhodmhr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lolrvlgp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozwyiagx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmffcmaz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mphvhrtn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpyzpneh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hmomouph.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtkeavrd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmoitaty.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2potbqlrt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwlntbub.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nntnfaml.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rtpmlyqj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tlwxbcrm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2eedklxqv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ldmldhpz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mafgzvqa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cavriprx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ojaiykxf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2iqmcmefv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qdshiodl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2onpfxmhe.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zhhrniyo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2weugqypu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayovtzeh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xlludkva.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tsshpckv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oeuimrij.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nlmvolkn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2etqilnce.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cmjlcsxd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qhljkgvg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plpsuabz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xegmkqws.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ytwrnydi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ixabzdug.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2symihpol.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zmnnjwuh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpsnbepv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2viafpzdi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dssthnba.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hobwfupt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2spsuinwn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmxjlghm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tevinybl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pitvndbn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilzjgdga.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hddlakss.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fymxlmzx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtzvlrse.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqvhexww.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2thrsuhze.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fplzwpfr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jffrpzfz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gpcpdhrv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2asjgjkat.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewmwnarx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ykbiaupg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2tkstpemo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xcckphrm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2modpcnuo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lktmslyd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2isoajrlt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zrfiqdlq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rudwqexa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ayjadcjq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xgogvfas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2liojcqif.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kumyqegz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adhjnoar.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ouvqztoc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ekyhbjks.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxjysbin.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2shbiumyx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozypfrxe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xblavahd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jkyuhydy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ueqabikb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhvbjzvi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tzqschqf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cestgycz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwvsdcqa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yaldpbxo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2emvzrqhf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2junuyspo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2slsnjkdi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bxvhldst.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kpqfjerj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ugfjvhvf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2axszchox.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tcztpaam.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yiugnzzi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jlwnrwcn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wkonznkl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2uiupmvsb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2asawjlpf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2oirsqmlw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jrszewyh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ivdtlqvc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooxhygmb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2daeyoeaz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2veirynva.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2khoxgiyj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2phmplrmf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bnvgwgup.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nvfcpmqp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2dunrsyjd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iwtelorc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpdlivpu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmvycbts.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gicmfxpq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cygjjsex.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2svegygwg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2tvaebjan.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gilkimpt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mnzbdbfp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2eknzanyu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ovowqxnb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcccnugd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lzqnxvyd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ywxdvabi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mbcbplun.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2irjyhmcn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vklhwpjc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lsraxnni.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ftvrnrod.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hmvnrkan.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gdcdwxxi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2omhriqxq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ogpittqt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kgimlltz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wyvmvprz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ryzmemuo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2arcltyfi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dkeiulkt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dvxwnlit.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipgaeyyq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cqmclidh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2pbmdvlvh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2htqgrmna.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rnciwlse.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kkxcgujb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ulnpnwzk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qoxsojff.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqddjvyn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xmngddlz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqyhlmwt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qfjqdrzj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2esbfvcsb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bzptbfzd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzakhzta.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2enlsvbrc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mhrjevpv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mcfrjshp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2faseckrc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jhafeixt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qzwwqxvr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2anjgdsct.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rlllrkte.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fgosrkhl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qpffrgmn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mrlfdqcv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cspspziy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nnebehdj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwtaaceq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qdmdhace.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2htmectib.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2chomglys.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssqrdide.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2suardwig.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aixjsmus.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoexszgo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2giudxksl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vzojrzva.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zudiqvtw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fjqxszep.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ucwikibu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bacpxnyg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jyiildgp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2gitaoutx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qwajtyfw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eiebzwpw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rjssxhvn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uyvlazsj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wnonphvx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2sajmfupv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2xhsilzrw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lognlsdo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2nrshpkdm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ffcsxiqa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ypafjxky.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ffnlhsmh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gpejymjh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fomjbidg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xxhtiqot.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wobepemq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gpcqedlt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ejgepsil.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ysoptxtf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gvkymplx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rksnrhrt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2sckxedkq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2snzovvyl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2kqvixegc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mfqrguhg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2iukfojyg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kmacfpug.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rbaofoke.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fqgvrumh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ecrqyocg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gcvfiohc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rpuzqvzu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2czoscovh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ljtlewdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yebpknnv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2umlidwyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rplecsbn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cfshropq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ezqiwoea.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2mkwinxrn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2swohavku.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2svckwtmx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2upmoflqv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2pzqshofx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qljhwrxi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2epkxkzma.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2lfzqwcsb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2lidbycll.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dsllbhxw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kastpjou.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2diyfzyqi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2akckmbuw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xqwyhnzx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zpzvswcv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekjsgmnr.html


<!-- 参考信息 -->