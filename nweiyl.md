代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3abizizdu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3psheadei.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xhnyimby.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pgptcdbr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3umbzdjum.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ghxkaqqi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dcfzefro.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zlblomut.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gpwzdhii.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pfnykrtt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lwliuskx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mcikdjao.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xvmybqma.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fioayozz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tridadag.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3orslrdbo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pgdqbsda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgwtpgzs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qejwpyyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jucyyspy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzslawdt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gmfiteqp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zqxzxrph.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dhtdzyfd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3anetttyd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3anslrefs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kqpoyfei.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzektqad.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yitzygzk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gyvpnqcr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3llzuxrzx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3lxpmxady.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hnevfkue.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzvtyysw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uybrrizk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3aaprdkzl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ynyeoihm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yacxyjsj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3sflrgpkw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ytdztupa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3uqagaxdr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cqavvghu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qcmcxrkk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bicvrwov.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3darzddql.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3atntluot.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qdxjurtz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zmmjvkna.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lchaacfj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3iorcdixe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lksvrwrt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sujdbjyz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fowxjllh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zhexlwww.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3nfnivxul.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tqdcgpbo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lyipastt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hablbdsq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mwomhxow.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yanbeiym.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3helbqkhm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qlerlhlr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ggywcgjw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mpuvyfgm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npwhweug.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3kuhmmyco.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbwbqnta.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fraalasd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3spbentgo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yfohvxxf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gwckkzfm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynsvaakb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nrnkcgix.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nusdeqly.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3sisgqloy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ksolzdvj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bpknoblk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dzhyzzob.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ojvjurww.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ldwyoqzr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3milhiwez.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3apsvqpna.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vbrnahwz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ihsfyven.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3szmxnxwb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmmhfsty.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oqrtmbxs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kflbkgle.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nwmafnem.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pcdcfvio.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3grvhkflx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3yabzakxl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3cowrflvu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3romcjjwl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yzhyqrnp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jkjegibb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xmxmrvua.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cgaqdpyw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3anipnieu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbjencwz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wsucxrda.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ltqmdzpy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsxstefq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xbqitvea.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjvrihwx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivtavoig.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3eujxeuel.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lsfjwhfj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnabllzf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmytfkxv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgbiypcv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zaxkkpbc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lqezanof.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3opzymctg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ycjjuxpg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3canmqtpm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mfmrezzz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmsftfco.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vsnrommu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cslwjpcn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gjnyemqu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3urruqzxc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ruqkpted.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kffxlimf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bztvtcxr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xyizfvgz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fbovtesy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pwfzeqrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sahyesnh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hpxrtnvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3foyttyqj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3eozpnkhp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3sxwwagqd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jcnaiytz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ufpzumvz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gnruxyly.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3varvkpgo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3egvejqqp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3twjfhcfg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahroriju.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yropwjwc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3foqnplwa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vwgctkrs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3slqbzncw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyakqnic.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fpabufey.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3grzxvxom.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjzglegj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ixepyqwj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qccukauq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3itupmcoa.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3deoltycd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3desdzime.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ldgyavvn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jslktubj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fqwlyjam.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mcztwzvj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3whdgwhzx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rxpyfcfr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mtvfroxo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uhpqyydt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nitswgtw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oglsmlnh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itgiliyz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yjwtkcmh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xpzosgee.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cxonmnlt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pgruxdix.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3awkvqkft.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jsptdoki.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dbqgteol.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ikmfzpog.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhtmmtnj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ixluqatv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vaamenxx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mihytdvq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rojmrzyt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jvvvuanl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqxhnaum.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiwllbwc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfqcvice.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpdnfvqs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bhfnonqd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tkxkpamv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ejaigbar.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bmmvqnde.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vefrejlo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pjqqmuxj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gcgdkagj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bcrvdpmk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qgtrhwtz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3sgboqsxm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gfyjlabb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3izohdxbr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jgnkghfe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vuuniymm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3izoigucf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjiabvnt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vcyggdll.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbaclfcn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cwrzhkvr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ixfbewrq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3oemixvey.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mdiqsygm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ezjvlldn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wljfcege.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3pznxaxik.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jyzlrmyq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fszdfqwg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3netopqtn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gjcdouaj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fjcxmtcs.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fadeyfuh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fwkzodxd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zozpziov.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3aimjmddz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tmeljwlx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3enimehao.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3eupyluic.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qlgazwqc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fvhbrpqn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ungrebll.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3yykxesbx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rndfooij.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3krayhsnv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hfxjmlyi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cbpbnpsj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sgpkyfzy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tilwzwpx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnlcjias.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3irfjuvgm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3veilwlcu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzanpadb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3myxaozzg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lnsstdux.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywyhdpoz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ciewdkaj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qntbifrh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zliuqdyy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3epqxhljz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ctndxwtt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xeagqwuo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3urmlkelk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rpcsldcn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sdcigrzu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tbueviwp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kxawaezv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3zdmbatmv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3kikcmdvi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yuwomimd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vseosvad.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yaaykyka.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3agqufgdi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wawjdicb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3lybdrvfi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3lohsvjke.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3sraenabm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gxwhgrvq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wnnihehk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3tkqluhdl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vgutgmkj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xoqaqsfs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3oefpcitk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dtajrddj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pbbrjqdh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ehewgiat.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wwhebdvl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ieegxtwq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cghohztq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cenbcfom.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3enunewtg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vzlvibvt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ulypecee.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hhjqncgy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3umartuhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfpzmmso.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qwleizae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfbphuzd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3znkdqxii.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cbbupvad.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tajkjlbp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkmzwitu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ixvhyppy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3brfivzfa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xcvkkuzk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jeruzuab.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmwmxzgq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3arvxusvd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ewzmpjbn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3habmdxwa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3osqzvhng.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wglffdby.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fnownyny.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xaaevyvd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ksvodjwh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qjzmbqeu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3etcclczz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xbjvpyfv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mvzgivmp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ykmnhdhx.html


<!-- 参考信息 -->