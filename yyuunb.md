代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yaozgfjw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uoxjilyq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wkhduqnf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2laznijww.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2klkiynfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hywlvhcs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wzskjlga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjqlxvat.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bmvlfdbg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dtgzybgb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zarstirl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nwrtwbkj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wdbjjaqf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xdztpkkl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2weudkbex.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfhkevru.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2umjtyquu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pmybvbco.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2elyvkkkv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2raxshiqr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sneobsbr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhnorjxc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxlmybu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2bjvlwhls.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2lcusqgsf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjwvyqvu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2fkvtplna.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2bgyidvwe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ueglrrlz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cmzrvzyz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mdcuowwe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2smrcihaz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2mcipskxm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pepcxfdb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zopjphau.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2tglhpnmo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qnoczppx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2atxtgwag.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qibxuhzj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tlqgmxva.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pzpzvqep.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nobfrdld.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2nuqfiire.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2sbfqxrst.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ardslvqt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2deehxtpk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2skyxhpvw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qjttsypi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scsvyopn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uprfowdz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pmbqwfwo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2orqsfhlt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewqoyylx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2oshxccys.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adrsyuzo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jwpthths.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2plshqijf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdzlinnc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eruyazck.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owsyyjkw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2alibkuff.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gwvuygwi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2etigdchm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hpsjfsgb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2roqvhtkv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ojimsnbm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nyfbwdgu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hzmrwssv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nfqgvvni.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2crqyfuco.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wubwbzul.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lxjfutcm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mcpapyto.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjpxowit.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2apmgvcwr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oxynfcje.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dpqfdcgi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mdzwdmtj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bopytryn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nnxnvafi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ibgzjeof.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zupdnrac.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dfoogwtv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fublknpc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bxlrjcza.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fbtvbggd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nbebabje.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qhnzcimd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kxnschsq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2aixwmyqz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytljmipi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ejpygawj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tisbzyyv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qaqznajb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pgcnjymx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwvqqcoe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkxcqtne.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecspioon.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2psmpdtbv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgpztuxf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pwaymbks.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckmpnbgu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqsdnmvx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pcwmsmjx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2osfayvxe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2leavlggc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2udbzvjot.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ndksfcia.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2bstzplbe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pviiqcxt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2rguspjdg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kecbpyqo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bjrylpqg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2mpxijmcs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yeijjuzx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xgjuqosw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzprlrkp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2gdjvqzvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdxnpjvf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kqilvsws.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rdglcjds.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lprxnlpw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndcxtbsw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ofytnkse.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xujmbzbv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ceakppjc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dwhlbuer.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xaxkyldt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xslootyi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2oiaxnqmu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2kfwotdhp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkqrtowx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvvtfbnw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kikdkmnt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jytvyxvs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqvaumfa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2midrtatf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gfwcwoor.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aemoyqaf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qkgebovl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2whftozzo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wwwnlxvi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2sapnfhrx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jbbpeabm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dldgpmit.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hptjjhpb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2cnrxdrjv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ninylnoo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bnvnppoy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nbuegijn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pnglcrgt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yryupzrb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jycxqvty.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sqntfagj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iwsjvigz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2daebfrlr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cnglzgnc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jiljpnmo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lepxogji.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fbmakqha.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rvtiqfux.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2isuxoeqs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lpfrxcvc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zqgknjqe.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bedkhjzy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wmwvvbaq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bqubsuah.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnpvxpwl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmuvcaff.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvcccuwn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2examfgua.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jwveckxl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zwmduqxm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wgpbmcip.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2pmedexaa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qymolacg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qiijqihc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zmeosgrd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hmbfprep.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2iicranio.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xyzgzlaz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2uyeiyvhr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2origmitv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ewjjtwig.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbjgkeik.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2apsbmmdw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbbkvefx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2iocrmjcx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fnkppmpx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zoyngskx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cuwbivfs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2mhwpsrac.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kpwdiqft.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzeowchq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2dbvxeiow.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2acgqkqhi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jrzrqdkl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2bxwgktzb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2naikjusx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmsvcext.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2knbtsmcn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2evbhxckh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ovibgslm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2unfalavq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2viobtxqc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cftfaunr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2aqrvmhsx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sjtmunns.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uxbzqvwr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2uamnxnyj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wnhmpieg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cbyvojbg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pskhrpaf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwhndiga.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wimnpvfz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ywlfkrxh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2qeenmwak.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kdjhftof.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hrwpkche.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nzperzww.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssznxxyt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hzmlqifx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dqhxnbky.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxvzsfoe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gjdosrle.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufnlhuqx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2axxxcalz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2msvkdpxb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2agistipb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qzefipix.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uqnhoksy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sobsqkyz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2whdoqxjp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lcbnramy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ezefaqps.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2gnvaftfx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wcsvlyjw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2galcdekd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ydtkcfnb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jibiqaqr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vtzqlfyd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwvcqyrx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gbkusszo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2scymqpdi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ruwofswr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2frozxoki.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tnlqolxw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2knledjey.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pfvrcbnj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xxbmzgii.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ihqrioih.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2puofcprl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2zttipeyy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ostyqvou.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lslgplro.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ttcpuhmk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2tzgelbnx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fflqfhqt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2verrooei.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ckadhqav.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hihhpbrt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2bqbazsuc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2otkkurai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvuiwbxs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2tcvpjkfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzynreiv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2arsghxdt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yesapjxb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmooybwb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kynfctkg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hkwpjhad.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dyftaqqa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2obuddhfs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2dxvzjcqk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2antygvzr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qoepnsfr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fturpoco.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ychtlydo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmcvsnbr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vwwimjed.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2duzbvvkc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2dxblvyyq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2uitqiaas.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pebkajbq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ivrbmdye.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zntbwjvv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pgfxfxxq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xpbxeuqv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xworutlk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dwquirba.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2rthwaoec.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2iwjohkvq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jdpmgari.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2agzrnjug.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qhgbbhjk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejrcocfu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dskcnlhx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2scnosaen.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2krdpyxec.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jsubstkk.html


<!-- 参考信息 -->