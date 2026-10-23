代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mdlxrorr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3prhfvkcl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gimqvcvm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vygvvxji.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gewcmxvs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pmlvvjuc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kaetknzd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dhwvxdpz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sqkkxsgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysjhsmlt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yhpmsqya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayrbrkyo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgdetpzb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3imzrqfnb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tbwzujro.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3crbctmfu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qosnrzmd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3drvbxxxf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3lqclvhfw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kbcionzp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hwpriglj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nrkleelz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jazuvxko.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kakxehdb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3drlwknkg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxirspfp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3twbjlend.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qjnpfkvm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3fiouhqgi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3eaqdqhaa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ofxlwkiy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ezwqmxib.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3johyomgu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3izbphocb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ukdzyjyh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eojbclqv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ofnaqwvl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3llybvafv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3umijtadk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3eosnypen.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iyffmcpk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3lqbknnqe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3muxcsecn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fmwsmdkd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iavlhwhb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dayntrpf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nnapupso.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jiprfyzq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hsmcxvlj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rsvsqlft.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hluhiyih.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jirqyaps.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjptjgjq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dthdoxrc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qnohdosj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxezysyc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzwgrely.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3frnuxrex.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbzlouav.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bjxrpofr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ssoekfct.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsxfgamb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zuzeions.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wnbhwhka.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wbzgcxyr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lmroifwm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3yffsudkz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mjqkkscv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lwwbqutr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rbljssly.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pflkuscd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3afcvaujc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rggmnkrh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tuluouwl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ikcrkvxp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gonnvvvl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ybnuhtmx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fauwphna.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ghmsjtyq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3varxbcvc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3iwdbnoae.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hmwdoeqf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mcgudehz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wrhirtec.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sstgexsb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eoztpurj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xpmlfihn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qdmdvffb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kzmvornk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ownozhxn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3uqatebdl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgwsanet.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xjsuizrr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3tquxsffe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvvocwki.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sgfmzale.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3urphpbaz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ignhdwkz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vwaywmlm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzoddmjw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbqzlrqy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lovdmqws.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3werbvwzk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqnpklhn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3mvfhaxwx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwbgebzc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvtrlsrh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3iuoaffbs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zfehngyc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zitmvjfk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3oiatvzcn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3tsdqlwcm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fjeckcwc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vzjfafna.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wgloilzy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mpvlmtha.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tbmontmq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gywhogdc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xqsnzzju.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3yfgrfpwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxdayhfz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hfywsiyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtnblhtt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fxvbbqjj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3awloggro.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3tziynjcy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hktaveqk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vamoearo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqjbsljf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3cswmecgj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lnreinjf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kptgkqyc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwodtimn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3svlnhtek.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ugxpeloo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iyjlkaal.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsjlftgh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfyuddrv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3phvnulmc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jehhltxf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wederjiw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3upfjqejj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qicmfwhh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3muvnwhtz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fsdvxrtu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zbisgyko.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hujbqzja.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xqggduob.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nthsvnlz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bqxdmpan.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vqmhczlx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3erytfyvd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kdmwfsxh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lazdesoz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtbhkjls.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mgrscoyo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tucralfk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zdpbqycv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ysuzwcit.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3disojitx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qpoqhydf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxsbwynu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uddemsbl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3arimmpbw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbtavuco.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ozabkgmc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzfiuiwa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3iyphczpg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3aqupfkap.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qbwgrcdo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3acjpsmht.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfyqjpbe.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lyvkkxiz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlfkxqmh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3einxjzse.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3azgeovny.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3emfypeyc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qrkmvqkz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3uadmmiej.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vefuqzbw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dshrzjws.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sfcpijbe.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gmfsbjod.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bzrvfjyd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3tysiveiq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cntemdgl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ztegxnmq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fbgwriug.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fpaszihy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ghugmloh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3otnwmiri.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lioihdyw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3folldbne.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3wxagvgjj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdwcdfch.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wnjzsxbb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dyrzxosv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3oacqvvay.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3epivazyt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3utljgnss.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hqzdwizk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fitoxiwy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3mhlnpbfd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uczqedcx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cdcjfxvf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3keuoxmbe.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bbdaulis.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kvbfiiqw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xkezxsaw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ackxqaht.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xyfahetc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zffyxsqt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pjsfcvbt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gtpzfgfh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3sslesnqe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phxlsiqj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wibdweqp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kcuxiwon.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohgiskup.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sesnemjo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3katwyusk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfckdyyr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3caeqxneh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3svjfsbvg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3osrexnvj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qksvbzkz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfyxbnyd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bazzjugj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xqnhvizd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fxiexcod.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oakonnpi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rshbznol.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fsggbncv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qdvunlzt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bhqonkbg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aazultma.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3opivutev.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3enucwdic.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xuvmevix.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zalxfsgv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vgoaxtvn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3sxyqynqm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3cwcviilv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vgsohytj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bwokcgpn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbutsjko.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3omyyxwfb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ipbwclfn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rfcfgxcm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3crfonoqt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mspozuxt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rymhygvc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3xliikyii.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pnjiiavx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lqdjmelc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ioylzxpz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gzclrdgd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3agxmmjvb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3untydiqe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3bjtbuvyd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3reyympye.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3eebpomko.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bkwwpjzm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dvgqqbdt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3uihpzoyp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3fxpqoalf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3oilvwqno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmavdwfi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3lyvgvjjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suguchzy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qgitdtjo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3daumlqhu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aiaykbdv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3aftytlza.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhgyvhfd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuxtisbr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tsydvixq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3yuigomtz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3bxqhuduh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3opqanrhf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ayxsltfb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbrgwytd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zonckbkb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekrvvqrg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eqcfjppn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3icqyluib.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ghauxbbq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkqtvhvd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vepdzvzg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3viikdnev.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rqulomea.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tqvvdsvd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wzhnmqdo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rxuygmrd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bffcuiio.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xypaftvt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mtszvhof.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rofctimv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fpphjvga.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfmgrgba.html


<!-- 参考信息 -->