代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dvxavylx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijblsqar.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rnhrkjgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzwutrky.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dkkaxvzc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rxngmctz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sfhmhybj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2eapddovt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2evvrkyts.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ksjsypgz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2eyhtokmj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hsnlcrjf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lczhbdok.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vocxbftr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qtdidbbx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2azhfagpl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nevohgjh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvxhrrti.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2crtqijml.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gzyyfftk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rngyqtpr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2sxqahxco.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jkxbcdbu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vpugqszg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jvnribwo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zihzuegg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2edhtafxb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zknvgbsc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2zuzibknw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ovgxpcjc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mqyphrsh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2dvroctpt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vxrsqwks.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2lpnzcdeb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gtnylhsb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qqukvzfx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pxofpuek.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jkzsxowf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hoxhcdvi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qljipxjt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jbdjuzpw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2pysnitzb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2egyhcbbl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odkpqnwk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnkdxaik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qmmcsxvj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2goktzika.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azhjqgex.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfjzqsff.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lsbgegfg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qetgwcmd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fgydsbxp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vsmfrjjc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcuyozca.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eiezvjoo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hrgguzlx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ridyfcst.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2antlbzzd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kotzgaph.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dmknaclk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jlhznbdc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qjpwemrl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qcdisrxy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2thnpqabu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2cwterlgo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2snzyzhff.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pbsuqhqw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2irxwyajc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kgrpgjjr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixmtwcdm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xkuuwbcx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2prbmfmzy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vvisloyl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dlqacskt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tloryico.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bkjnpdem.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tzdfczje.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjelmpdj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iovjcofr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2chwugqfx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pyhkuaeg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2unzhcngg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2iwrusnfa.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oywxneex.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gsgvowkq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gtcmfdqm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hlygscwl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2agduqzvf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hiesadlz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjfclwpr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qrrupofe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2detyftgq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dyqraehy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jirvlzbv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kemdaibv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukyxfpsq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2brgmikug.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2regctykn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jfiicbwe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lalzolte.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ypweepdd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2afuzitgg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2svxclmsd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2evatnboo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ewayslbg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fuprdokf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dobfjsde.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ftfptind.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tmmkqcow.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wcyoanje.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wetebalu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uzcetfgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxahxujn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2urwneibn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chpkzoet.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ekxgxzlf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2efdhuvvo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpzsngcc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2znimzool.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnksoanw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2sjcklgae.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pqrqszgs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xqwsjhmu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yppyabfb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2osoadvsb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qwpbezqn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2yxnzpkwi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmgvpqix.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ywgyjxwo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcbyhrto.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2eueqjtde.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2klykbjzw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nefrceqb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pqdfmyev.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tdmwtpfh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fhtmbkpo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wtiihcok.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2uyymbduh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2itenaoad.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qtfkdoao.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wgfpqpyv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2asumkujf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2lvprubkd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fryeppgx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2napgncet.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kspuwjim.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqfllwkp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvylmcgk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cnjtbrcg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pslmpyal.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ouqfculw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ufzrmday.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rvyauqra.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2epzincdm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvzjgpqx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2goaoqaxu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2buwzyiey.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ajhpncer.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nxhqrgkw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zuyudlxd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mshilaqp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hxzkymra.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pofwhpth.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfwnwmuw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrvaniqd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rgvznsjb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wvyuwnrs.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2czovfybo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vbensaxi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ijdvkrtf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vzluzele.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2orydapac.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wekdcbwy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2imkipbra.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2flohpepl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2acolhjaw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qmqwdjfd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zivjgumd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zkomrnmj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ttwlusll.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsmqbfsc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mmtusqlc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qvverwra.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwqtsbbg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xtkpsgwx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xsreaxlk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vrhijboj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2uuqysfij.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2whhxhjrr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jxkpxmcr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nhhislqs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxeyjnaa.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtmwkicn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ogduphmj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2lfeyhpcc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2sloqhrfc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2byfvceeq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zmqkxidu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pnqbcqix.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lceaxwoc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fdbjlike.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fuwmitiq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lvenpbrp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fofkyglk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pcsytwqt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dfehcjqn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gbtjkfrf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wunwvwvg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eycivooh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nohdgujs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2btxwdzzi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2usxdgikh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2twexlddf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxefxmul.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dppfrkwu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wbzotymk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axxxcduo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2unisufnl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mgqvxzqp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2baoxwdvu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mzhkupdn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pzqkgryg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fbnklizg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ouaumtyj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ipkemqgu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mjlecmxz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qujbvmtk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wvpghmfr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ypgirldp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2kasrtzvp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2mkrrcfca.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vkjophsy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2shujzjjc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ykbyajjc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ffvthwjc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2gzdaqaie.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mgevnhgu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqssigxa.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tntmzccq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2atwzdfuj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2rxkslrna.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fvrhinnv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2appufbkp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gwydhqhf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lgqfryzv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dfcvcyrp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rtrylspg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2lurtlkct.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ofihciqj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dgwmiduc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2gngvaxjc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2eokbjejm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2plkxzyme.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pfofecqs.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nixwrxdc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kxeafmpn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2spxdxulr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2toeyumuf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tbeqaswh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbukumgi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wicfugbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omfogbfa.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lcdohife.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gucakpxc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2brkunueb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbllotin.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrsavixg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhpblsvv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2wtnxkcfk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2rvkdimsz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qylykmvv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hklnqgsl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ingsrvei.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sdzpcyux.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpoptuwa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2izpcqxwa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djhkxndh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xxffuvyp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2iiplgddy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfvaudxb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tuoytzyc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2afrrxjwn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2omuvmctv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2znmwoxzi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2toduaidg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jcitfxhp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2agoxehoo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2lgwtpmwe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ozpkgjls.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2eblirbzs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fhmzqwtr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbqlnhme.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kulijnmu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhsrrnud.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2yeruydjd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2degxwfqf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2cbdmqaeh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebtreamq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2mtshqvlc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2rkapcnzt.html


<!-- 参考信息 -->