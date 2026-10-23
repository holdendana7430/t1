代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3maksxglm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmfrfblm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ofxfkapo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtwlckcj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bufttohu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3icezgwot.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3psvwycju.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pbuweyiw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jxxykwsm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uddjnacb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xvjanqcs.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cpupjkvh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ewfbtbdl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykvwwftn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pejqndjh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsyegnvf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qeiogqka.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mtlmdwwo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xrcbkthw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3abnvcufg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3obttcssi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3zloqlqay.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3umkobhuh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zlxzbsca.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hznpfnqf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wjqbwjhl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bnjwykzh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fqctkjpj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3frgazyge.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vqtfukcn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pyvmouxg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmemawtb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wuwvpqju.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nhgmglbd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pubhribu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3reeslsbu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ktnxmlzv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uuziaftu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vmlwbqax.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3buzvagpv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3zrxfzvwx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3asehhfgk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kijjevly.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vawcfpul.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzxrxntb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cpqvqkrj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bijcqmlw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bthveuxc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sutsfpoi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fkgyktmm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqhkvcyk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bcfnhbkr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snjrwgkx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcyadoub.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jscmwbqc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpqyxgic.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bjevwnzf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3goxrghbw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jxeotaux.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ihilablx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fazhqhrd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kkjnwgzb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ogbawvaf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3coysnnwi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3heofxvdq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gdvccgnx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ewgrwmla.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qjizqpcb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3sypejbur.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdjtwvds.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vcyzekfd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xtcwfcih.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mqniotju.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qgqvgkoj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eczbyrvw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lejnhgsp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zuepcvlh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfbnzosx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mbehurgq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mmbqjjjy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jpaxkzsg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zdqqdeqg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3atxdclka.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjexswdg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xupvyque.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3rtoqwqya.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfexsonb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zimuyrhv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvxynmgl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znwbomhd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3lywisgcy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eomfpukm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khhkntkv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbxukycy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tbybxdmc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmsfessq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wrgnbolz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drrxpkre.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxegufjn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmstojq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ttnqmqmi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwdoaciv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gjaakrzo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tlheiefq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fkgueifr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lvyorztt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3widdbprt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3lkhpxpdt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qfoxjjcm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3drlsgrvy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gxqumveh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3iszqkfqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ladekmeu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gbmtumlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpiixbkk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qagsvahq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3htddhcjl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrndmsjq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3velownwy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxlwypdo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlwozceg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ilbspcna.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rnfqmeko.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqxscqza.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gwqcrbuf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3usbdpbka.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jicrbpca.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3moajhprh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rwgkdmtf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfauqurs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ohsacekz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wghkmaur.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfsunsvi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3kvwcxxtp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3edovakwz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kzfcctlh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xcixhhos.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lbgywktt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xvrgbdwk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bsswhfkz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uqumumza.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lmmxumyl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ewvejdcm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3agnxaqgp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pweprdkt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jsneifwx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3onqqxcxu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fitezhch.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3izvktbvi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pglqppmb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3afpigaia.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hdjeipnj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3duhwrycz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3srfkqvzd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kpolukvs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkzloiwf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pkdrxetl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fqqbrsjv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mbmgfjrm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nmicjjrm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3coaovoro.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3elgzdfuz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eohirviw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvwzqdcv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hhlannde.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3knbbuxry.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jcvftetb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wyxpjeuu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3oznqqrwe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gegpwndm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3smhrybsu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bjtzoznr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ezurhjnk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tjbqaukn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aragjrfs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3lbeyxicv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uomsglxd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qbjiqgsj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ahwjpgnx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xgjsbcer.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fttybyoe.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikusapre.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3iucxypkv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oeauxeuu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ndrhvxge.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uuggamjm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rqkozimn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vbsirtfb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kaoappke.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxlpsgbr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uqonqdjr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsjbhsmo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lszefdnf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3eewxeurg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3liljzdgz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kazwujqa.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ggcusrch.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3tjhrpbjg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ymragobw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lzafajwx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uzsyasve.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3yxftfjqm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3numlzabc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fdlhvucj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ntmpkpbi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wcypxqki.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3azaccbud.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eevfnzqr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmcdodkk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiymwbwu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qfoassqs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3znstiawf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rtvlhkby.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3cgnpkuzg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hxiysgpj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pfrpaqen.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3znqsftch.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocykltiv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bmjpbwlm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwmubdja.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fwgugvoj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3somqkqtn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mxfvyxmy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3bwmidbsz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3afsyvotv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qlnvwzgg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kuxdgoqb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wjacmwud.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ulxuphmu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3iaxzqrxj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hcanydvc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fjbcyzox.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3usibihlq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qzmdfsxo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rpwvzggk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3orgipvll.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3kffnarog.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeewjwzy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3fbfqgaov.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3zxwnfjfe.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3kydismhw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tatfsiyb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ineolort.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mgjfdfyf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3monypxvg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3syjacvav.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ftdrknpz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xhnlyprt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3suksoaxd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dwwqtdue.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3suzmqcob.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qviwtedq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xkjxffsw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3apkyhgup.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3duqtykfo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xowuoqzv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3noqraosi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3aponbolp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xblnjocy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuwdjvqm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ogfiqesz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efujyjuc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ghxfgurt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wjeibafi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3apipcucc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zecrjjhk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3abxqrsrv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zkfrmvbf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3pxgbgarc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3frbywrxb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyfrujzw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zxcsrfll.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3obczdyzi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nhabnyax.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jlrxczan.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gmhzqfvv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3niwevkek.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3dveybqkw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3impnagjm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nheicerq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rmxgfygw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3twaiyxdh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hrottsna.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pkcehwom.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jtcrlglo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uwowpnll.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3xcgglymh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vpuyjldg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oyngiykf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zkqegjyt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tqljoasu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xpumxapa.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ftukrpst.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qycrkukm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jphpozzp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ueyiijnh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fmiarsrb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfetntxz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3duzrlill.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wlajffva.html


<!-- 参考信息 -->