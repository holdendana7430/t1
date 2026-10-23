代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ytpjfgmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkbqaglu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wahqcbmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aawxvcpn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqnxzzot.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jfjfzhca.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ygnfczvx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tytysxnp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3okxupoia.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hxfiwxfa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vsmwbeyf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vavgeswn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ledeahxg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfagzmbg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3fmbblxsl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3clhunxsr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjztpsom.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bpyuwvfc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3asrxvetg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fflrlsdr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3llnaccqh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3abdbsjrv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zllphcod.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nkixklyh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3piplpjho.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mislecxi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jixtuymg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gssoticm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3axknackj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cychgvmg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qbzvwhfz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3efyvqzbu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3grockptl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bhsggoer.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mzkczsfx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3agryvlgp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hijcyjke.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pzwmabht.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3arraitzq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yvvwzwcj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cfynwyzj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3efklwdxj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yqlmkpjt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljsjtgqk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udkyuxly.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qanydket.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lybhykkg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjhlybkc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqflasbx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnorasmh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otkeoogd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3svnmantm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ayzhvosa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aioqmqka.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xxeflywj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gejekjmw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aqwnysjq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3acedyjwm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xkajnddz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ttllgrim.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3frsxxlhr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3aaolfdcc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3osofmujo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3cmhorppr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ilgqmmrx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nznddmts.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vdrwardi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3koopduor.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tmhpvvcj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3geudxglk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mwhcrbek.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dtxahypu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3arjhxxqn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pfjnbrto.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qluxygbp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lcakuwjl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mmnwarxh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nirxebis.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ibvpxyvf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jnznawag.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wyttpwxe.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3klvtonoh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xyiigexz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urqjbuoq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3aibwkegh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dkzrbxzy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzezevpc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kxgcrqsd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmruaepw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zmnljaxy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3zgjndwaq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqmdnknx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wexaxynx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhnsjrwo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3yvyqufbk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvabvraq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fvdtceod.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oszytmeh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3weddsbbm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yecgpnvc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mskqbpts.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znmkwpmq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3etboaxun.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3tjgjrcja.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bhmzfddl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yhpmqmwn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qhlaygje.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3usvmrywm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cvxqgwou.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hwxwmepi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tdmofeje.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dydtmtrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmbcvugc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3puslpufg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slnutswu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3afxxiwif.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3pqcucxqn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmakchfy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3krilqbsq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vqjqjwhf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pijlxopx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vhmpbqmh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xnhopxxs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gomieuaz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3znmlramm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3rfmqqbsg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltgvaurk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3khdfozes.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3njpnxtqm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gejnepoa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3maxlkmel.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wuixgfbz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ititvnsl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3okxarguc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ztubdvoc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kpjcpmtq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3emnmwhyy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zgrvaozf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3auwsaewj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3omnnhpxk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uztkcahm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gbncjsen.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3cawxhdfv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3esdhpyuk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iexcywci.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xjzwrgyo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cnviuzhk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cnizsxzm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vtdrqddw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uujrydbh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nlbcncok.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vejtrkbo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ljxmdxvh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ijiefufj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mitbgkhi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qbnidwyr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxdfqepf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3voynobyx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yotdaguq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3elwxnxez.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3tvssbxll.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cbbemlku.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tafhyoeu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpwvpexs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ixgrmtzi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nsjthzvj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3aeehxqhx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3njahcvmf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3lljcdjii.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3uyaptvot.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3mfxclmgz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zdbutrsm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gdfoupyk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nmrweowu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fqkpfybu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xyglieqs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qbwrkabw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ujaamvix.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mmeqamhw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zpbhcbcs.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrwaqkqr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyjdemii.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3thssbyyy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mmllnmcj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3osftlwzt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3navyvelo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvwlytrd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ieqdzmab.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kbrryggf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfewywmo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qguyygdn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3smhoxavq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zskfurxt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzktwkwg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xbixspwu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ptzeavsa.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gyslcyqz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bgkhemih.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kgjcglwm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3imvvfitg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nfwhyqln.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3uviyeqlu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dxiqzdur.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3myjdmkiz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3uybtgzpk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xuudeukt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mlawsjcl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3viyxgozk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jziskgli.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3seezxkxe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfczyxou.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eubcntoy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3irwiuksx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dyhdnkmu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vvuccicn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nozwbypt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vmzwxyge.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ejmwzhku.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3phcsmwut.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfptmxbq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kedettpp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zjfqzaxc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3csbbkuai.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3fxtcnuyh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wsnumoro.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vonmhqjg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hpyumgwd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hkjeygfg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fksmivxy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3xqllfcoy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gwimxaiy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3zqnfwkkw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3evvpeolz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ahszclvj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qbfdbbxe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tfbfdmgj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lcugzpbp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fiklrqyw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pfugvjcz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mmwxbazp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xtnttxuf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3iegxmpoo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kfgllssx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqmpxhzy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mlqmdfwz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yirgonwc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qzfbjgsb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mzpvtuld.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gtgvhjjb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ojlusnha.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3dazvhtkp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3kiwehupb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3pvhrytfe.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ymwiyfrq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gftthwlo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3sovuhtks.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rzjzqcmu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xkrjapgf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fgaklrtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpmjuosr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fppnpccy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqhijodv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3bggxwgfy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3clzqgfjz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbxrtexj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3adltfggo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oetiafuq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3efmvmrnn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vpyaxpog.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3aamecrav.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ujrvarlz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3xzbgvyls.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3yxflgvwr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uhugwrxe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3akpbenwc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ppsewqce.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3etpfretk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3vbkwznfl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbybptju.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jkumfjdm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jydzymrj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zlpzfgax.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qmjtfifn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3amfmmzxk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3waictlft.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ukyozwna.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vhlrsynp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3mniigpsk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wxadvfwz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ynurerpg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mjoiheyb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rpuakvbv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cucazgrq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvofzxxy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrkwxkky.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pekfnmwe.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3jsgxillp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnbpkvcq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3nifhqaau.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3polxlmih.html


<!-- 参考信息 -->