代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ehtuvvwn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sjkfpphx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hbiswpxp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3diuhvtnf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ijtwnbxv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gwyzgahk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bddzbbfm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3glnwuvah.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3tivjnxtn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fuqsbnyj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yflkijqj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aiwhyvap.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3chauejok.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bkwydlnt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hkgipeks.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ekzdushy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vdwlhyhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkwtyadh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pnpssrqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkuyxlvb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jyimgxbi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3eosrjasg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onkqmags.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3zmmqadev.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iwpoovpi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hpbqguqf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hxlsamvn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmxdmuzd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ixrcnhrc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fbsrnnpm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3kqjlzfui.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbxdshxr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcjocktl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3excusucy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3djgigbsq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3rjijtquq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tuzatdan.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pltlaibz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3sambnqwf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3scerdllr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xxmpfeli.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tchekpwy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3aqbtobdw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iwuridpx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hgopymsv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zszpszbm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ayyjetdf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bquhnboa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3llbwivki.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gejjxryl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gvirhgvx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3redtmjfm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fylktclw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zaqqwuge.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3smkgqwmj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qnrjaium.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vihyejku.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3uaxjrlon.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3whulfxgb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pthtrbcj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ziqnigtx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oczqddrl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wlhpczqn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mcpbybfo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfcjzvjc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3uwybfhiv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffruefnk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hjrqlfhj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbgurxxs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddtcohae.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ioinlucw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emiwctnj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tuqjhmwl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sjxprond.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xwbwaqqm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3joeobsyz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qfnvuhlu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zjdudkqc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ihtoiclc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ufzkgitp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3bwafekrh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zpolugkq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rnpzokmw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wacqqumr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lkiuxbxn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnvkwrax.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qpswqmle.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bzdnzbyw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aznupsau.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ioovfmts.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3twldyztg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zszvuepl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sbxwtwvg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cdpfcexn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3adlnigmm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wqeanfos.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pvyralvh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lcimzpgu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zxubmwef.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3byyanlvl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3abinrcru.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nxqlbvuh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxcwnrld.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jrufrkdz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wohntgns.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oaisgurl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3onswprno.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3srllkmgd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgyunmia.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crfkacyv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3odxccaim.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehyvtuva.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kprmzhyi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjqxdkvj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnqybdfh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jlfgvfbw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3udcvwdya.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlajnion.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ngkrtzda.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vbfeyjoa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3huynafbo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rwfcuspl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mmmmofau.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3icjsgfuq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hbavfpsx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lmiruzjh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bevsbcqn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fvynnegg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mczwqpkv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wdgsksie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbrazvbq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ouwdonzk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3kpbdcjee.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3phuegnqt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jshxlonb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjlgbeaj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocgybsee.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3eyozzldo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gokojhao.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3drktxhvk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xsjuijyi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wzofdxty.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zdyptgoz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3umqxecsc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3iandjrqq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mopdbcye.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3voqxjcbu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3jiqbpthx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjlkwqhk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fyjcubrr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pomevqcg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3efvjdiab.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aqcrtdxp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zmmaxygx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cazfckig.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3svbvsguy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lwftyhxc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uavkrjvc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mlrshyju.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ujwrdpxs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lnohrdse.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oibtfeeh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fboyxvor.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3htukllcr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3monzcnbb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iormcpqo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lkrhochk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zcdkmiph.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gnelrfqt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ovvadtij.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpbzgeii.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsvbhhqv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxzmaulo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zecwspdz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dalvsinn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyfylmvq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jqgvagzf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3iexesyyr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmejjlke.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ozszkdwr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sexlkhmg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrwvdztb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3iptgnofk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bsgmszei.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xlhlgfuo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3unmdukkp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yfrcvdad.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jteeqhds.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nqpldmlp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3irzzkbre.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xpvmdmsi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3aalugjlx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3taxuaxhb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hawhdmkp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pdkwuova.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wmflqcqs.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrnicmqa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3csdtsxen.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhonvvax.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3syghqbvn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mhdtpstp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dfgyjzmn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3skyztboe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jsymzwxd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3amkygwor.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vdwjyphi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hdxmjpit.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wdhzftko.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zxkthgub.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3sauxqulc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3moedysyz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ffyhovvp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gkvoyfyi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lvzvkdoo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eepedcdo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3thvqdiap.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hulazmdb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3pvarheyr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3uytcxkzo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xfnfuzzl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3iyzjwkib.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qvaohzhs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gqjpmsvx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3avdsdpmj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwwxvgmr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3axznrjhq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3famlpziv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pyfutkxu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3axbhguts.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3nolupozg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3maxpcekk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zdrmvnyc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jljpmmyq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzuhvntx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fztclcws.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aejuzgbh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fejaigmg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wpduljsb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uxvitpvn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hncjelmd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ejozvanv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3segqaeqv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3drfxvfit.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ekkzyucc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rhdxptvk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fnhqyrhi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3tlxbmkvt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xmcnwjgu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qpdksdbh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ssbmajsu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tdwqvbfa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3izhukutw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vjsxeliz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3puvemdlr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3sypywxex.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vyutdnmz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3uniuraox.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nrhyqpjm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nbfkckjp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3exgldymp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zouugwtq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nzeyfdyy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ygaxkhwc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3osdslqau.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jyitbmkk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jvyurhhe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3erhztyjt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3mlezlusr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hpitsomj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tfobahcc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xacyncvt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fkisfsaf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3oyormfla.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mdgxlitx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gajwrqhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwpdptyj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tqopjuls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aebuyyah.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mpkqaqzs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3suevskix.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhkmwvmt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xybivour.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qymweagv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3uzdyjbou.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gzocxqmo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jmmzldtn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwtzikas.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3isajmrcg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3whjfzvqa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qiefwfkx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zodkjkeu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmnlsfez.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gojyhfya.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bstulrld.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3nfcvfbai.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3njeqietc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mtgrxzwh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3vnocjkqi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ukxwqgfe.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dyoxgohq.html


<!-- 参考信息 -->