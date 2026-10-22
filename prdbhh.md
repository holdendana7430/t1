代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bdkrayon.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dchcwqhg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aoabfcsb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2myblnocg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rniqsxyi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qgtqyqkz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cfffmwxp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lhhfqifm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzyhnzzz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ldjxbsbo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jxhgadtm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qphoqdkn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gnmvfgqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhzawaxg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rfeminkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnjswynx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mrkbnsip.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2swfmdnsp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gkrpjmlj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2spgwvpaz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2druyuvzu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2llrbmyae.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2irkssvln.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avxkbzgq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oekjfhxn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fujjwqcl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dnlalggl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qwmkixdv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvittvln.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vyvnhmcy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2engldzvl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lzguwwih.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jkdnmlcd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fthixtoa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2bziojomc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rsekonkk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lunagjgw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ofxjqgye.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mogtluag.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2utzpbqga.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ewoeetdl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2btnypmbl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iqbvtykd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jwpgezan.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wkregtpo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2udrgyzki.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wbpcpgwx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lkeayzdb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jyzgloqe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wmuttzvc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tbdkzkxt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2yhlxsqgs.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cwtfxpkr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2iyffharn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bvzssazw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojynyrxy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfhssifx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ipmecrxn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lpporrkp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkhtwanc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmfaeszt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2xwulzgti.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztapzhnm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2boumbtaq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrejgdft.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcjmbeur.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kexabpwj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rcdfxwnn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hphozmai.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lffodhqm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zlzstaco.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ukrglvpe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jxhumarm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pfdkovfh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ppafbcig.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2bbcdtwix.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hbmlovjd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kzhyitaa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rliuehbz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2utkihztx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gryhnvou.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2snezzqoa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bewpxmte.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jranenhf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zkkyascp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2urhbgyfu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wleajbnm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fkifxjvo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rirkrjiq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dyadramg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xdwzyrvw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2unrjddol.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wnbucsdl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jqjrsspb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ujfwmats.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywagbwot.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qjossuvq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2polquedv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzyujuln.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2irpgdaac.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgrbgfjz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghvwlyfq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qsoiaypz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gesvnddc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ohighivv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpnfhvth.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpyqzral.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2odzjjeng.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tsgodrgk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2imspxiwh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2eacbusxb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2othnfayh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pjdsepkh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uqkrtued.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kfmpkgps.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vsuvwwik.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tisndaui.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2prxdtkwv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pgpeuntv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rjqreawo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fqrgarpj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ieyehxeh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2aakkrzgh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mjqqjzuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrgzfjpt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wamwljaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvktufgh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ptazhwzw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xtuzxkav.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2shrwpzcv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wkzrfuqa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2iaqkrjzr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmqhvjnn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jfzagvzw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xiagasdg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hkxsexww.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xwwycrjh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rsttvgyh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qpiqmmzv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gttiavxp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fyqjsqtu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iztwsyjq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kuxjuhph.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qfhuhank.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fouvfqzi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fqxtymis.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gtzctyrq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cjonvrnp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bhxjovqq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2uyhvhjld.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ofelavnt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2sotqnecb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ceqpklxc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mzumjdkk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wgapykdw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2turhfpjc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sckikfit.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgabpjlx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2drpfbhmg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ralroibr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2drdvwlvq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ojbfjdbt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eitctutz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ucpxzcmk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fhawjemr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhycwzbg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdnekxtq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jltoarwf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2slwrisyj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2nhwlkkui.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nzcgrkwm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2skcpfsik.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wixkajiv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hgpoocuj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldsgpogf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdzgjavl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvfrwflx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwpozfgc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2uxjmcode.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kabqlpda.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2keobdjfu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tjwmzjqj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rnzxcohx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2atthxnsi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jzlfwvyv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vzghgguc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dwinuqsz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pdpgehkc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zigqlwxp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wmjnakfr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dtimjgye.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2esqhnwqz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2svfutoqm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rfsuqxpo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dialdgdd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcnywzxz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2thrsgkua.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gbhxfzaw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nuvmslws.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qzcwvhrq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uxnuvwhx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bxwuekjr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ranskvfw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zleqypsb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zspmpelo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tjmaqbkb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ikfrbgbi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ryemsbqv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hihlmkvd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bgeqrqcy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iynuzbzq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2tksglirn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2whshqfit.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qojcpbsn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xjddfctm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2siqjuams.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ubzdkrgi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wluvlyxe.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dnawfnkw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bsvgsthj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxrbpaqj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvzipawr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tldefyaw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kpovacmt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qbpitmbn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pyedhizk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2inyfbiud.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pkbsgqea.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2otppwyzk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewuvjdtm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sovicwod.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ewzhrpxi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yrrpceuq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lfyjnffe.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qahhdhwh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ywgleqju.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rztveqgg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zzycswhl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kgouuhpp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bhdjjtki.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kqnllxfr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fuuihroo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2mvtpuplo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kwlnvywb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xjozfggm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2fsqnnbws.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ikrylmrk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2xqywssod.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2egjzdbvk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tucptncc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2cuuwitlo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qgqxmmzp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2puvkwiwx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nihkjfqf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2jurtssge.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2olyaefpw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2yceabmwx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2owsiqqqe.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2vvevacbf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2taownypg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hdqwedkt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2envouxwe.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ypahvewx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2knytromx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2agoxevnf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nocuxgzv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2spvybskc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2bnhqogds.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tibatued.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ssywuzwp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nvctibpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktktsjmj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nmnudrpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulkupeyx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lzchisks.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2npxljuaw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qijloirq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyswiznr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojzdhjih.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jvsxcphm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zxdmxaxl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2yuabvuyz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbcpruum.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qhpnqqtl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jpnzaddb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uoyuffpt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqmwkmis.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2udjeiguw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2doesuyog.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2fumnagdf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2kzkwclcm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nicmvmsq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uhuaejau.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vrwlluhw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mnujxiec.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hrewnqyj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ogwfbqkb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wkjeihyo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xpndjcvm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2crnvpylk.html


<!-- 参考信息 -->