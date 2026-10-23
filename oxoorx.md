代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oulxzxfn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cuzcqvqw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bbspvivm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jvzvpmqh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3efwstzxe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arqjdiod.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hnsrxiyu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3punrvbxs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zhdfbwch.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3erqrlyqu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xflwjbfw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xdbcfmxt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3imnutqyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aspltumi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fctzasqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkfhelyh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3joezvyrk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3fncyewnv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iqateunp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hwxdlcrj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fuqbtkkc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sjxciclv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3quzcxcba.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxajovof.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3egvcvrnm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezikjjiz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3webfxxxa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3bulrgghl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ximvyrzd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3givyhjvj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tfpwlhqm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kzhmapbb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3egmbyybz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgkvkuwu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3owydstot.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vwkvtima.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qjapyjzp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ttunxzig.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nseosljg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tyuntmtt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mviwitrm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rmmsrxbv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vxujxmhf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zzczzibu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uwamvjpi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jyzoxsmz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vijkhwzd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yxecqarg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3odxdrhgc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gjiuteid.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rhjhsbrw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xfsezynp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cjpkzxpt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3dibacidw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gdwhlqgy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikwgfwob.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tijheawm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ykzdmcwq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nyhcwygc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3skdpnwde.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ofomagpl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywhjfkpc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjkxpbla.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aohjhcrm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vceilgdv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3euvuwtcz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wndokror.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qiobqnqw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vkmvljyj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aulffhtk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cipogrhn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qtwrlgiv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fqfpucoo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3oehyqtmt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tbjzmrle.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3acnmgxjn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rhudzalx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vqodedor.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qmpijauk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zbiachjj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ucfgtvem.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gpffyqxw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3prbsnmcg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3looviypa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mouhnock.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3dluwbiuv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3pptdqjne.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lioyivtw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3gnzvrszf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spwxddda.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qwnvvpac.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jtsxxxbf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3otulando.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xwnbnfuz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hrzmlcqv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jlpzxlox.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wlqokoee.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3azcbqjyw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iisgpatb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qgwiaxgc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkocardu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uprnbkie.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3babfjver.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmadefba.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpxpvvkz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hguksots.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3inmphwdh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vivhmdjh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fxuvfagk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pboxtlnx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fapieuax.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vygcwjje.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3aosdtbnu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tupyvkhj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nimmiayd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zajovfun.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qvvxkpmx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ewxjufib.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tudolevr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zzdycrwi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3nxuzcpxc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3qtusplsi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3eipqrmvd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3woatsfio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnancnsl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3oegbxpxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuqjsgkn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pwqolcxq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3veoumoun.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3aclkxxxt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibnriige.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3aojuygae.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iatcagcg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zudutslx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qzfinccn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bfglmkfv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3reqlqseh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kpqgedsq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adfytodq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jiqljpwm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3eaxdqixe.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahlxsqgd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3srzqijgm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vyvsjkpu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qjhtqjwu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3uqrnssjx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ibiynego.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3imjmifjs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mnbgnxok.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3sruueoho.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tckfwvyb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3kgpcrfux.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nmledskt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ojqqznhe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mabtviqe.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rnmozlwj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uzhtxkzj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ygrrhlhm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tcrmrxxu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdofhlwv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rzuyyfjd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uvratuae.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kparaude.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uxivecti.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vuycncnv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wcriirxa.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ailxfkxr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sphxhvjn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wubvwrog.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jpwvamoc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rkdclukl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmuzlkxl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xblcamcr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rekcywae.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lubgqfbg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cdnscovs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tmglgkjy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3shanxnrq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qqujfafr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tzwrcjzv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3paxbezjv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gmffqfan.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3esgokyvq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lcksndao.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wwntrrdc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rxaaceir.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dsgkridi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hptnuvgl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yzllkaaf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vwnwewjo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kfddpezb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mxpxuduf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3exvinguc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxssyoce.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nfiouonr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzfspueu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pkuylhfg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3eamwwmwm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vwwlhqxc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3puuiatip.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vepvibnw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hecyyxdi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3hoexvthg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwxmilbz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixfexiww.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gmfbixoe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ipclvbpt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfliveqf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3popbuiij.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lkzyvzrn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xbskpdis.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tfmxvflg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zanbcmpr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3uhoxjnmh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xzffgvee.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ycjccuzk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3zqxyvtiv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cxmzhogy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3uuewzkdg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtzuyudz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpklxwyx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3safawlka.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwtawqrs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ldsmeyge.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3psfwfrix.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3smyvnwit.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rvlrkxjm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tpfguujn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlpdbipx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpdrtgju.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hzyahrcq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahvcvkba.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zoyqdadp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3prypdxuj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3stbzptjq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xtmlefsn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fxbshixr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wksfhcpj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cgawdgym.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ksdoxwor.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mkujliba.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3caqgervs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3npjbeiwd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ywxpijlr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fbvgzzyt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kfeufdgd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3siwojbiz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xxzqyjrv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ossiprvi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3gnzddoou.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3laoehllm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nvqjmjan.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3msqehpzp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gmxxuwnt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nvlpqfud.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjcqwpjd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ebxniteq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oorkwjaw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3fufuftdh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jcaaeori.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jahgikxp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zszmscoi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3trdqtbsb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hosgqiki.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rpmgvabh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3motnqfma.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lcjmgoma.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3rulcwffz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3gijuxkyh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ktlocvla.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tbscqblb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylxomjuj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kznkaybz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lubmpirn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3sjjtdxys.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3conipapj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyysmqqp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvgfeutc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cibhlszh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcucqeey.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cjaudqhk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vdvjlnws.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewcxxcbd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3yqmhwffv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ersiofzk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xeokgaxg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lmydmvmu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3attpwhxd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oyrgbfrc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tbdychtj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlcoclvx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3laxlcjpw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cjiifqam.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3evuxkqrv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ewxkqzgr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3feknzoqo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tsvrdffi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jltkeack.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3dltohziw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3vbepvyxc.html


<!-- 参考信息 -->