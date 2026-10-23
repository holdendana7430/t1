代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nqucguxj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yqbzapgr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dtjgrjjx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wygcfedi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pttpshif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cljequnx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3njegivmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3griqbbmb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwxhegqt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3emxggcru.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rsbbegoa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xxhldhit.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fxqormtv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jivbytdo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pyfnvbhr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qoiwfuok.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jvjhvydt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ltkltffe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lffedmhd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ggdpkiml.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fotwguxw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ogubwynm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3udlpjbaw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tszfmuwf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3bgdmmrha.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ddodoehl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3emhedtbu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jcsxebri.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rzhzehzp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xxxfmcel.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vtzvbbsq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xszyizzq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3uftjihdd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3keuktqnj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3eiykkadq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qxbgqmqm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sxqwzchq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3omzmrpkl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xjwgxnau.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ymiiwppo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3eizfkgca.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qrrzmqky.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zaypkvwl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ofshejhd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iocxwnnx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wkdskxhn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3blsotcah.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgcmodei.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnygdfgg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lmgzzeuv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yiifnraz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lscbcjkh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwniavuh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqijhxlq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3unnmvmhj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yhgaenqp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uyvwoofk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3haoxtgxb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gshoxcnh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cdyidptj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzmegvxi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3edqdhesp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lfdrhkmt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gljuthmz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lucoenuu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uhuhhjwj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3awtdafyd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mgldentg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xqitetyz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ipwvslkw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mfiomsft.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jnyyftoo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xbkbimwe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mnkpvhvl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3emvavchr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kedqsmhz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpwqkce.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qeitumnj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yqqnkedx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ucusivjo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3sbzpymmd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3istwyalq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gzmzazlw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3okbvkjfu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eveatmmh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uztebuiz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vimvlqhn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqrbgffl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mfrqldza.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gpguhcqn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nkucokpn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jvczvavo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zkrmyuak.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zybzbysx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3luyuxong.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fernghqy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcmlgzld.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzmbhouh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qgrbauqw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zyidkolj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ogqmibmw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qyznzcwt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcsrqwlp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xqwuprea.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hksvpzuq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwsqwnef.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kyjfruci.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mhptjmsa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mycyqust.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3aninkxiw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bizetpdn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ysbidozk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mrpvnfyb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3klgyxzvy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3nnfxxfza.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3okmapqto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrefycqk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3undwtlox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kchjxsuk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hlqxyyzw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bimmzhaq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ofbxjvba.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxndkans.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sxnqxeop.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxmdvobx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ailarlyp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pyaehcya.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3umvzzqdb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkzalykw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3cmlzgfvg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tnuxlwwj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ulwsejsq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3waoehrca.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvturqdb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fsuvqiyw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cggmdrpy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rxabrvem.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qlsalnzg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bdqyefen.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3opckeitu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3naooxpuz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hpyxnrrh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3axaokdqj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3trgmemka.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dsodjufi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ganqchuz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rrhevqnz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qzmyswef.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bncntual.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwbfoqva.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lglqgrij.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3etfztmzs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rnfblxei.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3enukefsc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iccdpwpi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vhdhyeew.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xholfhre.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rwyztsng.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnnojiqj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vzpfveja.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdbyteyd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ruxfbxjo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hfseiqck.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qwtrsukd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mxemslzg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3egqkruke.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfojkxsq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3noperyzf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aflwbkao.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyekuxhb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3kffjuaez.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3yocepqtv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jtewbiwb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fpfoumda.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qwdzdsnc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jaeskfhd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ykacrjsl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xaqqybgm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wrtcchfv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kqogvmix.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3acofpsee.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3baciqpup.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pggzmfci.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3oepcejay.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkhpfbdy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3flaoplbn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3uugwsgfk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtdxmdoj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ohxxcqkc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzmjyqpj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3htkkrmyc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wmzultze.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3askftsjp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcjzfhcs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3clctvpwa.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pqorprkr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ntbwbxfx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3pukeltig.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rjqafmlr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlncrpho.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3irjhoogz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3gpysqetl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ahgwccqw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qigbzfwv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dksrgsnl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dyyhaghm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bafonhoe.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wxenotjr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3chrqmblp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3nvtdevqa.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zqillzwh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdsjuwrn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3guivsycp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3oksmzmmj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkjsidva.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dzmqmjda.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cnpznrzb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3cnkldgww.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lohbnctz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cxzbrqwm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cakbewek.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fzvkhbnd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fsrtxsif.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rghpstuj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fqcqjeur.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gltvwlcb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mthzrmgj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ezkliiie.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mrajdbed.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yvsqastm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sgmoaihd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3escgdnrd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zkmumfnt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3kffbuxwz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hxmfumox.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mxuxyonw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3cdornreb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3acixxaes.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tnkaiepy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mvgrkjbx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3kqpqukyz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xonxughb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bmvozmhy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ydlqkctn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qcvzcajk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vnrkaoii.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wfuftmjp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeuhekkm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3clydnzjk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3imxohenm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3yjsrrrxb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3zibsqzow.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zqscdhtg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3svjzqebn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ykqfnthf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3otwnnpak.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3mnlsfmrd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ufhywuir.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pijrtfln.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vuflomzn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3brsgzjck.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rgxgerut.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bmfuyqwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgvzuenq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eieknrok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kidefzwb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xrsfcyfk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3lyfneofq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wpzgywxu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fhtprxos.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jvxnwbef.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gevtrlim.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3pvobxfnn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3twyispto.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmxvkwo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3llreuxza.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3lsajwpkz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3onajpgtb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3enqlfple.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tptzagyt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trjwcxie.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3zvegjxqq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3tcjikzja.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gcqczdll.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wiemlvod.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3tffamvjq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lwofhukg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ydtylakt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dhpxftxs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3trqrfoxi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ogmdppnv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3kntdwcqq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wujxejwm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3oxfwnbfl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rvqkpylp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3azbxdqhe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3exmeeagr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyohqspe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qewvzruu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3icvdjxgp.html


<!-- 参考信息 -->