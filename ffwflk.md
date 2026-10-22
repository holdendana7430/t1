代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gfeykmgt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oevvghsk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2eaiidcdf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cwfcofyu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2totyzjoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgfqctkk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hcadwsvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekhgdoip.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hedoftbg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qeuvzilb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oycsgidg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xdpppczx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kkboteml.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ckttgyaz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vcbagzpr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnclywuq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dfiezigb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rotrcxar.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2oyfsdfep.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2nnovvjpt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvkpqnse.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atihmquo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vozeykkn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2pfclgctn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ljavyubo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tauugjxb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xvmnhpob.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2iuphgvre.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ksleslwb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mypnpshm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tfepjsar.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jopftrrw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rrntcwyw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ajowxlgf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tguagsby.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jvvqfsnl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ljnwkvho.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jbxvgpsl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xysauhrl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rldsfzjg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2jyjnwhcv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xeernwrz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bccavofe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pwcbixwl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xkbjduzb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2nepsydhg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nzsvwsds.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vkbflgio.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxrzkcpi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kqerezhj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tmeqfoaf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jthmvmdf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxumolmx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2evgbbngg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dovckmku.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2swhknany.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obgiufdl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkiroade.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nxuddsan.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eptmsgtw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lrbwwyam.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yojeofno.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hlthoqth.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yzojgmhp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ekqlwhqj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ricundlr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wecotsqo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qgehmppq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jecgcflx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2twjcvspq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2pnorhgzy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2riopghtp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2iiyccelj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hmarhvwx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tfuyeqrv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dqonjsey.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vbmapcro.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xopjmrul.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hlwbdgou.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2axombvht.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mbqeluuh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjtunerz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qraboure.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dyyjxoap.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tkbojnac.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nztbxatp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wcofnbra.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gamifqdm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hjjzrrab.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2izulfdcj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2efyhjrah.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vkybvhrx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kadzigzf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phrjnplc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rfnritde.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccmjptxa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzhuobyx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnmcrctq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2puedtnwp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozpjfeyk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qxxarzyh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vnmajgpb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oajwoqqn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jkyswcbb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wnrcdlzd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elwjwaon.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fqueprxg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fdfhvmns.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2othorlsd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2whdwrlyx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cluqwxmd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vofwlexp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gpzhdhjg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zimxfilu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2izakttas.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2xmpovyht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eblbcvdw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hmtiffll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iapmsiip.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fvhddmtb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vroarmmh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rbxmymug.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnwxibjy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ywkviuzg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmgeuabd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ajekrnbu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ltmiyjfq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmnudxvx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2dqqrfhik.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2tiadhkvn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngrqboni.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcivjtog.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cpjdrrsf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpoezsep.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2idvempdr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wwmnyrfh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfnerun.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vygmvzee.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fhuoadbt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pnzvzaiu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dioocmtz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aqwfuicz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wywyjkfd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2pnfvqoos.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yrndfnlo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hsjekexd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vioykbua.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zeccdgoo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nappjwcn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcnenyvi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrovylsd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqzghigb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wzbjcqta.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dtnqcefq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lxawxzqm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2clnpqgky.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mgbkuyaw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rjteqowp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2amqdfccy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyhpnqgi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vicaboew.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mrzqebjf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nkrnmyxv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rieaxork.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2brdnbixa.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mleijcut.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ofmqjsiu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ykhafats.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rocqzyht.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtwzjnvp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tfdgznwj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2nyuuqimi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hhnnvoon.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bukdhcui.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dhrzcfqx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bvfqurdw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2arrxvfiy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eiqicawq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mbngzabw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pqpxuwjn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hcflbsqf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zxdmsiem.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2llalilpu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xaekomsl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdcwrtov.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nubthafv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tptjapmd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sliblkvo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vgoyxyqp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2plfivgxf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mahnbawr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ubggohbu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2odiuqrlt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2wzzmbbdb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2rdfnitfq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcguxhbw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cthtyghb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dznpqqce.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gujnmjyj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgldnogn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2yhbaeewz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2othuxpcy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2owiddmin.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2etrnjxsh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2foauzeuy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rimihtfa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ujmogskp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2urlwpolm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2avouzugk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gculpijn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2fxgsried.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2puksrbpb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmltcymy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rfowcgft.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2libwhxlr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uddcfwem.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ngfmrguu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2djzdbery.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2epevjnwr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hzassikd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dywwlpgv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nhryeykg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2onethiio.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkaqtblg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vpusrrho.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jnbfzgdw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xamxdsns.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mthwaezf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mfvdkmff.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fbclnjhm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hiojvjwf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xcrxruoi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xbqljtnu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bzolwaar.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrxatnu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uemwrhxg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ekxpciej.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ktqyrzox.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qtsvufls.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hfxcrcbw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2jjepsyvd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shxyenez.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2nnbsbeaj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2eccmsewm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jzfjiijk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kcnkivix.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nlsuawty.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2plmgzyje.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2nymopfyn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tthtmvla.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2uqbfwhzg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2grbclqpd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hzdszcwz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tbitnutz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mvqneusy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2enocvohn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2mfvnokrv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zpoaevbb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ipkouexr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fdotsbxh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zneqnqgw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vaxjxdkq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rqsavgdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsoeikjo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2cpewfrft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftabvjoh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2rkmtkvyq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gmgdthql.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vluyuokg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqubzgai.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bhmsgwli.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fifuopiu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hdapvcce.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ebapnkbk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ixywoojj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ojedcsez.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tdwhmmox.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qofoeajt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqswgkgl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfkeuqsd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2seofeyqt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2anoylixy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2rrqnxxpp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwnycabh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2aozaxihf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ipemkslt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wbyvftko.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2umcfklyl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2loqfiodo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uthrbojt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2bjpdbvht.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2dlhtjpqi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lytzyokn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2xifmnfuv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2cavbmmyf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2klebbyrg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2oeucluxy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycwmdcfq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dcdwincc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2zysogssz.html


<!-- 参考信息 -->