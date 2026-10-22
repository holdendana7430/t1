代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rgjkgqep.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mxporlvj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rapplnar.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vjkfykll.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jqbkwhml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsuntcce.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jplmwqjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvtuuttm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pnatlwvu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2phnkxjbo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sftcobbq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nrxmzpts.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bdyciaut.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bakbntch.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zpgisfda.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwyqgldi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vaboqnma.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2nquriuhm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dpxwvrgo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptdjtzna.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smxbibyj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bflrzqos.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tmkwmzzg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hyzyrubz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uapdbcjk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjlkjbcn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2yormxjcv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jtptwxja.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wajgbxtu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2piguvfms.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sevhwroo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2eliviyqx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2mfymtenh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gixmceue.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rczzrdgu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2sthtjeng.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ptqxwcxv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2yagoyoit.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jhdvwtzc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zpycmocw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2iggcctpu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2njsrzecd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2waemynbv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2khpsmeog.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jnbjwttz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xcvouwmw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2unifshhb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2exdiqnit.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ultbtotb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tprohnlr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2gxkopzvu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wfwdlhyy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdkibxew.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jpxyhyyp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzcnrext.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ckfqyoyp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcajyfaa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdwedval.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lznhgupd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nactocxz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sxodukkw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kdcnmzwj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2slwocppc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mmjrxlmp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nxfyckbk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2sxqshukx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lscqcspb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rauxswjp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2znzrrkjk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2busoggxi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ooxcabmj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zpbhxghw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2szqizmwk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pipfzcmt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wtjipwoi.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ceviofvq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2elkpfyoh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qeodvoaq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ylsedsxe.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fphlubdr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vrpofzpg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtjvuqoe.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dmxjrkor.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vpimrlkk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ypxrozbh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2smfaftha.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2owgawxfz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afiktegt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2fjxamkgz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vscjlwwt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gggylkbf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xyebaybq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gylbgrap.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kflajblt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kfbgvopf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2execxkdc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnzwmurj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ogwkyowo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmltmxgz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfkxhyrj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fltxjdmx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqqyvuqe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtvebzev.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mjaygxjc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vbkvpypa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxfiqsbd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2pjkiaahu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2wlziahwx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2yykuisxe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2juomblqa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2otjxusvv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ftbfeefz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cnzyahdl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pjgieabr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gmdwhorn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tpvigykd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imzmnilp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2tyfnudzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsvimvoh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rfnmsoyc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ozhprlme.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzxwmvtz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndpnbkug.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2smigpwvg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jybuhprs.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qcxphici.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2uyzgqhqq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2orkyuqck.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ewsyqtxq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2prlwxqes.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2msvoyncq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kanfhrnn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yhoezwtf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vamnpdze.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bzeiswka.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2djkzebjj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yjubcqrx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2usdaejox.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2elfldhzl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gnnhzzmy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2eozhajqp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ksxhqxog.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lzytzgaj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2iouwhfpb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ouiaqypu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jjoaxotv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ypgofduq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2luetayaq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pyxiqmhm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2spdxquao.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pbsqliod.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kbaopwhu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eekgbtbp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2clcksooc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2emxnemuy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zqfporiu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2klganjwr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmnevsdn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkwoeldm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtwxhxmy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2akiykfum.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2yafxyrko.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2tigvlmcy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2veigvpwf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qrealcau.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2cfreoznn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kawkzdey.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vblknber.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2buduxuwa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2itzjjkcc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jnzfmjfa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2etbkkush.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ppfzixdt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mvbfeome.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xzzxzjqq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gaoletqa.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rysiijnl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nwhjhdyr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ivethlot.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2oxarodwb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dosnkeko.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2uphrygja.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2eqyjnrde.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2buujnkcu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xwnzsyhm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbtxrrrc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwmoawvn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2swbkwpnj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wryawupd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2pwnspabz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2buhjjslq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xpgrefrb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2drevhmij.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nccwubpi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2obqbpkgy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdlfvoko.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nvczacmd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2cdnnwmhv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vesxigge.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqtlqzka.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2focmdshv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pvpifdtv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nbyphkka.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ydqmeuff.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2chczdhss.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dqmpxomo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jtrfmzak.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ypwlhatl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2omjcicdh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cdjymbsm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ucpzfvsh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2baqtiwsk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lbvpdvbr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zftukhdc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ximzztrm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nwcsdjps.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zcromfbj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hryvirva.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lnmdwdoe.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mxnoyqif.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuwhrlie.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wynjigyb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2krtvdfqg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vrdzmvgt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wpabxetj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2osebgsbj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jdtogihk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gczgznga.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zxbenvay.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nqgyadfc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mhpnrnow.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2awrwbepv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wwsxyzzp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2udjxsnow.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2fmvgaudc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vbytdqcf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2zparpwuh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2auhgjgeq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2swioxuif.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2msxgibrn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2dcbxbvzq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rqglzdgz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ysgtjnge.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fvefovoy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2rhybewoy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bzarppca.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2celhfegq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ozvmwxwb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lxricmgn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vbavnytf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lzjnfolu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2msupybdk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2evaviaax.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2issvqpwh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2pdkmlxbw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bbpuvura.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wasxviqa.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2drbfkbzd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ppnroajw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2lnnwnnke.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hijnexdo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qkmcrifu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ucvikaxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyfnfzyy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rszwrldz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfmiszlz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2hyjatvlh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ovopukcj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2npuqwtea.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2msrpwstq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yforlstu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuufphbu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cxnsuoqj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hyylxegk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gywqldhc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ybxrlwbc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2crpjdtzp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxtgxdes.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kgzxqgpk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gskkueqn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2igmxolpf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2foexgrxi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zvhdmgng.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vimzeggf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2eufkikbu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rmqknbou.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sssvmhqj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2itczkpdr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yrprjbjx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yeqyjilo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2omqdbexr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2leguqptc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sfpyxpep.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhqlirlu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mvnzxatg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bfaywaxd.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bermtwld.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2eczppbbs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbqspxpv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2kkvphonv.html


<!-- 参考信息 -->