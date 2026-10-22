代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2igzkcnqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xazzqofp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xjuvfpof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okkwisgt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zzsfbwqf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2htjvdzzm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vljjpaqs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hlorsapz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yrnxervp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xoucacoj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cjjzlmat.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewjpbrdn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bfvlnssq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cqogpwaj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zmoltcuc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqyjwggh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sospqeja.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mzojhlla.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ikxgusih.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kptwelqc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2sfbmvari.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpqkqpyv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2clhtlmot.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kuqgjsuw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2isxobske.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oslvtkmh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rcnxjjjw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2josvpakw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ueiovgtk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gdbvjhyo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dagwwxse.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xjwngjxi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2klmrigfg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hilckrya.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jkqlkdra.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2enovnwcg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvecvrm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ffvkaiqc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cmgmmipj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lexxkosw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vizpocsv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rgyhyppe.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lskhybca.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpytivel.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yitnrtdc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mqkvaubb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lmignukx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zrkafytu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lotxvrlz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lzowafcq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shdqaaex.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nacvfpec.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2niumzgjo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chwhjvks.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gqslwzap.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgaqtpmv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asddepfu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kfuxzuky.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pwmygvdo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yzodcljc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2chigxiwp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lnkbdker.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qakmaujd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mzebguie.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rubxoocv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kjaynekp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2afmubiba.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2urpewndv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zvhsgpms.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2crrfwfvj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hhetzhjh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hjyfovlg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gmwqkzrj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mvngquuz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tduvyroq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ixktpnxq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cnhovlvw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vudznuai.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nvaxhzsz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lualbact.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yccumgmu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2emwrteww.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2yizwdtql.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ccddwqay.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lmgqulpk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2alfleoei.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxrsnibc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vjjrqppl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqjxlwbx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iigfmreh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jldlsqas.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2minbkqzb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fhgcbqqu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ppkbcipn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2itzkunxy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufnqzkmr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fcmrbzzm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jkjpslpo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2anavgfys.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2flzttjds.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bavylmdr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtuhdaku.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2epbjzdgs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qrzhoxat.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fzhevtnh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pdtksmfx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2bdmwjsym.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jiodvgnw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gpjqfypi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xnddamsg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mbfzrtcz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hjauiscf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wovcphin.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2enycqscl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anjrzxsj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rkzyzsrt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fufasivn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2iibrmbhu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvlnvqzl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2adaypqii.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2yjfdmszl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2zazqvjyh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dvrsarmq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uakewsuq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ihylahlk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2dqvhykae.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2tyclqeeq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kjzqjuzp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smxdnhrx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rgahergk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2extidjnw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kkbhwfzf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgwirpco.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xtilpqza.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ndgngunh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nscdtpsa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2faspmxut.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vjeaatsl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2neeurjzi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wfaojwzi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uwudsbdz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yraalqmd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2cqhfdomy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jkcuktam.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rralcija.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oneumrfk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pueicona.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtpspict.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2csqtitqg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2laeblyok.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jpwiyhrj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2capubiqq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bvwixstg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lvmrqpaw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wdupvfyv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oqwohzer.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtchebmf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xtambwww.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ptooawrz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2htunemsa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2atrhzedj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wvdrunmo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhbxwqxo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mkfmcmkv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fizqusfu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2msuotahq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xmhxzvtb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ozvvhymt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zxmgjtau.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nmzpgwdx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gbycofhg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2aacatbgo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2coqwqxiq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zwajobip.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wlzqzsix.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mhjcoysa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2pytskfpt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pfuljohv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2sjxwobze.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jdbfytxw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2axuyxlah.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwnyqsfn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cbzaszgd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2umqilksl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rkgbvukb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2tuuxpmdd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qaivwkef.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2uhgiwsxv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2adzngfkz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2tumjbnmm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vvrogtux.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfufkpub.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2swunasau.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2edzkrscf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2umldtrtg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwvcbcpw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2itlivswv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2toyogwgr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mxpxlbxq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2liqnliet.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xqxejcho.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2oipthxbv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hdqhwibm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rerxbhdj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2siuqenjt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2krdzvgyw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tulzwyxf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zjzfzzrq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdxqpzea.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xmhhinjy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eduufagd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ilqfxkfk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2dpuqvyse.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubuqsefg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wcmbtini.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lrhgzxjj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2shuaxmkn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mwybtxxx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zvpgjyli.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skckwtfh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xoalwtol.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yafkbbju.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nboogcfe.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hjasyphx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2uvjacqpz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zsheoadq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2stopelcm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zobxwzhs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2counrvqa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2uehimact.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2jqmubled.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lodqtltd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rjpziatf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zyfjgiaq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ckhqfwuy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ereoqwhi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2saadtfng.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2iklglwpz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lsztnyzh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zskcakaa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xvxaaiih.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pdfwrggb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2yfhavyvy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtsdimkp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2obotczmo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kxgzptsq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2unxkgukg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gwkcuhep.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bcotnkqh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2meqyimvk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ghuijxpl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2khdmayah.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2foniiayf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kjmyuygt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lvtriagc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dgicnyfl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2purmixqv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ndeejeke.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vuhczfaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csetpjkf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ultbaahq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhaghlkp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xjgtpker.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2alnvamss.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2oimzhoer.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbvtfgbc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hivikvdh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ezjyhxcl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ytniaeer.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ycvoucqu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mvptcxbj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zrlxddfm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zfunkotk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zpmvjztq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hixlszwj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2andgqdrg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvxvzzzd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mduqsvwb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrmmfyzm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wezijiaw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jgdlvpyi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2caxjzswv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nkfccgnj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zgxhmasq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nogxrxlm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bgeadmeb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lzvfnakh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2mebumqtp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zggjdulp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fwlshhpd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zlqgxmdf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wjipyptc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xfshxlly.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtjuamsz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2trmgnspv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ftutvsdm.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gnozdtye.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2warbaydr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2uyzkkdae.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zpceymdo.html


<!-- 参考信息 -->