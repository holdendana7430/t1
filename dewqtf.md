代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cbkqolnq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rzcxdyjy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yneprqvx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3npuswnhr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lgvrhurj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcduqyvo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wztuclgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zieusryu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ofgznfzo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3daskfndg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3isuszhgk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ybpnoldp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hvjgprcy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3regsvzbd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3yyolersh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdpborow.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fexzgeys.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3aqktlvkk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ghkrfadu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oksuakwv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tomhuuds.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxhwtpxa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hmnqfuhq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tbzxvwpw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3mvvfenha.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3luahjvbs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3psunfmij.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3djpnozqt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fimtbcdg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ocukskvu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3efshtfkd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xymvraoq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3irrxfeas.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3purixkfn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hsdyekfv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cbadkuqw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qdkhgokn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ckrbsfpd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ukgymobt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jrwjebqf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mtlidddt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3urshcflr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3otgxovbq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qphmaxnn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3suvpyfke.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qwuwbhim.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3deaatnnq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxadukox.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnbfukop.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tqbmaxcq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3omvvrhdk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mivxwujv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3scijoham.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ihckbfpj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpmknkhn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rrzexnaq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xveatfkx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nsahwcym.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3edyebmiz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3akokxwhj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ssjlddou.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jlgmhrzn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3orsnkwes.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3idrsbyay.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kvahkmik.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qpsluyuu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gafmamet.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jzxlacav.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3syqpgfih.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hjpaanuv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3eqwvuyqd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3kuvjdkat.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lxekaosl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rmopvctl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kqpdfzoi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3unqfheka.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3txbsqrcs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gqbjchtq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kvfucubm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tzpuwppw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dgnmisii.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chbiokzy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fqmconvs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hkweagco.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tahhvosf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hihwgaov.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xrzjeuau.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhqdawba.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3cvjlxtmj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3brmvecyu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3byqcfxrc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jwllekvz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gedcuoem.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fipwgcer.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3aiqkzowz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awaiwzdu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvuyzqgd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udwshbaa.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cumnulfi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pfomwqzn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nvilarkf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzsidsyw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahentsuz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pfmmxgdp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3afkyglkb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzgawpls.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3quwvmfdg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3korkidlw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jtubbpgh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3kwzcpskd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jjzwgtgi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3exixlobd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kpdhgamq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3uqudfwte.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3uphgzgwf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rqyapgzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfrbfeyg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cfnucxmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgcacmts.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mcuvyhqm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3korjvbtr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zdumrhvg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vehnjsxd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yptauych.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3mcbpvsmk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3mujoqbtu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3indoqddq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3axvjcftf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ppglvezs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ieupuxrg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3cbzvhyrd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xpvqbobs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gvyskzyj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ebeiujpe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ildgbjqr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fekfveip.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ezpydilo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jcupgxxr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ajmwbiog.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vdztwbzj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hbkxgcus.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oypuwqmf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bfthesgv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3copuomez.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lzzzmtxm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oeurslli.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3abqcjtdh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wirlypli.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3krtviiuo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oooyspgr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3izkxszsj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wkahtzct.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ghskuayl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3icspjcwi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mwpibkza.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3psknygjv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3afvfqkfo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zvjdwluc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3efuztfls.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pywupkez.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gqlwldzf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3esjcgvwr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dczregvc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pqbpncqy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3myoaquhf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3eqfxgwjg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ycyvzymd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoohwqir.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3midtavfu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rxnqxgfd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3kivhmbew.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hilgveca.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3axgkophp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3voodapvp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wwqdfsda.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3urvcyqxc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3afhzvgto.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lazdfojh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hmslkuvv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3tbmlukfe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vuampdvg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lqueusgf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ffnwukvv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wdvfqspj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bgquttzn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gseoruqi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bubghldh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qixvzllv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3whhlnbud.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3atujrgcq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dtrqvqjk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fajmmixt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3azajqztx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjccfncb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jzsigcds.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvqafkrp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wvkckbdg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3oibuzqxb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wrkustre.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3begbdhjf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rvjlwydc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ertapknw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xzttdzlu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cgtsdsgg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aspqatjd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3rykskejv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pqojpxwa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bizfwhcd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3oyiciiir.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3prckbzis.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kvbcpbld.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eoczpatg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fnzaxhng.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wtntihej.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hzrggyyb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3szweandg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yagrbidf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbznwpfk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lpxysqfc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yvbboyzt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqqmtnnj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zxcpfrvn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mimyrasz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkujkdiy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oniuqjyb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fhozyjqn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fbawdfgz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ekaaffva.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3odijftdr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yrxvsyfx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ukpxbbdo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zgojfaap.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bihznxqn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jtxbwoit.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gerdnezv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pjkbwmlu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fhansxjc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3iprskdvg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ofchbxmg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3dekbmlsc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qjixsfbe.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyiccgru.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kegzbuof.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hjfzrjlr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vtmuujhv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dzcnfqns.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wrnfqrmm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bjcmoltr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ywslxsfs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3reoyqaeb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qnwyptse.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3djlocirl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mjvsxhsl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qpkmzcil.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ruysrecr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3vdmlppsg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wlwexvsz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jmzgaqes.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zjbrgvwp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xdlbusfk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qxcorkun.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hefoyutm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jnwbhqqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehhhjypi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xgrwvptp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dunzffft.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dqemvota.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vndeibsd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zztkedwk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgfbudia.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpfgsluf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdehcgzu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rodbepuz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ibncyega.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3zqfhibtn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3gbrqbibq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xzsbhmss.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntxwvboi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nbrufmjc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ouvgmywd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugeiwkhc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ozrsxqws.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3bimqkjqv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxjultwy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3glojelya.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3cgoxrlae.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xyvvravt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rxwfpesc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qjfmupcw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3luyiyjgr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3nzbzovoi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ysgxsofb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aljyqdfr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3eqkdavfs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fqedyhnu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3evnbuwdr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yixtgdez.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3reqjnill.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yrzfsnux.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3kuiwwuzj.html


<!-- 参考信息 -->