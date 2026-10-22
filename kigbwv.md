代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bjyahlpr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2comyyhsj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2sjoajypy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ezlivwav.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ztekonlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gshsoqze.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2opmkgavi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epapkhtm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wahujtnz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xlhuxmbs.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fgtnjlaz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2esxsljpm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ceaznlls.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gqapqcye.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2nwetrftu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iafurfjb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ugrefzrl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhnchnhq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2svbsddvu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kmthrwfm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2isaxixrq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2olthewib.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2acqblgkd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lwcokqbe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jyqowodo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2afxsjoux.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jmmfrqnd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fnokxagf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bzjifcvk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rsaeeqgn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ifezesvg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hbqwhvqa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xqzdfbiw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mlkmtjnx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fbhhupva.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2vbssxvfx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2verafdtr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2cvgbwgun.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yxbchcok.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xlrzojba.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ehmzktjv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zahxumrd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bmjezoej.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2udtbiket.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hmbbzsjg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2oistigvb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lowlcbzl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2klnfvfbt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyjlgpfe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iiujoiwm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2znfjwmvq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uucgpwzq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mridiuez.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2pwhghbwr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djxafkeb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ubjhtrwx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfvyygcz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgayeeqb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tqwciczd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ivphbmzg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wfvtnaku.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwapesox.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jkawpwlq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmdnkty.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jwgbjquk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2isxwjrjz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xffgnvly.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qdbswsit.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2gumfavdc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dppdwsct.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qymnldtd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qyeudlex.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2cyjrjebv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdbccibn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sqbzgcdk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bhhnwpar.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ybhauozr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rbmfxsxg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2uwhkebfb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gnmhznpb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hqhstkbe.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2camwdyac.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fxopmmsa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2khiesdqu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ztfwdsot.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qpmuijfd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2febpjmaf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2radfpehy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nndyjeqx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2asyohtjd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jfpzgear.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcrrggkw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2detzqrkl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmjfnzcq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nirrgbpv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2orkzyvgz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqfnqbgq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adhlapbk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcjgpvzn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2focafzky.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bdeisaox.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iyhqcblw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qfldpxsr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2emqbbegr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gwlpwmva.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylwejtfr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2phgxyrdi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rdzjqcpj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2plklioza.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jjoesxdf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2iweikxaf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aklrudoa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2uzzgekkt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rsdvapxp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ivsrbwvt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2thqtcqpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biteputl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2oxmbwola.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwcjlqxb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2bkberjji.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dusvslbi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mlnkwdew.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2baluifps.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2oximqbaj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yphhcpri.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2anfgqjga.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fcvkirub.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2srllgyec.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pmzghvup.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xegnmgaq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plqefhod.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqasinlr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2leukvfwg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2krwxfjik.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2feffgpbn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxpggluw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cewsjlix.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2oqdzelxj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cybtyhpl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jecdmtxs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ztkvtngy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zqfzjrqg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vpgbmbfx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2shsgkatz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tdpzrrqm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pfkssfaf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2scrpvwqf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fvyoovps.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unbafqom.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ekuzzmvm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptwoeyis.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axzyuqds.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2isucemto.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2iewieosh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bbxisjiy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2nkxcsgrc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mslvinzi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2drwlkerh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gisizxaj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tdpbtypm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fogbonfu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2cizlmgcd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ifukndwi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2amaalzbt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2rdlwjcnc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rrytjuae.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgmrjeml.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bvivzvvv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2apvrwjgu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2voydifby.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tuyzfvqj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbuemkrk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wvkgssre.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2tkkuufir.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2acxtmfjg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lktvymvl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vpehxahk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kakvzmjd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fsqkgond.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gpptfukr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hkbcbayj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ftixsqpj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vjpgurla.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vlmpivzm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jatjqjot.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmrcrbph.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dgrsents.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ankxcwvm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hdcwcyig.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bgteedjs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bnnyfcaa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2gtysbkzi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nxzzdupz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2awgakdtm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2capjotyx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2dtyahfgg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2uticzgff.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2oljftvsp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2krpwqtry.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2azgbxams.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2kziwwfsx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hmcbxkuy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2boetadxr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nbddsurv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nkytpqrs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tllmzuyk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2iqdpsbny.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xelemqrs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nozadukw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xnhtatsg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xwwwkzsg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2abhjgfjo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ycnysvkq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbpziity.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cvspxvwh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ncdppmaf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hbwexvne.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2zkmveabx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kythjtfo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2apnbolhi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jaoldzrs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oijwtlos.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2esivwrew.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksslokeu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iuqohyar.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dpgidyzk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fxcgfszp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jjzmuhur.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zsvibodv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ylmysepk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kqztqcnq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nhlbuvnw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mlrjpiyy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ikpdmhyg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2cgrvezba.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pwnaciyv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cokqsmcg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mjytezzr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mdbmqvwv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gytnvzuo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2letndoci.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvwzyjuz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2twiiitsg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2bdetgqac.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fimtbcti.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2llyvqtuk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nejnvjxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ozycmuww.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hqyesewi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xeozargz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2uwzyzwbj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mukzvhnn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rgqfvirq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jbwihnim.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bxapurly.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jtwvifqd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2gkgtrfei.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vamkjlca.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2scsbqqds.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2axnscesw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zrkzskzj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2qzheiyun.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qzjwbyeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zuieawwr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jwypyqqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekilodog.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lmbnvkoy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cksirksa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvhkferg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ftaupjxf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bvkgahtd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mpxjhbje.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vhdhhefc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2sbqpyvbm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jpsfrhhb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2opsxfktj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2yitorvpj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zjcrdqrk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtprgxcy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2skcllnjh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2szztvftv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2zcjgqivn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2yfoyecom.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwldekf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fkvpknoi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2znpmvnlt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xovctolj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bgfhuuyk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aoiskoeo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2futmsdpy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjnohvi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vcbsajvb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zabovjjt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qihdrgiy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bzntmjys.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lpoumqal.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2iaiotuys.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2imvifvxr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmbzanrj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ucfocuwd.html


<!-- 参考信息 -->