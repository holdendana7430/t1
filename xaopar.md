代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qkxgtjqw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhjuvser.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rbebtmqk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tcfycljj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2irrqtiad.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2okpobevs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cyovevob.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2inweavaj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tuqklzgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hooycnxm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mravfajo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncncbbbc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqtjemkx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ghtapdpy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rsgrbfpo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2kdfpqnvn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qgajpscp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xxjjswqo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2uwqksqir.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2neutpoyg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ntiqoeou.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2eosbpbja.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2evltoyvr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kkqihkat.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mrnaboyy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gctrykqi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ztogrnsf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2khloduyi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kkustfpa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2aafrocwj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tldfvelq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ykkstcsx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ojjsrssv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tabaztkh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aaclznty.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hmhltabp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2uofatmxe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jtiqhqnt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vliaptpt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjbfdazi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zeufzglm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2flhbscoe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cvqbkmln.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tltuoxjz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2iomafrok.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uhdigldy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dligdfka.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2spcvjvyb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nqqtupsv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2shjthxdm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2decetqwf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmodguxs.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipepqfxq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pwilquuz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rodycyxx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqqjtdge.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2swxkomdv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2fqslhoql.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pedudblq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pqsoemqp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylgykute.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tutzjehj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mqpthtgx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocjrkodk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmedyskg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nynexfxl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vgmirxzb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2prqlkily.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nazvziwb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aflmpdsp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jwzelnel.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bsaxjadl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2kvgxsxdj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xtgldupe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hhkgstko.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ajkbvupd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vihsguzs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckmdiafq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yetpaalv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yfyhjkdc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xudnecsy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2emenobpk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2eocaysor.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lclbjfnl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jxokuosc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qiahrgrn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmrhqvxw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ngpvuomg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zbdqtbqh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dqpafrlx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2bhcsrzji.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxtcsygw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ahlbjmkr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2laygixxl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhjdzkji.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xjjhouoj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2odnexpnu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qycmrahh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dfrwdogp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxtjyifg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilhfwhcl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmndfrwi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2stfuozjd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxvrancm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zjnoyktb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jmjfsvxj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atlgiutg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pxcfqgtt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2eivmjeex.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsqylpgn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2smxyeqha.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2yrzrhunz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xekkchom.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2efomxrhh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kngldjuu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vajczlbl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2znrsglut.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ynuxsekw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2lyqxgeqz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tvdkkble.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulbmcqpy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jxmagdrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eydnqfxn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2obqjoayt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qmzxdmoq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eovyamkh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojpbgfxo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2idpeupay.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2udegbkdc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xiwfoocj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2khndjuoz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmmydsqh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kmxksfsi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2stniygwx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2eliyekma.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kxsduyvf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwklkrhf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljyjcokt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2szthxtwl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2iqtufkql.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjhhznaa.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xgdblqbd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ratdzaly.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fbwzjkii.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gcpgkcsx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2klqpspyo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uahaqxyi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2cehcqlyn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2iegebywz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2psbynquh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wspadrlh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uhvmbxog.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaqyukhf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpvsdlrp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jmjdxhmn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bscpwybk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nibeeoky.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijygifkp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kwfotuuv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2easmuqeb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2flymaplm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lqfzyxxu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lxnjxbtc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbtkobsq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogyhwhtm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xzuxvrds.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ruhjaegw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2thnmfkzl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qthxojlc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2urqwdysj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrwkeqkm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jtwrbgna.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2quvqyjco.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqkeevqk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bfiszijx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xjkbegjo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wzdkvzqh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fsjesbzx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qazknhra.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pckegjep.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2phnnnzld.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cubwmwzo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kmmjgmih.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ujjhimov.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hkhzituy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wkcsjbeo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ldfwjhdj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fwcsjnnz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2aqgwhqcs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2pqgekagj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xmsrbvdh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xhyamodb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ychdnmxu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrbxpibi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rpshlvtu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2yvofmpwr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2cxoykejx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2uwtphlhl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2noyuvnlz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2xfgicpnu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2igsbeknu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2zsqgkqjo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2znnhivjw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2btsdatks.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2worlaytn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2yvtnvtmc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fytaewao.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2syvidola.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xghvczag.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2htvcmkrl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ztryuvcb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rjkszqdj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ijxeqngs.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2kdeiwnmu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2reecnoip.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjvzjlpq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2atyvvkdb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmvfmxyz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rwvegabp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vrhbdoap.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zvkqprmn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2neybpwlj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cyalmkse.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vtxoapmk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgbnevgp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqqyyypj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfpffzes.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zjftsivg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mgysyvsf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbflyocm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pjwamwkl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2buwvorrm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2mdovisko.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ebgfoidm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2crijseks.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fssdeeqf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jbhvtaeb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2unegdiro.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2iapnhjjf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cpsyzwxw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nydmizib.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ntuplqmf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mjpcevof.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jlgcqodo.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qraylmvh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vckekkbe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ucekzqpj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xjkkqdvb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2hxtfpkcs.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hwchlrqa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ybexpqsl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcbvgkfj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hmfokxhi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kwprcmqe.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2smlraxjj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ngubgrrq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2znxmslwr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pznbkllx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xdsiifok.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2zeummsxs.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2yabmhwtw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jksqlqjm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kzvuvist.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2avdeedqe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2dasrbuwj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2sostxvgv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2owxjlpud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmzfvzog.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ndnqwgib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqyqelwq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bkeuuvly.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2amukoait.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2yzjcjmsv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2edvejjij.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2emmytljx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2oxdmvanr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2emligxqh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2tjdbsfgv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzuigsel.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2swimngoh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2kitkeoap.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2atkerasy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2spijuose.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cyhggloi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2frjeocag.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jywvjeuy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2yfxvziqe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zgmwzddu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2swqdpxcf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tptjavvi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lldihoqd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ppluraoz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wgejndca.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ctgjwioo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zvurzuzs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2knojimtk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rpkkxjla.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2lkdgjput.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2knnhvixb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2iazzrgum.html


<!-- 参考信息 -->