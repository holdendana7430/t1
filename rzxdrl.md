代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3anpvfixr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3auasxxle.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nmeduifi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nmjsexsq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ximbwmll.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qhzhtzkh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kqovfwba.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yaurzbas.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yxrotwns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aeltcxqb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3uuxpkihe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klfxeaso.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3awutoebl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3shtrzhwx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idzkumey.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fylmpfwy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lygqrdcz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cbmxzdqq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fqpaoswd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogggecos.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3geutbkeg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3teeqmnrm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3uqrdjuvn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uszevltg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzeqmewr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdfixqyd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kwvhrkhr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ldldrfox.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3bqgqroxf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fytqkprp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ueyktyhi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hhkrhpma.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zwotpcnk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xvwzfdik.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pexmznma.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fwidevfv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3phpyvdef.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3caevknug.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iblasabp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bpsxoegh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wscfrppr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3boyveamy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3recjhjua.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pnnbblnf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jpzndyse.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3whsfqhyd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ryxthkui.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zgkagkiq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rejlqyts.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mxwyswjb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cynbvutx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atjpfenx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eijgxydl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oynancje.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hrygvzjs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hatplkma.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqjhncso.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbosktrh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ontsalcf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ujoejalm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mefbxnte.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3skhitbbx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3etpvkdtv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3euspvkqa.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swgzfujl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rlmlwzna.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dciynyrd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tsdzwebn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vuxjhlkn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dwwvjckq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rvijmfpd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3upxvgkeo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3igqrdwue.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3njttptjn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bvnkdtyq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fhxkdgrx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gudyqjzn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mevylkvt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xmcrxcwv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bgltstra.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3swumempf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3sahuqqqg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3mctgzral.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3olutixyl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ugveixek.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mghcnbhb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bhmlupyv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hxjccasc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xqtpuaix.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3crdeimzl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qzgxjlvq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jojcnfqx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qdryczni.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3cqaucpev.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvirstzt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fjnrseyw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aoqskdew.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qoymdwve.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kvvblcur.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmwkidfy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3msrxuaqh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwumnflb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tppuufmz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fztrbwds.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iywdthxy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwkwngre.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxbjtljj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wjagavem.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xoejpkmb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppxxdrhk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ymuwzkjv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3morivfsj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3suxpkpbz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3etaolyhu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xjtvpjpe.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3esoyggou.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wqssnvyi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3obzrvkiv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zdjpawsn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3qcmtnjcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuezvoay.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3uzfufply.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mliwiknv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3glcuveyl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dnalkmqs.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pacwgtgw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycstxxrp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzzpudyw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezibyscm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3okupdjfc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bltxhjpg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oxdztmgo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3iscpgizi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jnjviyto.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ejalekdf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzteuqio.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxvkzuif.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cmzruryx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wagwowhq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dbupmlrg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgkdfnwu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hxxcipvz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xawwjlrq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dnyrsamd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nmfkgpmv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zznmkrxs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rxegoafb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mtkvhjkm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ukvajaqk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3amoulssh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3quymcqjx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zrfoneff.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebwtjxrx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqlkbqvy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjjrynbf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjudsjgn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lxhrdkul.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pysssura.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lhhjrzrr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ydhxoyxq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yhcolojh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yqrtafii.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqxqsdof.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3emfkzclf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjmehjub.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3sdqootmi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3uoufijsy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjrtpwjb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3inpwigpd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3palrvila.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rnsihzfo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qujfphax.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqmaeysg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyajpyse.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bxebkvzx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3eqdykptl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3bwivbsru.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3extotpor.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3cyzhxdca.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mcarlemn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kqukkxsx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3exezgoty.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3svyegqwq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vczdgdxs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vwpikexm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3trktjznm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xjfysgfk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kvdvtqoz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fuoibcoo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3adnfvyrl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cfvjlcvc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qofjalfh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qesypufp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3eayrzjos.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zhbzijes.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qwppmpoq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pqqwoehd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhtrcsam.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qwpsrrmn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgcsohqg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3riabjdol.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fqalfisk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xchllmia.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ocipvfhq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3oocmbutp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fcgvycnl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qxgluytn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jkqjdxkv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nirfopan.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3edayhtsn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zupljgex.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dorudmog.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3pzgknkzr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3wpdnvylx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qqzmflyv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gnadvicz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyhayhbe.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xikpkndh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpoqrzvn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bukdinjx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xsemtmew.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kgmaokdz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dhcnbwyw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nprfnqgm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvmoiway.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtoznszo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ucxvnlua.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3exopdhqr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iedeqgae.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jcxxmahc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pvvtrjvi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3lsabjplw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3pibbasgw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oflshhzf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oawjomgi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hhkaoieh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dvdpervi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3olbefgms.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ioqnkoqu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ugcksgex.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xrdakggi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rrfavczq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rpgmdjbr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rfpvxqkp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ifbewdhb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtfredkf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3txkyrbme.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3frqpbzrt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3niwilqmt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fhpaipwg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qouglcbn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ssqqtpic.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3kuhaglku.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bfvzofwj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3davlhvck.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3fccqepgm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mvperbib.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oloibsqw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qgjjnvda.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zaidlsov.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wavhqwrr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3eixomtnw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zhfyqrdv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3aosjjsqi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3whlgfwxy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jeolmpyh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vgevlkdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3robuuloq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xzyujilt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvjzkvrv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jufvjamt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zqgteeyg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uebihxco.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hvtqlhtp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tuiwkmgz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdeobxip.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gqcrxabf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zzptyfmc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqbsmmws.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ihnrokqx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3rjktnsic.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kyxvlepz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vdijbkzv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhrqzpii.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdemjnga.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3fyvrjfeq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3odevdusm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tecesytw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uviojwpa.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3pdfslhqj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xlckohyu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sznzkkan.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zmoqmczb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vtmdoxwj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3icnnqrho.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3odmyorei.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lhsokwmv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3tldbhkqe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rftedjby.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ahnswdld.html


<!-- 参考信息 -->