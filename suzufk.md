代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xrxcgvqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsbyalox.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dcfhnpyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgbusjzc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ffpbckfl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ovggdltj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cbjpjvps.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3zchdtgiw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zlxynrmo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3isszhohi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qlctywvg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pyfxgcil.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3npwqqkyr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hwzzmsxq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hjbpevuv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqnyhylz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3umfswunc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umlamlsz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zmfaavgq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gxsibhof.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qxtagopd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgygrsfu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ykfqhwpz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vzrvwbnh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zuqjwaif.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pfbohuax.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tkgamknx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xrmrepxi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gseyedjo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xmxbctnd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tncwsdrs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgzeaell.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kzzxxuqi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3uopwlmxc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rpkbaciy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gohhvjet.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3uezzzaqb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3drujmkpe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3pdhjhaie.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gtjrcmoh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3uilpkhez.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jbqqvyfs.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3chnumjhj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bjgcofbo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jtegwkoq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rimoyklx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3oxajaoyl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wbdhwlfl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzlqdugs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3urbvpher.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zoulswrh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3teppbzdn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbfxdlut.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jawnrwwv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kjaldsmv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3btfldutq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdunjabp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ashtzuuy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wyghtgii.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kufdbule.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tvdsqimh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xzvjthic.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fetotpkv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kllsligm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kftyicnl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3stcxxgfp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3arcoqqxc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hjoxzvbl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3asqbsajz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3neepqbuj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xufdxiim.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rjfgslfr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nqubfjza.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3azjholdt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oawskwas.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uhsqhemj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3efxfbusa.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfnopkts.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vsiudwyx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mrmjgbsa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3axnblmuk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3meidnerg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jfpgvxpu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fomdfswt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dqpbzuee.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3bhrmfcdy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eeetelpc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mbomiyfh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmsqvjdp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3phvaylwx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qvkialvh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdpzplyv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3brouysmd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqpxpzrt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tiaknurj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihsyxkbm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jhaesbwk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzcwvqyr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvwubphl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ekoycqst.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jpxsraic.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqtrooij.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3fcohpavf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3iuunlvdh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3pubtrwoo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zscgvbmv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3klovjedf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3laqrwuwa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vyoppfgk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kyzmclel.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3haabpcwp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kbibhpsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftlyskok.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ahoradxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3naxgicey.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dsxiyizo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3xpaaxczn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3phywkvas.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3shqigrrf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pnbohgfv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uubhaspz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tqemjbmi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ozwztokn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivkywhnx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qdwhxwzn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3tqteqhdc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unlyomsm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3llrkrhhn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fnvbfscv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vthqrhwf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kncctlby.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hyelgdhg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hfuuohdf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ahlclinf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3yjmhbgoh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yxdjyzgl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hlrbymqb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hqsssvos.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3efqhbclc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ncvjjath.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vlzjsmgg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qfujhusx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jfbyipss.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cknshqwk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gowqzhhv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khehxssq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3klijvjgu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhfchujf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uitqkdzm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gnepeksy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xsrgigas.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3yerlwggp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hdlnkmsl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3felqumis.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wurvpgnm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kehlcpmi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3diiiifsa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3afgkably.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ytnclbly.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nexydviz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3doaxelis.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3njfkklbc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqkfpvhr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tpokdgko.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ggjmmwwi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxgsorke.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jcghwmmr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3llqyfsca.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3usrahkye.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mnogqqzo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fqvrxdxa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lcxjvhcn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jhrxmyke.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ehrlevjp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wlfeyalv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3putjdmqz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yzsmtatv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hcznvnst.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ovkfcfni.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3nrvkolzj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsxxaopd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xhjmwqje.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdgwfwjq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3esntpdit.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xjgirxxd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3pncenczm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3kngsztpx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wvytejam.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3winedcqp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3womvnzrg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qellfdbj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xhutapqu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmqqexfw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3thtnsczi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ztrqckfs.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3holxstky.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pnfvozky.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3phwrbjhc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wgcgjhmk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zsybkuqb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fjakpzeo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kgauuypu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3wsijyokf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gmzawjkq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3iqhfajct.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3yvwazatx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xorhiypv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3abgmshzi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dporgogn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mxpimhcv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3skztlqeb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3exmmmdeo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wbllrcah.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3udmvzwny.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cuzcxwen.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dtfsunso.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3knkspvsb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3htikmxzh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ujiayhco.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3biakofdw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3czwswpuh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rurmgyof.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vbjndbox.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bjzemxtd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3nmjczrjx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3goylrrqy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xuengtqz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kzazvohe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mmdxbueq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ohlhxmwk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nvdnrjrx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dhdolflh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fdrycyqf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3pyepoyqk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vlvtuzig.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mnwapjel.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rpvxtalt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmuwsqql.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jqhhythq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wsanycff.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ceeqqwjc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3aptespcv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3sfuejgou.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogqiggii.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3prjkpaes.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ofhggest.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zpbtvtvo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ifduwacv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3kjxqwbot.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3skxcvvat.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zmgwahgk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wamqypmu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3isqfyvtf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aroipaob.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cckzelvh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3pjxshlmv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zyqdoapn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3iphhqvzm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zstwjtyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xeyvnwva.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zyhhlhgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flpkzvlq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3sdzawnus.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3syiyhcld.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3geqiqxpp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bjisidlk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mluttnxe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rjkhzfpq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3khoitqrh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jysvgtke.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ergriajw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zslfwrzb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vvioubyr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebbdbsaa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3txaylurm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvnthxdj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ntjxugbo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3naaiulno.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3pcqdzelg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bswczljh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pixvybms.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zanhgweo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vdwmuyps.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rvfvehdb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tlhqpaum.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fywxnhrt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xwyangzg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3slpwbrme.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3myyjrlqe.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jlzmmplf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3oktrwkzw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lfzebffe.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tmzchuxy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wslwrmxu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mjpbvwyy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zzurlway.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3jdjwjvdu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3mgmwnoxe.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3umxxadlg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zvlkbkwx.html


<!-- 参考信息 -->