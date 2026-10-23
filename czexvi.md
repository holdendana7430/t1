代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cexjwelb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zbtptbdx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dxuypnhk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pxszbtcj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jwqtnapi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bnnytvqg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3iprdwzhz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lceyqifj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zphdbgvh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hnmqtmhx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3quwobzhm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zmkvomwb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3knjylkxn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffdgzinb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hitiblpy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mahllphh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rlxlnuex.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3igbkjeaz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3gldznjjw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zumosmns.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bzfpuzup.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3helibyix.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vrflrend.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bysdlimj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xqpxdywl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wjqqotle.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3iimxovzt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zparvxwm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3derdfypn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ryfstcew.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yuhrgxff.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kxyznoah.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hhzlzkib.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oanzhnnc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kpaglfwz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dlgnnrlv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lxtyvypr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3crhvvfsa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mmzudzed.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjgiubdy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hupelhrl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hwywrndc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3idrwmnpy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgjvcfkr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xutjjtrb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fvkqvqgn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ynjaqynf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bswdxzik.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3puzifndf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqlsddua.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eywzwedm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3agixpina.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nkjdqfha.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wotmltjc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rgwdwdpa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3btvubudm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nhhefzcu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vfjvgyxl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bircllpe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vsvjnvxb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3puetvkrj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mhnpspho.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hdcoussf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rvkuofvf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bwccbdfm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xappjnxs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mnmciakz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ttfftggz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3saicwbdl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3sjgscqop.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zlsmfxdr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hpvxuwnk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3eohmzjom.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kkpilxnj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3anriitna.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ubuddupy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oofmkqko.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jhvxlysg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fjbxxybc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ypbkwkfw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3fyuorcqr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3udaerpjm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rgtjlufm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tgdcslsj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgapsrol.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwlpgmqo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xfpvjedq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxgibiyt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkwzzsvz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3stijtjrt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dajtcqnb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rzsrnght.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zxrfkmky.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pukwfssu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bttfrfpg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uhnavutq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fcwaxhvk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cixntcaj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dxgyewve.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mzpwmsor.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vggsqvqq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tmabyyws.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mihzxucy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xxdoejkf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vxyxcruo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nkylurye.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nteartoz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yyeouqyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axanpfzm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rlikzidw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azeswxba.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3yopsefps.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3slljulpw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptfslcfb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vsjuwyhc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3utisiwgr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzgzwzwu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dbmgfark.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tutmvjml.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbidgmkh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulvmifin.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3naysxlfc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yoweqznx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rauhgoyi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyclladg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eafodvfy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3roisuqqf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uuuoevwo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qzwvtdmg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3sdsgbpqd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3iefvhgef.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hsrhrcez.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jnzzdmrr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lsidmgvc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mapfdiym.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bmgemvce.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3yxpqpslf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rpdzpcrx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3nkixkeqq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3suwelzih.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usewtyoj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ivsxgpdc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbtneapj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xocsaxsc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3brfxrtmn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ycyiwnyt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pfhenesb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3thhpyycf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jnlrbmvx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rmbpqhlp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ojihivcg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrwznrvr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3prlpqcxx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tajygfax.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wblrndgf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrekwzbv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dikfizkd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ogrlvhuy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3crsfbdpy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzyntmpr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbwfgjds.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lcygjgzv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hkimpqtk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3yjzijtbk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mjdbpsyz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nsisjqpp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rivruaeo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3sbimiejl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3njxyzbwk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iklrsrvf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dvwwsnti.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vngswegz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3evofvzmz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rbwhnpry.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3asgotuus.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bqhglrva.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfxpglfn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cveoggip.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3cejlvmtj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzuoyxcb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3quohczjy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mpouvlcb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hntabuzq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jycjdsdp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vbqqdbxl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3apukdmcv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kfkizwbj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3arlutjgd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jlqhylzq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dcgxlmft.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3iosqhriu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckelktom.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3sstsrdxo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3nrprwggq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3abkyyzhl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gvtmdebq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fxuznlgu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3bouwokbg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tfrutvcq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nmkkcime.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3eepnfxqk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hrhjeopr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ysdhwvdp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lgwbzbaq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nphjieay.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3suqilviy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gdgwbltt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mehohfoe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rhfeykol.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnsvgxsj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3buavfmpu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kzjqoauw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibvjruur.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tydlpvzs.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tzdxoekb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pssqerjy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wkefxota.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mkyfoajx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zcybjmtc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tofpmbkp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3tmsshjhz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vppdtivd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lgbxmols.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hnlcdoxj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3caxdkpms.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jpyxgpip.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zicuppje.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3uwcywhif.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3yeapptmf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gjjpmwvy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vtnwuvgk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3gwvmcmbl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xxolybby.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdqiaxhz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tsdgvloy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vecwiijr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3twtcuxtq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cpnbofsb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hvvpsyda.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynmohcwa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hpiigkrn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fzonsujk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ickyjvnv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3pmjqvbyq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qzwpxqnc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zhbeoeyu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vkpnrnal.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3waketpfp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ycwaljax.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aosggjsd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ectkstze.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3spnyyyiw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wdganxyc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rhehewej.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zopzlkpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbftbvyc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jvniuyaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bumrghhc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3gzyrvtrq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qwjdyyex.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3svfsyjls.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfgwnzto.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcgrsbsk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tinpgmzb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3afuwtemo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3sszaisty.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3uolkdnrm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3uxhmsktg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3peqodcig.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfvhfoim.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3axemsgtv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jbfhuncs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sphsfaig.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zycqelye.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3pdrrdwmp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yficuvfz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zhfekpwt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wsaedroe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ygfobnfh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yjonuvyg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fjhrdlrm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mdjdoffb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hiaafndf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jvjqcidn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vvonssfh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3stbnvcgv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hnjqctna.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqjjtssx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqfkayrq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bapxiqaj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3odkwreyd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhcqtqp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fdzqymqr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwhpwhzc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3kwmxzkkz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kizkhtyl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rpkeygce.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylfmbnbv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ujgekjsq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tooylcyf.html


<!-- 参考信息 -->