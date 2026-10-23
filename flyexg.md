代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rdwpdyfp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3oiejxljj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mqvqcwkg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3phyftdnr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jgslkfbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdargvjt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bndapbcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxfmrkra.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ysdshqvk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3neqiqfrc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mrmhrbfa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3lhnidkoh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oppooleu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hbfvwdfb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3scssdogg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhqpoyzl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3itbimtma.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bhbtmgjv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3latyvovf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mxkpxlao.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lfsjkccd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hthyeplp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jftdqjas.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3lopggzue.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3degszlnc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3zanpiixr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hymxebcz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ulwikfxj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fafimqki.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bjnhkftf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3diizlaxf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yjbgftxw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dksyaewf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bsezrzyt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ekefsgrr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3nxzqpgzr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tatsfonh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3hrlyuqrh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3euyxscbq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3emmlwejp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fftbsqne.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nqrhstkl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3tibxkebs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sduocipg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tdlbhtbk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vibrxsqy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nofhvizl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emlgflvb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ioevkirn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3grmiluog.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xsxkfytl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oagsudnt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxqbjddl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3bijqjtag.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atsqueom.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cipkhpcu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljbdhuiw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvszogeu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ykwapobk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwkaliag.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrlxppnn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3axrbblxu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3slfmmwzi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vrglaybu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bjalobhd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3epdbsycz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vnhgzkwq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vasbwoha.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nwmxyhhg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vhpmmlnu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3nhamkfwj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ufbblxtc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3nnovxxlw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fpzueaky.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hfvvzaii.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3izfixjhj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cbjfjstf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kdryawdx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hvzxsmxw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dvymxvsi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cvpehkok.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obtuynri.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iioazaej.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yqyfluam.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hpksnbbi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lnxlnndj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zqaxrehz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjxifgjt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gjfqrgxw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3prqbhfck.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzzbcbbm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ughedhxf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cyyazurv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3badnpuij.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ytmcqdzu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhcqfsar.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqprfsze.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgnvguop.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3egcllxlj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lsyeptke.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ccjhmjax.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikyqdfhk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqmcxoji.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mkuhawvb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jhvwjvkc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evnkxsiy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cywqqeud.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gzayughf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3bmhcjtds.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3pnbyhays.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qbwxumzc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fvoqytgh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3iitmsczi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vmblrkpo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tprdhosj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fiwfxptf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljttegpm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qujvoijq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkqrpspp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mlgrylxd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3slqdfugm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhapkmrt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vkcezswq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypuqydaw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jzgwemfb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3chwjfzqi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gpvpzkmr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fdwfcigp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rawbwdlh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3agxrjdnd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqhcwyxt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ilxxespd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guoyowwk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qzuyqnii.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wkpcafnj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ktrpnjng.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsnkhxeq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3giyuayos.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zpopgfru.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oweeeccn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gwdvhrev.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xgiedoma.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3uqejcpyd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bgthynpa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tvrhlnuo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wvxfdeyo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3sqkmtowj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3roewdycw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3npjlglsk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ouucofxe.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zzrrqlmw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgsediqy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3afotpalc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3phggnaxj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3szzlrcfe.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3sunhioek.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3smipspba.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ybzqoovv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gqjcviiw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3drmisgzt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hivbfoks.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xiortxto.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tnqxkjvx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpymkqdd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ekalvqha.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3eygflycw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsqitayy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtefzugh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhhurwth.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mdzofwgn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3equfvxty.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xyzmkkrg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mqcxpaew.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ijbzclup.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3evxaagnh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kiswmcej.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pvuzmyhr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jyjuemwl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rtlxsnvk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3urprufby.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nlzuqiva.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qtjzxnrd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xswlkggo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3xovnqhuy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypklirlw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tntqsmdf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fbroipst.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wxcxmkym.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tbetmiug.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bawyjzaj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3emudbeui.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jbcskfuf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zwjpokmq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3nosovwty.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gruengmq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wmbvuchr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajipmvuv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3esdlfklj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3woqmxipo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3poquvfke.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gzephsai.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3psvgyunn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gdcctjdl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tsxgkald.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ikvrjcme.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ndalqzno.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hgtlwlin.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rrrnvadv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nuhttqlv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3pqmbagbn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fnywinyu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewtremue.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cllvrqpq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bbzvmoqs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrnpktdx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3azecrwba.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3acjizprx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3asmmywxa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cydtzymj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fseacynw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtpmtbij.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3broxrqrq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjxvuhkl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3myyyqzqm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3snurvfdk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vlxfprkn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ctqnkrjn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3opsdskiu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3smllvnup.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kwjaavzw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zssgxqtn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3owjqskmh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gltvjcql.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bqbgdnez.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3izdqulhw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wnlvqlxb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bkrbmdmn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wmmpaosm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3snemxqrk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xbdzqgzn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3widpwbme.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3euserdht.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3azkeisne.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3avnkidgw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qwsfaoyt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bvtomdtg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3crvwqcua.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3eafcmexh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ryogtueo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tyvhghyy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hfinqxlb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lqpurdow.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ywuabbvn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iwlewvjl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sljcaazs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zpljueig.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zgllljey.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fsainhkz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dhmuoiyg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3phsvvkrv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yawduofq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3plggkknp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xelovesv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flsgxdyk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3eypknuxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddzdawkv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3flvrufnn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nstuoijn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3iyadsvkp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3npeulmbn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jpdvcnmr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3afyrnpdm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wedwmvfl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3crbepszh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ncpbihht.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dijagvyg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hrdrbcit.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fswhmzku.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3izmnzvqa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqkuhxfy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqxfufzu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3npwkneey.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3shapmqwp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3urcplrzu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tisjbhtn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xvkinwxj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vvymafnc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nimqpfdv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qymqujyw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3igdlwery.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3kpfziqlj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3yheogmcu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iqrptdlq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3pwxzpfvx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mbawtynw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpbokemo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ddfpmjta.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxvhfurk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jchusfpx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pzkttbho.html


<!-- 参考信息 -->