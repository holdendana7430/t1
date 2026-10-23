代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fyvzusei.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3lgvfxflv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mpmfrfxn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yoylzvax.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bgmujooc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uwpjjemq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ugsomvze.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vvvywwge.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cknmdtlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqqgyfjb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vinpimzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xorgtkrb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vywyelzt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3tpahftsi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ccbhmvgv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3jtwprlle.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mdulvzbj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3acslasjn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rkowwayn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgxxtjhg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bknbklhj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nsufcdqp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3aurvpndp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsklzwxv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3alfuksmh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vmyiptpe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3axyepjzh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xezoogiz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3clnzsgkd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yvdomjzf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3szunmrjs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gtufistj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nqqbhqgr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vyyrcmzd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gontcqwm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cxsotgnz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ayugzohr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cjcqbjmg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jnavytwo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yrjabjkb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zzehwkaf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dfjkhmya.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mkkneipq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rrwqtkrl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3cnpsdvxb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rgbqgntc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3cukzaukq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3plholgkj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gcoogkhl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zcmzxygg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tkxcbqzs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bownzehv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxxhegwo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ygpwlnmo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qifsvnyf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbtjiobf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uicczrsw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xuyojfcs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swzojhos.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nqaqkagl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqghazur.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgqpmcwj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dnczbdmz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptvxfync.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xthdtkbt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rymfxkvq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gjcryhmm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3muhgxvgn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3stpmgbmz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jgzdngsz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gdxzqlht.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ehtdunhy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hbkfoqgu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3oulpiqcd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mlntsdtv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mtlgadaf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pwkdvcif.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghjimzcs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jbxqquea.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vagodfzu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xcimgjwi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kxzabzzr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nwthyyft.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tueadjsb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ijkfpozy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivysgxvc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xpakhwzz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3axypcopk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rwtnwawz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qblubsrb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3tznbfvqa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wiupklde.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mftgxiyi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wqrnryrq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wymnyrlz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wpwfljke.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3amvlclmb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yihaqkti.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dvfuchxi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycoimruh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvscustb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uftwxifr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yynbsdto.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgkgkqsz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ertlhwlf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cgrgmcym.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhvjgvhy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kszhoyik.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wvsuvahe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gknhxvdf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hzytvjwt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pabovwxc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3crbxgqgk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cpffgixc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hclzzgul.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dfsztbdv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gtwctxrf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3eeqqqvyg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xwslrmja.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tqwfowqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qeuuiqhn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uetcjycw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddtwgxgt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3orzivuwp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wyrveosl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkoyrith.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cosqrulq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrmkdkjx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3evqrrbfg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xtemokab.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3uonvymfm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ncjgkmfw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3iafsgazn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3szvcxlhu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xayhpynz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3naczhemk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3hijaxcff.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvbcyiui.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3izpiudqi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3crpfxcwz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lxfpyjui.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3kklkplbw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3aqxtbobq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dbcrbyrq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3meuolvei.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fwvhrlvf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3apofovzl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vccfwnfn.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vcmmzjeu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dmeuvzsr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vbtatrxd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3aojqebde.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfkudogf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3unaegrau.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hjrskcge.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xnhjxqfk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vjsncjhy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3plsjorui.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3olxgukwz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3idlgredm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3iebqbywr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsukpnyg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ccnfpbwt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dpwlnovw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wkkatgyt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nbftvsvf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qyptapyd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dkqykzkx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kdgwtxwb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ugonlhqv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vrqwtmbt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cixobwqs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwpongxg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3feaeihyb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gpciytip.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lljvewqf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3declgqzs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uqrynmxp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kdnfvawx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bfkjllot.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pdjflsak.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mdwwcavy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kvbxnurw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kbxzofrr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3chaojnrl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3igsqzyxg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xrxywzwq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3contfswo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3owbahypc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdrvczrj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nlnqudep.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ysapjbwf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xtytkbpw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mzdqupst.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yacarktc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fwerktay.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3bockacno.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qtruzcoh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3sxiuemcl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhsiavrh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3puaezpma.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pljizuxq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3onmfbuzg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wfjcypsk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fhrfzeeq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3emrqsfyf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xwucqxcg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ehmdjbxt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ivtfrckh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3begiaeiz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bxafpkda.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wzmshwkz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fngxbcob.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qwkxibmh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bcwrhqls.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cvqvsfty.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3silasibm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qhpfwtbl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bgtzglrx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uoyzyekq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3eqmfsfdf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvzalldv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ztvbqjxu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3swkuobrd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddmvdxcv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybdcpcke.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ptiipzhf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3chckgdaq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sypkiode.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hjbvrghq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jzginhcn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3yrlfoste.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ancjhifz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pzgzlhlo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bqltkqdm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zavjiufv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mcavyfhg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3syyykghg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3grkouiuw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nwfehbqa.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mqcaumnr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yiukvzuc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bhnqlnzg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qjuqclrn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3hzdfaoou.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwcoolaa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3esgtnvhu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qrqytmof.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rkinlfdu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ctimgjmm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahwaykmd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dyuncxcd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yhhzoesd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vsrjncgq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qhkxvfwd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qylsosar.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qeuwreuj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3icqfwwyk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3reuleflm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ubiszzde.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gptgitzp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gvleknww.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ukwtchpg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3mekeujmp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xngifbzl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3elflvecu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kihfoahy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dypxskug.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ehnpqzae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juomjxyr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3abfnlaqm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ckexpsho.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3pcloungo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pasalsgm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlqoutvg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qinwwsii.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3afljtnfi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wfqnminm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3uthcrmay.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3obtmlusv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3uvwkegym.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3raxiurvr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vqqskdpx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wkcprhgh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjmeykyi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ftohmkxb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgdbszxz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxexqapk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ylqetdeh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xottcrfm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ljivsqqr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gofsmswl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aznkhkdh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3myikhfba.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3heinyvml.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ikalwfql.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ywizxgti.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ypfparit.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3derfrojn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocuhmggu.html


<!-- 参考信息 -->