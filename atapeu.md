代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ajuenzpw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fjscguao.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rtfxsvgo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ccrobpmv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zdiujbnh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fbypxyim.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xgbxymnw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dlkzicfb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2slspkqhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dipqcihg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hpqgpynk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyduvwnw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjqhyalr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bsoxyero.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2umuswsio.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nghyyrob.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cjhprutu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xhypjonr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ikcjkzug.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iikchiqq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oxltgjfw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2yefogngc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2enutaiae.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2npoxlkif.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxxmcdbc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqtulodl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ntzhcnlp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ykccdoaj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gmcjznot.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2umgrkjfq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2brebfgbo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xkfljveh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wrzmuuom.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ghrfyiti.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lqgvxazu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2amdtcjqk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pbghqrhu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gqyfnpfo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ytbwdowa.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqzuvsjb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wfdsnadt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2qjqwynux.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mhicoyhs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hbklwlov.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2imocijkh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2indkpqxi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2quqisjiq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2djwqxcpt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cmyoaogh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2kakbohoy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oqitxyqb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pphehzyf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzqccljh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qcgbaadh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rbtxfryz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wprihatj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vogxqjik.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2recrzdln.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqyzuerk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2abtjxzuk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghwrkiza.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2szfxsixi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xszfjgsy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yoxdyaoa.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjyzjxbf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lhspycun.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tkrpypmh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wnnlbxdd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2oggnrgdh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dsxcnrct.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wmzzhiji.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zfectbsc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wjvrvwsy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kxcotxax.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2cqxuodxl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2osfdnyrb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mxkqdvgk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2uzhdqyvw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wwpgeivv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2izuwhfrq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qlkawnog.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tyzztfof.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hxiyavuf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gptszubh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dsrodxfg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzmoifgo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mcouoxwc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pwslqqdn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cxexrnpd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tubksoyq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bvywukbi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iipcoswz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wwsiftmw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zjrqxlld.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2diwdzlle.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ccuhcnep.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2auhagqfh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdjcvkye.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wrvqebsu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iizwnckn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qryytven.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edhpmpyr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2edqxojfh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uljqnnee.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ngscwdbt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctxvflyh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmkuhdzq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rrerxvrt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lwakflfd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbwbyqpm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2otnavojv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2oagaiuyi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2cnczdeov.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pnxcroud.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ckvlssle.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lnkkubat.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ynmrtrkd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kugfxqfy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2quhumxkr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ezrynbdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdcnxwyc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2weijhbdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgbgkdhj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vcskwplk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rtlgafoo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rrgichmg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kxbjucou.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uzhslxml.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2fkoyrgas.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lodxfgyj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ozqskgce.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kwofafgm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aggrwurw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ahehyeyn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cbctducm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iosukksp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2illxoykv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwgkxptc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2hrjkncfs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wukxqabd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2whsvodbk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pwezkwfa.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ftdfpphw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qkchovcn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jjakzeee.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ufnqmfhz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bhxqqexr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2byiyathn.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2troulixo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tgyznwhv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vwnaaeuf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2urrhhped.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpdasuvi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sbtngadr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzefjeqz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsuwrcwe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dziivkrx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ytfvwzje.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fsvebsxl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2dxnqxclv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bxtngjob.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilvrugun.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hslksygp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sglbkftk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2okqofcij.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2duovcvde.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcrkwgro.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2uftaphfh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tazywnjn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vahygsgt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whkfhtem.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2idjmtbqw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jalzwrzv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fwcbfall.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qbeeufcb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ygvccyaj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ekvqgtzb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lptgiuez.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wnxjcvma.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2cianjftn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ppyetaoo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wbokaeaj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lyuvelar.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2msgqirpb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2epqkztvy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ftxeerwg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2gmgbevdu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2owgmteve.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vwnjeyfm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdepttuh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2sfcyvsnk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdplqudn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cbyrdvab.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mcydkxba.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2owpmkdls.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tiecwgoa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2slequxyv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2takxtxec.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2titfnhbb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fhtiiehn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vbhralfa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nkwkofip.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ghngwbpq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2selctecg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2epmzbmqv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2usvcxisb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ildleach.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2czcklpyf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gywxswky.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ibeochcv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xwgaexnf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cqmbspak.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2aamzifrj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ffokghuz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wfbjseju.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adtracsj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ohfbtzfj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qffauwpt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndjbpqet.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xistsewu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kicdylhk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ethzgepl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yevqhxwf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lpbnmwcd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2shwzbzej.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ivlyfiij.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2beuhpofn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewxcnqwl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jcwyksmn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ktxendfo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ljtulcuc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jfkwwvrs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2gzygstbe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ecqpyzzb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tfxntduq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eltpmpbx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kdbiient.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2uidcpdgk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gwobcsby.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rwazepzv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qfdvqlzt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pjicanyz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dbwibmiv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2dccudtbi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vldflvgi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2afysagim.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ncjoshda.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2pdpfosnd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kzwspnef.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2blkjzldl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xiwwsmor.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2woqdcbeo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ezymlwng.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yaibjooj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwlrfxk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mwuyhxcg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2teyafzjb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwkfdvwi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lzonlhpq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qanvsrhd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2guxhlobx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jcelfhrv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xsimfbzz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ilwzcqed.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2icutyiyl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yfzfgyck.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zlrnunmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqmlfqob.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lqaialmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpicxdce.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2pfcgvqlq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2szosiuby.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eebxflgg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nhsxjpmi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcjwfpin.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pzalpqxi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mewhcmqx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldhbznpv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2iumfhsof.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2bhhqmief.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xbyzbzbr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wcuusjcr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jeebwwhi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2thdsojeu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhxkhzgl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ozkmauiz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2hcqfrrye.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jnjrhtrq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2asgqppmy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2tjcuvmdl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nwpjfkrs.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rggvyoiv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xihggriu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ucpwqqkk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jpybefyy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2diuojden.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2feujlelr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hlauwxjm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dekgsagc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wstyujsq.html


<!-- 参考信息 -->