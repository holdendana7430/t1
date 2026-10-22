代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ikutkkpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iefqlmqa.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2kpkjlxky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfhjkqvb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujndbfnk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dogtactq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jpgjwqut.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hdzytqzi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hnqazaoi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zsgezetb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xlgpnqxx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujjhxons.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yuzgaizo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2whgynjeu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2guuoxmnc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytbucglb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bnweysbu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2spurciya.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vtruzmdo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vijcamyo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2cvjagasx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ukijivsn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2udspljnj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fpagozxs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jamatppq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oozjaaeh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yvojknzb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pptkplhh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lzynyzad.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2cugqsgup.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2clheqgkc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ngimzqvd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mvxttgre.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ueompytu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aaqzwxki.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uwbccpbg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2haeyebyb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lrqhqbaf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2zyahamer.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nxrwzjez.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2coirihbx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jmcnffwk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nqxkbjeu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kyqzvvvu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwmhtmkn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jovhcipw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ynytrpmg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcweyijx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txastlko.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2cjishdnm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvavvfyd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zhyauilf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrczzdaf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhxnbuic.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hkhnudtg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jegwqvpf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mygrucoc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfkqbklr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jaowpnli.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hmavgdbm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2juhbvhdh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wgdiejsd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vocuutzg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kkaqwiuz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2btsmxcdb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2caxucvuf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2whmuhkaz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wzghzpda.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rqpqvhdl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2opgrjxyc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zvtnokly.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yganhffu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ehkjsmep.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vfhjwzkt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jxkmysop.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ihbqttqj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2aionkaxg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkmnmqna.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rnsordkh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rdhekpid.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hzsunwlj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2murcwxdq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rifdqxqu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqkxwlrb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xooujjei.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nubuunyl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqgtzbsq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kvhnmhpv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yclxharj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjzklxle.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bymwmpfd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tdptirkn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zddphuer.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bfctibql.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxcjtupa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2plhwupbi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ityyiiok.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yewztmav.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnvgjxqn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vbnmnsib.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2iwehjiiz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqqomxpc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ppbdasom.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2icvtlxgw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mbpuzptf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kafesxpn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dweshrcz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cmxrtyqz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mtsddpfp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rnwvfsai.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qowbycir.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uggifwuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfgtcfhd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wbwohbrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myjjrjtl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gvwemwse.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wliczrnq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryjmrxjn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ppdoneac.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yznxzqya.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nvggnhao.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pgnhjgte.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2yjaqtpcb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ahymnwjd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtmbvovx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ogagcjyy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2riurwobl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rxjggxfo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spadvlsw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2twkdcgof.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2pgfgcgkh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2dzkiuvkt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmzbfxwz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yarmfhri.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qasjodle.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2balnfuox.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yrfcgddx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xwethano.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wknwdish.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2crljdmko.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gpzwnuep.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tdebbsql.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ryamzvhe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2khsakuve.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xtbxnnyd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ibwavsrw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2idxfzqgf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vcuuoood.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dhinjqve.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pezkfuis.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cinxfvsn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jvvmcqba.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kflfoivz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgztwaph.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhnnetty.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhfobfnl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzzeouut.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jbulfdur.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2iyocxlth.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2egwncsrj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2yuffhkyd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2auxciuog.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2guzakkhl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nxzuyxdd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oityzltz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hjxlngvb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zgypnudz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rjlhxuln.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rrhvrmkj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bwsedqkk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rwjvosvr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hyjsmqss.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cjtgmwrf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pwupzana.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2myezxosq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ujucbylg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rlmumxgc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bonodpza.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wmcvclhb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ddfpotud.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zsythpyz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ztmnajlm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhsrlaft.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lflwrsod.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wfwugwvg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mdpqnrjx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2twctlfaf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2eagqmgmu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2opcnlass.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ybkzzryz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2utnzoanv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vgtbhlew.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lndvbhrd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vtjpaofd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2yaxiogzx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfubhmfn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uafqzidf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2iafmochx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mjkzthwf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zvzvtyge.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uzwcrzdi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dcdzcwtt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2oticnnls.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bqeagiai.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vfgrdxht.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2whpgmwwc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2xqottdwi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2opvqgopw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlenfbun.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcytphus.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvdxuadr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hyhwdpci.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2tpmwkbfw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfebwces.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cghuqhhk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2drmxbfkt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2htjpddxt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yowtkqoy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rcqwrhsj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tikndmki.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eqfyhtsq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rdxymjgu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2foptrwne.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2nxkxhaxi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qejurgnx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ruolzfku.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bfesxwgz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2staqlokz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pmakmmov.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2daqrjibg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2udoctbdj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2fwclkusn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2axdbotxy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2iqlnetku.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2uvavcpit.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2rtplxpkv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2sewrgxkd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvjqgvhr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fwxtkqlc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2wxwpxnqv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2aimivwgc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ndsphemf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkjmuxmn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qufjfxcc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ekntkfzg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2shsklqkr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rqalmhnq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gkadkemz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2agkwtsma.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ckdqmarc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qkyuaxic.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dftjspam.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2iaqsfqcm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zaybuepr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdivvss.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gclgcdbj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2obfnuazz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yovxoarn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2iepjrqpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idwufcjq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2eprofoeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwuxzenb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bsvkacwy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yztonunq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nomhsbnh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgxxjdob.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2murvtbse.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2euyckird.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xrqjoswx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2isyxrags.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gbzdqsqg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2psfsperk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ygyazqvu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nqiinpvx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2drlrwfsy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tdzzmmjr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftocajmw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wyyoycmq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2cblmdken.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eojxujnf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ylpacjsl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qswixxht.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vqndtdnz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ducbkuyy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2otlxtgfr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mbuskljh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jztintsf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wtfbejsd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mbpviymh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mjiwoiws.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2janjsnfo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2quxijukw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmtwxcgo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlxdhkni.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fhdfzdlr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2hvqjqlbi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bweokvhe.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2sqflvelt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ifhfupvo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2oejyjtyb.html


<!-- 参考信息 -->