代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yslwirto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bubphopm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3cjwzlikk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkyiarlx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkyktnid.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3adcpvcez.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3idttsfvh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kphlstdj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tckrzqmg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wbmdjzti.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kvnfmxiy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bivapaqn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3edkmbquy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3cemltwrw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qibqbifc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mlwhnqjl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dffbeeoc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3axxdkdqn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zlxzviuj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qhyumwrn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nufvyepy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvwffuug.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ojlfjobd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vuigefim.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jxzidwjm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xjovumbi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3foekgybo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3mumarwfb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ornwiumu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3iawsjxlf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3sqqlovcu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fxnszype.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hmblxbwt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3okosyluw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ziqsmfay.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ikwzewwi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3himfhxqh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wltkwzyd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3knmtqtgx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eslwnmxm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uwnomvjx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3whidnpbi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aoisbouz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwfxkkch.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbhfbqbv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cvhcrspg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ymbpzmdg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxtwtrei.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdifpimb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3sunryspj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxzayrcq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xauntjvr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dlrgogne.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abonippb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ogplvrsp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mckynvcg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrkgvkxx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mcrwwyab.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3viugurwz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vzgqxgwi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3numcavbe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dizmuwcu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3axtrudfl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wygdgscr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ponppzxd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ezzjuzfm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3iynlykpx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gnaphwmt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dqmvkgja.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3swtjheus.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qtendayy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ytgxpuxv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wgxzdxfo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oqnkepoe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3eklphjvx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rrnjjkkg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ibdghwhz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znjhxdqc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rzkbrrew.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3phcgcypm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3umsftpdw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qylmujws.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ackepeyg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxlyejsv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dwpsrlya.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3riijggrt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3njhsujvv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kpwteowh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rokqvhbn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qljuhohk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ijsjpcbn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stvhzfwn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxsosluk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dzftdbcr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kghnwepa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvhtnfzf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dvtztcnu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vevqvfdd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cekavkvg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xfdxzdsf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hlpsznmp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kudddcxf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3axiebzfs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3yphnaoai.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cfgmrccn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lgendfpx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ynqxappi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3egtmwmmd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3lqyociwd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3eyaycddz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ttzzyjkj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xdhegojp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfgjxobe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3prgpfjnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ankpcbiu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3sdnfssif.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3xxvksvuo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zkaxdgtu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3otdmiysg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbiqadex.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xibttxwn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3psdvdwqk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3swpnjmqn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3connyvrm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sbqdevju.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ewmkwfou.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3utdrlumf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3viebhlvc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3avenldjq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xtaidzlk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3oninvcao.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3yqmjvdzr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqorwast.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3yoefyqtg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rrqaojzb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3knwjlzzg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uyhjakqj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yidgoyuo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nvqvmjlf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xlfacwrc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3soqgfaei.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fnkpueou.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wqmuyuba.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fetisoam.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vpjubepl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyandhmv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ygesskbg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qeneoczt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wpvibstt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3clssdulb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3migsgnmd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3saeydyyg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qbdlfkah.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzrfnlci.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3luatgpvr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqvwyrpb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaiedguo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mncdlkdt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ywjtzziu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghlwoguf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bbcqqnyp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fzbbzmem.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tuyutuoy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vbdgoqil.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zohirmgu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncrdvbpm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3fbntsadv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3csbczvpd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3karcpshz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xmdbbycg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qudngajq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ywmbbuok.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vqxftcyn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kxxadzct.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qsnlgvas.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jctzspir.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dggkfnjr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xggwhgvz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gqaafcbm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ifthrgdd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjgjwiyv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rccjagzt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohwfpqfz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uoiydzpg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hvdhzxlr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwfvlayk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zngdajfl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qjxyxzsx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3knbeduux.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tphtxetp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3bynopgds.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjmttwku.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvgkmscs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqxfxcn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3pdcbtlqf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3uqszqfrq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gaygebwt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3tpxdzrxr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qmohljjm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3mgbqyllh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3igvjpvzz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rjuzodku.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3sqvcdmve.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3okjxaoez.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3bswxltkm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ilfzcvtv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hxgjanqb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lagnceso.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ebjzvbub.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bkqqksun.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rduhxlut.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3njkhlqpr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3rmkbzisd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jejmbkgu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3stkwahzu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kvqfevef.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mvsmobro.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuagxpno.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwmqfzzh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ebybbvpb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cibfectc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ufdrdeid.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aiakpzcc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tpvavieq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3utsjigge.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jkhzcjbw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gdikorrg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bwliltcy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3asewhyax.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qlmxgacz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vujqeeha.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bposvscc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qvuzqyds.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3dfqdyskr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3haishmxz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3tujxcakv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jlusbwuw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfdyvhla.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3xmrfukjb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jsoilpgh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3hfczdqgl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zzuzfchb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3scceoxoa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3umwjelcs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3sgjdrstk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xjrhofkb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3oxjrdvpy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcdbhju.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3kpigkkns.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jlqrpuzn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vshzfscy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3pufaclkx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pryfvzrn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ozxofdkd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3roiupbmn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3qqmuaegz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cwcximnw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3llugddsq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wstnpdpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlzmsjwr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ryouzsii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3telxsqzr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3eavphwil.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ohsnrfsi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3hpxuyzhg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrdsdjbz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ljnquqok.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yspgqrbd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3dyjigzjb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3oyfwdfqe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3upkxrzmk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3jmjliiqz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3iagpwzvh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rlrfucmw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ypkspdkf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mjpxidmd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfisenkp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ugdbppuo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dmxrtwgw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3actfumbq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3udhkbxwg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xonxqqbp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tttqkfxw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xqombize.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zysdooqw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ztyrpuhu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3aowbeivn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3dkjrbnng.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iplfmtsd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ymlgfrbx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jjkwqkrc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ievjnqdv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3syaqbjzf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qlosarwq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uzeemkmg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3xgfqoyiz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3cbwwydhb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ywpaemhs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3kixuxtnx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3eufcyvij.html


<!-- 参考信息 -->