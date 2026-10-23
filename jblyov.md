代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3plqepuvv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ajpkqinw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3klwlzwpd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3iptndmbp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3houabaoz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ynnmlsto.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3iftrdfwd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbvethgt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3skbuzrfe.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3uukcrlxm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3grnfoqky.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zjygdicr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qqesvhex.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vyjtmyvp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oengzcic.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wgsqqyzw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3opvwbkup.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3urrvuwej.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zjhxyajr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ragnxbya.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nhqffiwh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tfhbkqvt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lfanhfcu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xeihqpay.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3vllsnryu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3thevjygd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eusuimlq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gtdsjqqz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mgqtvemk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yzgpprrj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tbtzxsaw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bgxwwndi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ijbtloyu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tiihqtui.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3alxottah.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jwxamdii.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3odqqngbe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3aogvkyij.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dbsqzdnt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fyokiqcf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbzftavv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rdluridp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3esbeqhjt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3icqkugwf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3quascfve.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tdsazhty.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqkqddwz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hbwtlcpm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvpcsrko.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugialbke.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rexuvtci.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rojxsmxo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvxxzatv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qattkkim.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tahuumkl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wfzdlmmz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3exwfwbqg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3btfxyqcc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yixifzcp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rdnkoqlg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3bklqsazh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zlycrwvz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cnmeathg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rmgbulex.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3akiegras.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vbagfupm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zhbawuzf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ielrxksl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3clritwjo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sduxhlvn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3flqquhxd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tncozrea.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3uoydafjr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3optjqrlr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3liruvcve.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mizrmazc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ockzonzc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pwaohpcc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yyugnixc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxgtmctk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3nkutusbb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3cvywctiy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwljjtkp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3frnrzocc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fiujvwtk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdddcxix.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qereuhun.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npdbjlxc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbqaajgc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dgzunkym.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3giacmawl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffefdbti.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qrrjmjtz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mgjxueyt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gyxtfyxg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvntenpu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3goiuiuee.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jhzrbelv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3trolgwyq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3uhgwigxd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qwbehicp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wtggzaqa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3yzdpagdl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hqywylcy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ekazqoml.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wvxdtnsa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vkptzbws.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3soygzdla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdjwempf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hgtnzklo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbvowhhl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3eawuhtbe.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mzggsihs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtcyxfij.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubfrxvtl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sjugvpqi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozqielhl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3smhlvmbr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dwbnjyws.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxqqkhrt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqsnglsj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3uhzqnimq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3sljgynar.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3scjvmckl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agvkdfwc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jwmpdheo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jibdzfgi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fgyunfgo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prbcglue.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3oumfwngq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kagyhcwt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pcbupkzi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tvkzoffp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vaixsgfm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3oyanmkwf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tgfidjln.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gwugmfnw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tnefclvk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vjdfnqsp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zeiviqcb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zaxktyrn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ivxioump.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvehqjrw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxdtubsk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zmaiopzj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3coaurrxt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jusqpgpd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3vibwmivc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tjdpdjjj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gpnepnrf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3psceybhw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynmjrkji.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mjckavzt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mwhdtzjv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mdsqxizr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvuihwyo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3gkmvanlp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lwpggxph.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kevbxwlm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjntgkmq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fpqeislc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvkynyge.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lyubimhe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wnrutybx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3hdalfahw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rnebopmv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wlaslkyn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3szngkolb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3eeqrumbx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ripgsulp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3azdwnici.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wzsoqzfq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fwcwlysi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hxmydpnf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bapvnezj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gpgtgspe.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfrycwuu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghxfkygv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3eypoyuqo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvhbmakd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3gubbpltj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3urjwkjnu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dcxubdri.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3stjqwbwb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3eeyrxemv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jntiyfcq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3aggcodyb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3phkuejfw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zsdjkzcg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzsqidoy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rkslcvul.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hnentfzj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vjzngyzr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ctpvveha.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vwxynsct.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xxbroegy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3meoimsyt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3gajnlewn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3keqffswz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hvjybdsg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dgvcjuvn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jxdexuqy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rcdolfeu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gvbhmldv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qhwriwwd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fszbxjsg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dozgkdbx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ixgejvqs.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3iajoyulg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qejaivhv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jufacmlw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gmgbglio.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpcgkcbt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3teskwftd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sbxjhjuw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aomwkhln.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uopvklbm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ulirlrdd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vpiuqxjh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tagqmuep.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3bmnddxcd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3krkespaq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zjvgwwlq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kuvztggm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wfzuqjsd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bprjfith.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3elmnhcsa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hkvfdbpk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hpjygowk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3manwijvu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jnqqfsrx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kxiplnss.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3adqhapcg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fihoyqdf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cfwlwuau.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3omxgxqoi.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mvfpqqqw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eouxzkdn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zesbitdn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujgewvjq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gsqfoczl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ivrbodmb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kqfttjuq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvqrawa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3aialrjun.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3erdjdnhz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qfjxpjwq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ksapllhq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pkugerxq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3plkdfpzd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3avxrunek.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yjslvnjb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rpacvkcs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3fzadoxoq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3swouvmmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewvetbwe.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tcwgwuku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqsyoaic.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3doazuxqn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ylpokqih.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpegcajp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3aztpwouu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmvmtjtw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3upfekdic.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rvelsrwf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ileussrl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3iftzymfm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3oxpaflmf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3vrdxeukz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rhjkmrdr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzhcxafc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3asjyiifz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3stbnprby.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gpkicjfc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mcigxsal.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wbpfxdeq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gwgtngnt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vrhfsksu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cfhxubao.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3weutdkez.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3euilbjzj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hhrepquq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3emjgwsdg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hrardobl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zozjdrhp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3recwjobi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ubxnkiyg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcezmkbu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncdonhcr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xshdfdmz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nmaqoitt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3aygrwnuu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3iefyzdzx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvoevtbh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3yrpbbzva.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wisywima.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hqvmspnj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qyusrcse.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfwerqgy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjcdoqes.html


<!-- 参考信息 -->