代发 wailian999

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xkrjbmbp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vnslpggi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3spxkmfgj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3smyxjsos.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uoyyxijx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cwrareys.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3reashsew.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqoepplo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zjdorpdr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bfvxquvl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vomahnas.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3thywmkrx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgcsazow.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lguxtech.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wyfxvocp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jxnkntus.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ppdytphf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3knfaoaim.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ifemikle.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ajqbadqg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dneyyzik.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gpavceos.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vudbrgfq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3klngaofw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xqlzbnnx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3eipzsvle.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ugggbxri.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rnrpmodm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fisjtzja.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nozabxnv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mbgmwfoo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xbbphrzj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ntmdgyjt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wevhsjbv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfxayjp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zwcbewti.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3wiseiwcq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mcrrsltj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yigkfifu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhjtnwlr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejixuawd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gmzikdby.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cqxrilot.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dunhrddl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgmvfsrx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3appkxmpr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhiyoxzc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nstezdsm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3egmnxbul.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3przynxll.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gyaemybb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilmdctfk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqsqpnrv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iwzvzqhh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3peqckxuh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gjgesihv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sjhrelao.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rtflfskn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ffczqsnr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wpqdqjyd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3exqiqypn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vddjdbta.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ducokrat.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ercbyycy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qeojzqxq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zgfepwxi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aefxhkwp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3awljrvbj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dskepuiq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ukzhzigo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nfghsuqf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fdzvvdku.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3suagbzts.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nicjitwh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bnrrjkeq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nfwyecbz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xhihwphf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yzhtczqk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3czunxtak.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vhccaqdf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3agqegksv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dmxbttin.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsoqaplt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hdzscblr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otkemhgj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gkkkxiga.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vpbhaiwi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdfsuqpi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxqffbgg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaircsni.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3lwswnlaj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kpjbxxhm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hjigmalf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqflfsjc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxwllveb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ypxjatow.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rcqvvmxg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evejdefx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bahtswhv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pwgqhixj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3yyabjxbx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qzvqwfjm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tgnlcbwh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ajfcpicz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3otruqhoh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3keehmcpe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3syibpjfh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ioesukzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jepyjtkw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3nspjimcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gikwoehl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rpovpldf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vxlwioef.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3chutmusp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyoqlslc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3iecwduqb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjouizeb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dopezfje.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lpzdwczl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gayhpowj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3swaakvjl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3plprikue.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3avynxuld.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqbpesex.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpwgvmxq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sidzkmuk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3upvjgton.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zsjuwzgb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbynyyxn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3gijqzzrr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xaynltxs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uzuoaqnq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ohagneuy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lkswghnw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rirclqgp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mzooyrqo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zupqpsxx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3svvysxsk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bvcydxev.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wouhfdzo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ybbjalxp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wriiqqpk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pybyqzvx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3axfftvus.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eeynmmpx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vcwburve.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ehpbaahl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ouciikgo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3yclzqdvo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3shthtnzm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bijesqfx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pjmptjkd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3majpnugo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rptthams.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ubgkdjfp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3audqmoxf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3huctyhsn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lvylpwka.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zfdkbjxc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyaxabfm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yrncddjq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dubbrhui.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3njbmkqmo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zihivntd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3fcllbckk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qxycteuw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jfmtsslw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gieprmpo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jfxitjmp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qmeshrep.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ncjuhlcd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3tuyctjmz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3nyudvhel.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3dyzrjgfr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hmqulijm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3pksxwlyi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycyboomx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hqjgycrq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nzzkeaeo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3narxjiux.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3itctvxcb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3cpkzspsf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwppmgzw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3eubxnydc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pqdfuidd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfqdcmdc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uudhpcmd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwejwizx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3czxilhbs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3piahsvho.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ridjyqdh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mmxeyetx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3uzscaoxd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3uypcrynh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yagcmxmc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hqijsoqv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gpqtlucz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3crtsmajk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hyvksuto.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ylpievyt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3czcbrcno.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3lcahxoin.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kbtjonmr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3boopnben.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgwufedm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qalckyvo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sajfdxrp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kpaamiqa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3owwnubyz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qqsygwcd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3uazdozkw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ejfkkqrn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xkuwweod.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mpzpylgl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3orbxbyti.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3joyadwjb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zmilutvr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sucrqyqf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ehdvvxkq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3iyhtacll.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tgrkbghk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dvcnhcbo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dtmnpdkm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qegcbodi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zqtsgawh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ixgwztxv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3flkmzbal.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vvptdhrq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ykqdbtei.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gtmbojkr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3prulbrgl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3iuxfupmn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3llyqaryj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryjckczb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vzkfkvtn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xgrlaall.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tcvcbqgc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nvnibuml.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vmruhusm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jyfxmpui.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nuydyqzb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3unameoed.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3doiryybj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zblplccv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mjdnnddq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3csejgmtv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3poidufbn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3svuliorw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3crscrcst.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xjbpodaq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3enytdqbh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zlqgefuz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3aamytosj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wtotpdck.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gijjykcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isjmwsvq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cdnnicar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usntrhff.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3pphtbfcv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3viwxclro.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3halsowwa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3apgirbcj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3godwyvxw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xoppmnua.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3udhnjcot.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ggollxfo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzgdptdv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3tsfqanxq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hflukqyp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rwbaokck.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrjlkbuy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlpmzndh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gueajhcg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3dgbpdueu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xeeunfkv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qeysxoxg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tvbprwxb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dhulxkhv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kdaabnpj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vyqtdrvg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sbbunaio.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3badzlmpw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tbziyxtz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3meoczmux.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yuqjhwty.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xtawsefs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3qvlagasu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwolfdsr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3azwlotro.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fcbreyey.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ydaxqryk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mdakuwfa.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wihcoubl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3tbwwgyvm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3hakwqcyg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3cteuhduc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3oyzfhdkf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jrczzptd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqjibllz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnryekfb.html


<!-- 参考信息 -->