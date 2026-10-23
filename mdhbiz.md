代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmtwvgcf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cavxgrdv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3scbsfkxz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hudcebbh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yivoqgbw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ulfibsvs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3frjiyizt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkmivmoy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sepxfcag.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ssggijsm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gafxjpww.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjyuigtp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdesfvsm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzlhuhju.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ujkwzsxa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bhnnlbuk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3sqkuagsl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lyzpdqzh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bilhujrb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3diglppaj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hurtxcwu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3omoswdel.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ulpvriap.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hvegwxiy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kryxdfhi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rakmkhkn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3inlrvhng.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kaklqnvf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ozmrzzcp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uvorfljr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ztkusrdd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lwvjhhnk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fwrlrvoe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hrstdecv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3acnkxbxb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3akpwwaky.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ixtlifrg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cfboecot.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dmksaugp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snncdser.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aiomvsev.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xxnesfab.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mzcqdauo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aifsgnll.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbrgzlfm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3pmhqppor.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orqxrisl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hgokomml.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udhsyeil.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3madugnxv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ravxuhyk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mgdtdvhq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eartobug.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lyoghiei.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ifjsfhld.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rwxsouyj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sprufagy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rwhayhny.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zmdgwdbv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3cvjenivd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nrmyorev.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hehpkazp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ykuwooxc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vtkbfigd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3optjqors.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcwshkae.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3elyygrhv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qzhgquzr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3baurzrgq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nosrgcha.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3fatvcltq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rrzlmojw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tzcsrdlg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hyniwlzv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lejtqktd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3msgbuqlc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uyqubibr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vusvyxqh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3eaqwkxzc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfkeqdvw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3iybuuygk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3clxbpjmi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwnkhewo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uxrgwsnp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbzwltdb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyfxuzez.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3lngujtah.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahqngaev.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvlmlwsg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bajzzdxr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3snmzuaym.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztpqmfou.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3llwmsbaa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gimuesfl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlmflkio.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3enrvsoex.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3puwezeub.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3snbokcec.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3sawhzffk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pbsqlxua.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qstfwsyj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xebxyerc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qjasmbcw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3cxsukajf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3swgkzyjz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xnuxmaub.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qwikuukt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mnqpptgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyfbwcsj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jpyfttah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwmtekqb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zvtbbmgq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3yjexnvqs.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3gysghuhq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oycrvzfx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzglpwoq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qbmmxstj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3kcdjqnqo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hoguundo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qxwqawnd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wnuuunxm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3yibqsqlo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qarfxejx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhkcwhbz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zfvchrre.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eynmeaos.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3fglkwbcz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mmnrojtg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3chxcjqkg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fzewfsij.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3furkjxrx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rdbfaybd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pktsadrg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nzhzbach.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rezitvby.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3udrbapar.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3znlqlizv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ybdladgl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3nqbqhpgt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gfspinps.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgyuybae.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvbsepnr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xqhxhdiw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3meiuxagv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iogizzps.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fmelppqy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3noynlnpu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zlfnlthf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3igopjqul.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dckrthhy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gopkfwin.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntempfhs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xeqtedcd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3svoyansh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wccugqkb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3renwvpmp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kdmyqusq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3mstvppct.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbaowuiz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkcjjddd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfogcdjz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drcyvexb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nghshgex.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ympoytur.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wacsnhwt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wkmqmxyh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ghsmgoie.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jskovfwp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rrmflbit.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uaaisacu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pqvudrcx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ghzsuvma.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xvfsxbak.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3njdkvfak.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wrqdaihb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3eiwsqmdt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdrzoovl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3glxdersz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3soffbnju.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocmnphds.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3chkizbpz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ofamwrjc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yffaekia.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nqawitvv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3auyagkyx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3itbkvwrk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3dwcpbkkw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dkvmetga.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wessrfqf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jjyvemyq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3arktubrl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mqvzqtau.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xcazpiob.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zrrkwfxu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lninlvgk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3bsmhqiot.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zscdnkws.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hjswvxjv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vmebkdbx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hwwgrxjo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fxcdvyul.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kllraejs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oeddolmo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqsqjltt.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qvdlcxck.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3olsyqqvg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrxpydnr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wxqeshnd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3eknwpakl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3nxefehky.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jlcgtiqf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ntxckqio.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtmdgeyg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3whxencgg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bosmuojt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqzkkxac.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3elpuwjfu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3abdkvpzh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3blwnwvuj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bgvrpmhr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3yfjuwdwj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xjyufnhg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ggwjgpst.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jfesvlyt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mijulgac.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dsvhskcx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ybtjqdou.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3upkjvibh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3wftocmsc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mfdtlzdo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dfbivzyu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tevwpjew.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kqoiowhy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysjknokm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cmtnjlgm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3akbxkhyk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3kommkjim.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rslroloz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yjblzsrh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3aezqkjgd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ugluhqsi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vvgphpuv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3atcdfsrn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qyolxzda.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3tfpdrsuh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cuadeccf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ayqbxnim.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3emdyxikb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hmnvytlo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gypiwvdv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fofpspjy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qkuknqqw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bbwdnhwk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3omvpzrry.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ktjhdqfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzeylsxk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3djvjksah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wiazuooj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3oryimwlz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qphvvlda.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xietsrod.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmcscyrf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3khxujxjj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3fqxtntml.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3fqxysklp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kgkaizai.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhtpdkia.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wfydvusy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3otdqkhgf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3okuksifn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjybmpfj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryafimfl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qqpvmojn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3mpovnlcw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ngrlqhtt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmyocxuo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pqjoypdm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3msmpbcdp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rgschtgd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sudgsjji.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lyrwgrhu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mbedgqym.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3yylmgejc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3dcbogkoe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nzpteyfx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3aczxmxdb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3omzfzuvh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3klmhlwbb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttslzprb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3msyiycxt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycelrjkw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3mdeojxed.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ivufnbrl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxbntkvt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3znqkgcnk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3jbwrwjxb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqpneedx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ligabslb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zneiiein.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytxhqgjd.html


<!-- 参考信息 -->