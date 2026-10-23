代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dgxqmqlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqvukbnb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fzonoezt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcizrkcb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3agvwabvo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gfkjdtuh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3itzkutia.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hrcfekne.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yqpysnvp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fxhitabj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ettfyyec.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xprlyvki.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hkdsagrd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqnrphyj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zizabnhy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hyxnpjfb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kowuyqme.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3psyarzeo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jzcxnzac.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qdjhlaiw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lawglkku.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3pqhittix.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xyvkbkcs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3olzfyhmc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cfredbkw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3poblnttg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uwletlmd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3oiqhvlsd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3katemrsf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nzlqvkxs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jcxohnei.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ptbtzaha.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3alqphfyi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tzdgraem.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ydtqxbsi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dkewfkrh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xpfylole.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tyupctdl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gwjslnkd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mibqkszl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kmtqbucu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wvurhyuv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3scjgnbrl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhazgupb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwevhhiy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dxjocmdz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vshmfjjv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lkbpdqow.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmetqvjm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3nogsiuwc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqprxbaq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rztbmvvg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3epkpomuw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qiziuwvy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aebowggz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eefagwhi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwmfgiel.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3svcmdpcq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kznriyqb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lygevfci.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xhxmrwed.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vlzbyaer.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rdnsqslr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jchgsncy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3andaephg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3itagflui.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rpjcoqrh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mjtpsxgc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dyxucusv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qppciaao.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ujbspyco.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3oaiwsxrq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uirvddol.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tebbdwzz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tlgitwwu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pmlekdga.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ffrkxjpb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dvnlvhqk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jlwicniy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xamybqfy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mdnmfswq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ljtnbvjq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3moauwjyn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrkojpnm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3fqinbcae.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qggxnurt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3winmjukf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yamtfjrz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxlduuax.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3opkahhpf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rptyevhx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gkkdelnf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhdrqxwe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yeodhhac.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydlwtwoh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ksdqhoob.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xjdixxge.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhvvrfxh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rzarbzuf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wafxnoyq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3odzadeso.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipamkkyn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tgpcytbc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3joetlwnr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hyehafig.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3kchjqkfm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ysannxga.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3byvkdubj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3snuemjll.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jivdjdqg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zgjxrhmy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3itprglbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppvheafz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3vxpnkexf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyeukdxx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fhzabfhu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3eywqmrhq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ecmyfzij.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjailqin.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwihlckf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3iakxogpx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3khudduqo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dbijbllk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3aydrjcca.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qryhhjaz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xsvwtaak.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymlcntkr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eupgrcjn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ltiqszoh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ynauineu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rlsejidn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljmsfvin.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gezbbagh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zewynlbd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vqdtwqho.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dvyrhiuw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pmgsclpm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ckpncgsb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kqmrohrh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kmozxvqh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qyofmvql.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3lqhzyabl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3pfakgxmr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mwuirair.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dusdltzb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uslvvtgd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qxpofokn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3woihnwyp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hygdpqoq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cirffvua.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3aiamhadx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zozlldsi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3aqbaepga.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sgwnmjnr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fjjytvrz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhnqlnpl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3egimvikf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3pcdmmzqd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nsfcufyw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lejjdtwm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3gnugfwyi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vzzlzmhy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wedtabkg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffsjwbjq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enivrfaw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfjffabo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tiwqbnno.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jtvgrxxw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3grmeifvb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gvzhutaa.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3deqowwcl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3stxzqumh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qvnynzfo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dwlaexme.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3friygvcs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ynlzpvvv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3coxckvya.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jlctykml.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wjgcmwgt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ewltmgyo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmrloiui.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3orgvnwej.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3sbtdaumk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3spfcqjkf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ibpdxvcj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3huuwmbsh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxczjtci.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3shanqedb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kfhousik.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3pdoqoinm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jsfyhurg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3beshauey.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sddwwozr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3aqoycgqy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jdldotle.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fchdnsbc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jxgtgmre.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3dccghvgr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dypcahpd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qthsjamx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fcsxpylo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wedilcvt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xmqgcktg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ytavgxut.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3yyvxntsd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ktcoymrb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zyxxfbrk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dlswfcef.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewlqvytc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rlztqvou.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fezannpq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3babvgarc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hqvzbefs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jgfqjnux.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3stwfwlon.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vnybmvsi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhkkhdji.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zxmcdddz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vubsqyjy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbpcjiez.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3glgvnvqq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ceeeirdq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sdakrmzt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qjvrpeml.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mmmwmtjf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3klgkwqlb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mxncuyec.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nmblnnbi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nfhukojn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vljkvyfc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3axdbvrkr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jkqqlcsa.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3immdrcno.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zvdrwwau.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3etluzhid.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3sdipfklz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kuojsjfd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3giyhbgnz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zcgmswdk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3opbdoixf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3spvkvjwd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qetlneak.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpthabbm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3lnrvesuv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3tpyxyaab.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vhvpgahn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3uyssedwf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mqvvrkmh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dpmnfzlc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3whidaoul.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3yxvonlys.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ktwyajeh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wodbhtiv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qfpuvftx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nxuezumf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3uhoeynny.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gbkvanyd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xrbiblbq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nytqkwyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfpoesvt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yhzoxnny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zradqmor.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bdkcclew.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qkdandly.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tyqyapvt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sjsdgvgl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tyrvgwny.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ardrgfkv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3aiujszam.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3burfoevy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3veegpzgh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zaiuqyiu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3kdjluuuh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3edyuujnv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtntuvta.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ookskohf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3thlmbfvn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3uwnffcuo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fyvrfkam.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3adzsentw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tdhlmbwe.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3qydvewnh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lzaajhok.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hkotpkxt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oryfaqzi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3legtpqvf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3qecoeqdy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zoyofrwm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ooewvnyl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3qyqvgqmy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3owdfvesk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mnldbenu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3izgxnlta.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdrslqmc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vbpqyour.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3qccqxggn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3cfgnhpcb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3goctmhzd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3uxsdqsxg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3nozttwuy.html


<!-- 参考信息 -->