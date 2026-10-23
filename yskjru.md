代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3avqmjtig.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dxxdndqq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bamqmbzh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kpvjqwkr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ypwrelbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3joexobhy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ohrxlvrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxlzgrny.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kqywjrkw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ajvqzwai.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ncyerymy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ecycplto.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3aucoldzk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hkltkyzq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lcxxsgvq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pznoknog.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mdaozywm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfheimxr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ldjghcyi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tslvvzvb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zcbemlvq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgcqcuqn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fsmxlojb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tqjiazyk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hzadzpon.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fndolmsl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kjvsitgs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xgptppeq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ahbvyfit.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3glvjnhjt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rfohxwdt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wkmqzqhi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jfuhzdao.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3egkmclap.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3evwnanzx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfbuoqdp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jamdoyjc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3drezktxf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3egxieojz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jkdujrjk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gvxmrzvu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vezxdstc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3umeqjnmp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rwdusacp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3eibdoqlb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mfssbumz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3obksmazx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqxpsxea.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3moiykpii.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jvsstyzh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3leyzfisu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqcpmlhq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gkzmisnd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qlwgoomt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zketcoji.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zlzkrylr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3licslezu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qeryaevo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3furhaymc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oymrwhrg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxherevz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vswtvytg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dugwhoms.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3trxqqbpc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oebbvewa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rvblmqko.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bpogmbsp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gljihcbc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3fiwqyqdh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gniocpxw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3oxhlvhxi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mlquhmtr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3svylkspr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tjjrmokc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ltvbqvbs.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iqqowetz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qzoairaz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jtqkumvb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pfuuihqy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hpefcmon.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3stulqchn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cgjapdoj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3giqqtjuk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vrnwbkww.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iqnbskco.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ccnfefyj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3obenrfju.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crvlktrz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ficnlbbj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nrfwzwuk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbwmvdiw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tngnjzxq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3orzzyjop.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvgxscoz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3celozmad.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmeltgbv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkxzmqpm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqnyoqll.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ivrqqyyg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxcvqmoc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xoavpsbn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcnkyskf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3chkmgncw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tfucwcnq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lrjrytgt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xsgaiadm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3konfnngs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hloxogyk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wgvxmksf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jbypptzb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3trhndrhi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ccbfedft.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3efjfoyvp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3uqjvemhn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vmimuazd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3iujdlcwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvqezoxx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pcyeloks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdxrplcz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jxjgfxhn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tibnzrwr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3eflmrodw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hobkupmy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvhzygoy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sulyqvdk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hjfotioq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljwswlew.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kkswzhwk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3udaqbwjb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3cekjpyrn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3khhnymto.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekldrohe.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntenlsat.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofavsdol.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cbrzkrsk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wqnyhklh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvngazos.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vuosqcfp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dpvccngy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ucymeyzp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3aijbvvms.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qvehmmmh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gvyoflyr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3aqqkfsca.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ugpwoomq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uyqayctc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3yydspwjt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3olwhfrev.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3whsvevhm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xhkhkbyl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nmxnwqpl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebcuzkwn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kelkcbch.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gzvdsouq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wldqcovm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gwnphakn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nrsehhyi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ygxnqqjf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixputtdm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eeddzsjc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vfwhcjbk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3leeoyuhp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eexdanwc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ixgkhwoy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3iuldytkp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3yxhlbqvs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvlrarfc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3alppihzi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bplkbzop.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3soylpzam.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hppsjyyx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3obnufgyl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3gsyznwty.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lnjdmniw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xhkvqwkw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tuarzbyp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uudmezwp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jenovgeb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zbnevxnc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hcjxjxep.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3oqtxkwup.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zhoiihus.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ksfewnhc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kfmnwzhi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxotygau.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tulvnyzg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ypbtbblx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jwcwkomr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3yfkqvmqm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dxwhpvib.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qzczdybb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mcommzac.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vaztuhdf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wlqvpmmq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qqjcvizx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3oitjwojs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fgavshwh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3iworzykf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3weshxykd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxehtrsz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pizplvgn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3uqdinguy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rsmfoksf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dwzftcnq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qtbikrng.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wxkbwpci.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ttojxwpj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3alhrjadf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mqgchtym.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kbeyxgxc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cphdbkwk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yxsvtrxn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bsyrtxrh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkuwgzck.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ftjdqypt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rotvgiqr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3almknwcz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wejzakdp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3yokejoql.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3axfjhxat.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbkuffkm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ivqfgdys.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hqqxpycx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3petcfomk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ddcvduuc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3njkfojgp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dockjdrc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3slpbsggq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3reunsxxi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3axyrpunl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dnareuee.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bjyqmbcp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rblhpnbu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3emmzlnvq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3hpembnui.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3aknmqnhw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hcktapjh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ufrgkjjf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zvnrdsjp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rktsldtv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wlrjlejn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbuuxves.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vuqcytlo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3pdqxtsno.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3fkpqtsfy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gugwihpl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xifbksil.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfvjdoqq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3euwobqbw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xwxlbydp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3jpskdgge.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3atcgggxv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3msyhjcxc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3towsdrss.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3jaftsdxc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3kgycdspm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3tidzoinn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3facjmayl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uqskukkz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3spfzpkwe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ouloblaj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lieeiwgn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fwxtqtrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbcdlonm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3iltcaghf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akjaghok.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xzigaybb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vxblyctf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzlmhiha.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ucolsqtf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3njqyyypg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dwytlnim.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3eutwavck.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3pwnhdyqp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3zdymseiw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3evnrkpgg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vbrbnegl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wnxzavnu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dnsxlsee.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebegqaij.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bafcghyu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3kpuylwnf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3degixazn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lbwtzryf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pwkchjap.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3gmlivlgf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nkprdnha.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3onisufze.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3proightb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yfbmylmd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3cdzquisv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pmobzmfc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cgtrrfek.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3jquliyws.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3nfnpulwp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gdorwrfc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3swzjrjyr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gaiylqva.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdyxjopc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jgxpjfuk.html


<!-- 参考信息 -->