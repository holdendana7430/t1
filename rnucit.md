代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nhtdxzlb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3upfkqbph.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kycoozwy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3syxgcaeo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ihawofqt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fwdhppnk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kimkgnxv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uawviaui.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gqrprltr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3homeziva.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ppxyeftq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzblliib.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3efggasrg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dntwxxlq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dupcdumb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ynyjtmty.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xvdbmajt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cazhqqcc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lbxphlrn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iemuaybv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tgvyqgis.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3slbqwqjw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qjznnjiu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufbrqzwz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jberctnc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tacgixva.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fgcbhfbv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hwkslvsi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wfedqmxf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqtewnpi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3blbqhslt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rdhbwwkv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nppyajnt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mxbrexbw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kqfdaraq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3inlwrabw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rbhbbjgu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vcibraum.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mxlbtubc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jafqycnj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3axxfmxfs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vzqrzmdd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3eeojaafk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bupucoim.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ugeiegcs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kbirtopa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3tmdmruah.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3apjoqpwp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jnvjqsmh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jguprvaj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nerwhbjx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkfaphgs.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqhsvkig.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vdpwntbe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wdpcelkq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmthjfhs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngkfvejj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtsatsox.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tdjfeldy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vivdpkde.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdxowspt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxqdbujm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qukmuoaj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgbahsdq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvvdmdsz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ipqiwdla.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dgcumjsy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ufybeeko.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3exhanoyb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yqgaymit.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pszivbyi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ujjrvhzc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vmdwaytu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3espfsjkk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qmhkvriv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3borfyzkd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jcuhlerc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tkqrchey.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cnrzoimg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3afgkdbwd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hkfgjcuh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lgqwazrd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3owxxotnb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ocbwrmfz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cfsfdtlx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmyokubw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qluhajkz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ogpnfoxh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zusddbeo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ouqdpbeo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3iwmabltj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjzqqxdm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wlfstvvk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3uniemtwx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cikayswc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ltwhyjko.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogcdyvai.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nucgnmrf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qqdoiyak.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkenaaao.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxymgxsf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3demwbycw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3echzgozf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oucpwbsv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qtxmiftk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouhvsvje.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3statvwux.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3igporlfw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bbrreexr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qymgmsvp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3knxwigxi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3voabufqd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3urorczsb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zixrgicz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bpdrrndc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qzcugmtt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wndvjpfl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xkrntpna.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3igipnuro.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3evgkmeld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxlaruco.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3nnozndjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzznyslt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3shhhiile.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3govezzlf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzflrjld.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vltlcndv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3frkvxqqi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3twvayjfk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ahnvkxqc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oiluzhom.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3stzdodqq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3siluzcrl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zkmzemuz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovlrsylv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3thiwzxhx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3peounlnq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylaplcbv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wyztczkf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kklkucyi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlrmgcse.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3fsfddcft.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fbogsfbl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cxewywbr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sjtcnajv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ccxsjzrb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3excngnyz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3iohapxbu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rbntsyqu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3erqbsjak.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3psvqbwwb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3njhyatqd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjyhqjmz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gksyhyuw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixuswppu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuqybiao.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cirbaknk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3roaolosk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3maqpevof.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pbtdznoh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nhitanlr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lezmvqup.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqkrpsrr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3naxbypco.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3khmpkxgr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ghcykass.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lenpmvaj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3movxczlo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3sittxwuu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wxttyqam.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gfwzwmim.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxcyaaqv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqgpsxcm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fnwmgnuu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3uqquvgzi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jmbbwoas.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wrlbrwuq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tunbliid.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3mmtaoejb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qorzkjxm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3meyvycjz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yjmkgbov.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3grfpjfly.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mtsrfizl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fcvxizoq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cmsxhujb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rrbkrbmb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jyrxnlaw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nipmyunc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdasjcas.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gglrxrne.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjpitlhw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pjpbtphj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3stzxxyzj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cafnsfeg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3iimslblx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zqfkcqij.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjcmblra.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3nsjlpczd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3sfflbzox.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3srhuwltl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3nvwkwuhi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pqtqhsrn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dlylrbhk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yxzbdvqr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kkusvzrv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iattitfc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dtrxwiqc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vsfcvmxs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qmjjdjzz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jezaaadr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3waswpcgu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nuguhgol.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3aecgxryc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3uiodrdli.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iimjwwvi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dddppsry.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pgptcnyj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uwgwopfc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oosngpeo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3nwbxkwpn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zgyqonfh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gbroxysu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dmuqvtgk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyvbeddl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3luhzpwqh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pyufhgws.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3llxtqcto.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3keekwibn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ijnblbcr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cldwqrff.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ndlupdvs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ntpkmmlu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sgtvhrrj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rqcfghxw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qqutftfe.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3djmtzpba.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3murloeub.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mpbzsoid.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3nrdqsjia.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zcxzvnzh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ybgzfypy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pscwrhze.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nxevpqya.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3okzxpymj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fcelrpww.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ndqxzaec.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3erqfwcdf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3yvttqheu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jgdethkv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3reojilat.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3chqypuoo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vkjggksh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uvhezwgd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vnjezetx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3gpbjcbrr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xhxlgddk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vzfjhicj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ygkunsul.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mxkmwhii.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3decfgktu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nvijdsmf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gjncllrx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hialqkww.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3buvuglep.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jbdvpvwc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bggrorgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypeuoibm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qaufkxak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsgzngoc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3uufcgcea.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3eswxysqb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tyjbjvtu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dodxeipz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yfjoqmsy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtymcfcy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xhifbfsu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lqcddvut.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3uxcmpuog.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rwlkvakg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gcezujgo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jjttrogs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cbuczjuu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aoyusgss.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xxooslry.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rmdpxaon.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uwllpflm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3soedhvia.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3atuhjnwj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lvuvczny.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pqdenqfe.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tvllrshl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xmmforad.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hwxaynni.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3pzcpfuyj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ldiyiumw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yueonrvw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zpvevnbp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ccgpdlen.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jtnwyzgl.html


<!-- 参考信息 -->