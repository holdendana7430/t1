代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfhzxlor.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2niciesjr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjjprauu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2iqnbtdux.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nzbrqzso.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2amwumdnf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vbvwbypf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wtrewjho.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rkcwcpev.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ucoafnui.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fboppijp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zqnjjiak.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2epbpvvvh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cjtrxryj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nrdskjqx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nqhdermt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hphsrdmg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zfiasgil.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2devqwedz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uvokbidh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ctpmumop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wiymolvz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fbdszhxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxgoazsg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2sorxolti.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mggytbes.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tqotkcyi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2cgywpctu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tjkzizep.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rnymrlhp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fmaymbfd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trssdeka.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jkqpbvwm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lrquzemt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zmzampfg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uxpivdjo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yyaqjlsd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyttddcl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vvphsozy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zlzibwmo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2eypbpjrk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gdcxswzm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2yfdsiqhu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xryabwim.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2llhrnqri.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ayayykhe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fqkqyvam.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jjoeqygg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rtktnkco.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hdamopon.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2adlcdyft.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2svrjmjwp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wmzbqdcm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zzijylfz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2awhisecp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vzkbcfqk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgqsytl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jjufdxxq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qjzuldcx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zpsohybq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zjacfxit.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vfrkngmr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rotrdboc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fyiabymo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgolijwc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uydbbqtq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2kxndkqup.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vlxqysau.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nvmflxeu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2akzpfiuk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zysxercv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iqghhtwg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lulkhqyq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjsnwjci.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qifjsasg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzkqxuey.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dfvyolzb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cqfngiav.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bsbfmmrt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dvamoljy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pgbvywbb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ckczpemj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gkauhoqu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fcqoedxl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2kfxlabzn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jwfmsnha.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xourygyu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iuyqweyx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2igbsbcnm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jnfuocis.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ydijtblq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iumvqoge.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wznmfyea.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2daiqqoff.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2cflamvhj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wzqjzryr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2exvxpiky.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsmokbxy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vkofrsal.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2umdefvuv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qscquvvo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bhzxoink.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eglfmmzo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujoxwvmm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fjhsqlys.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2crbwlcnh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cxqlgnsl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kkojoglu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmbdiifl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbfzlymq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xihkixes.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igeucbks.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jopgsemw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbbhmbva.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qmivhmoi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmshpkzx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lhypfbsz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnutvzfb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zymrqezm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhlsiaf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ifcmzxae.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcrdffwi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2yhdtwspg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ohkhmkej.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2pfmafjhf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qofubydb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qdzbvusr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jzcffiwm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2npokgldg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2huobbsbh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ibtomrsy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2pkmcpnji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npczvrtp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mnijkqxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyvmzgkd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gwkwisuz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iepcvija.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2meycyhyc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ziuuoxhy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dptzecri.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wesvuhzf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2iykdwwkq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2envarlpz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qupisksl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kybdsobh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2cliaqcda.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykeyjggx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjnounrl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mljgnuip.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wmuwddwp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rvgstpnj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wobhnozw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlcycicz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pajswvkk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fobrbtec.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vvajvvaj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mywluvcu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2itcvdfte.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qkrkvbla.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ipbrguoy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uatxhixq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tsnjdfau.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2kvqbxxmj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xiqkfkma.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vwxjixam.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wphegcel.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lzkcspjy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypjzylcz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lmrjicgx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qystvbcg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jxerayhy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bkdvcvnb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2llnmkmpw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbdzyihe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2aljjvqiy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ehegpnau.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2thzvqaqt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hlytcawy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2avklaven.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2vudhprvk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2owbrnrcp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2iomsvugz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wxfuzyyr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uecwccbz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzumygqc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwsejunw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2daszntdj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijdqvdje.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2axsmsipw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jrxnwpaz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mvhphqze.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cwjyjdhc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2abhzkjdu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gterffuv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vavczbir.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ronuangk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2glqbaqge.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mhieanuc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pezxyvks.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yxigmirj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkjkwbuk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zrbmpthg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2oplkjgum.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2esjytyle.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bkooefhi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lbedequg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2njjxredy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hvrvtlmb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2irhvmhus.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2batwfpja.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2tlvotccj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ycccyffi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2cqtipgxv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jachzcuq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2lqgdlmoc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqgogfsu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2dobujjmk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fdjgvhbm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ddxqcuff.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jefmmpkp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2izwethrs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2giqhfvcr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fzcycxan.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dljplbot.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dpbbhhoh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2gzhqqucn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2phtrlpkg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fjotcbty.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2armyesxg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urkfsbqt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kwocmldg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2idfixfot.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mqhiuhmo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fedirqxi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fkistnlv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2krcivtff.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzslpwzg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oxaegyxr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzqfyttu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2snliruht.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jhucfydm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cqamuqge.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cayzxfqe.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2uybteznx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xildklbr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eisjsnln.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gnyqaswk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nuifkavq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yrfopqci.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jtagjjbg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2llobojyj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2alpplvkw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2zigovtmc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mbqdimjm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2txsueoec.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jbtbmjng.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2uxnnmbzq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2sndpjrhw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ygkywnzp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jxgczctz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tryktksf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pooqbsju.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uimdhzzc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ikzxexhi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rnvzqafs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zlrakncx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ejboymgn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfmbope.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wmkqtiup.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2iijvfard.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2cqfdqmwr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2indotrqz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2coyfbdiw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hetnatdf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2twrixsxj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2yqcjxqbh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jcfmokib.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2grlgkkxt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gezsldbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adznsbhr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gymksede.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmmmosse.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jwimgeio.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tzlqsrkr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvghrmhy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2guuliubg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghuwssbq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2cxvijrpp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ozvqngma.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vwstixoi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jqfpckts.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wtezgeaz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ihxuymzz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpfoprqh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xictkpzv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tizhndwl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pttqoaup.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2uvxxpvtg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xaciqxku.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lvizailc.html


<!-- 参考信息 -->