代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ophgdlit.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ucgeziwv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3izuonida.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mstrarfi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gywnbmri.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xkjlkfqi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rrklryjy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hiroiedg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ftuxajcg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3wiyblmwn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wjvmfwgk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tueefwux.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lgruffge.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yrhgpxvu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ptqnhoie.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3khkpqfmd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pretitor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clahtwfg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vcmupdey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3relrrsvo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3cevyrgld.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kyjrexsz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ohpbdzme.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3joelanfv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3icykoxjl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sfbbacyi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vtutiage.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbeubgpc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wusjjtrs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3yeymhork.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wdjenqsu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fgbikmrl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxjgxmsv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjcmsjiv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tcycqwkm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zcoeamgq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ejrrleis.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3uxilcxdd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pyfnyxbr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iydhtgma.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rfpfuyqu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uopokxsf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3orkcxcdu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3pzsrlhot.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zrkainzw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3eklbwanc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xqahajeb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkhfrldw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fdhylsou.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fovjksci.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3esilwhbs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3httebrdn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bcrcatmh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yvlbichv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mctrivwk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wdkkbdea.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hcnbxype.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fwdpfqcv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3abjqxtak.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jnbokwtp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfherbkc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3usnzvixt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zdqvuvvb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmayrvyu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrllhfse.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbsupmfv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3skmrdnzs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rkbkmzrp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vavaxxdi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3boacjxtx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lutkelwr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rcphaxaf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cikrtkfx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3avxaahqj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lzcpudcm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fyvxthzi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3jrhwjvzx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lgixyvez.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nymvzqgu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jvymzqfk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3njefjujh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ogujaxfj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ahwtwzlf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3pwhxdley.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vuttbujc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lyjdxdkm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xjucownu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ldgcqnha.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xwcynjul.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ltpweuai.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3cnlxxykp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pgyfaypi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sthrwsgz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wceduutj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eigiolcd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wvlljuzd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rmsmxxcq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qbhecyrs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3utyyryyk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emqewooa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vkblfomz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rclwxnjz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztgphfdn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ldkokyzo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zacqokjm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrtcznuy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gdzrvibb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukogmufo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zejewjei.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hyzmfszb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bpegkzbn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmkkdylh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kpgfmsca.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abocopzl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mahfuoro.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qpfyfdci.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pitlxrvh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urgeonuh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tpozeivs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ltjbqufw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pgwebccx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3weddhbvw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lbxhjbaq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ugflsdgp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3fnxgzpih.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hlwlaxpd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3btzpqjph.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vnwdtxjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqqjiuqk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3osxnonmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyfstiyc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bsdedfdz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3trczthwv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fvkflwxp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cskmzwyf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkrlyeam.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3obsyqyug.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wgvvkefe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3iqxraqzs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sgrxswuj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mgsvvema.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3uzodiubl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kuxrszgj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fgtwfsmv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvwdszpa.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hchssyqp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kalotusq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3awmfeyzg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3smbjfdfx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gjjvtquw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kcqixoqk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ybaknwiz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nkklgzrn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cxvnphmt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gdclvqqh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3oqhoeing.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ivnayjnu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ogvtjalx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3odwqllxr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3btmlpxqg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vgpdxxqn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvpbtjgp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryserkbw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kenyqaai.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kudobgha.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ttliudgi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ozsdnsmx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3igbnftda.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zofwqzep.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ipvkmayl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aglkosmt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3telambhd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lunhgokk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ljbobazh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ailkzqmb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ytsuhker.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3btnkzqrs.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ihlwbjkm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hwcctvub.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3flluaqzf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vxfxkblx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jhcrcrce.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3dhexjbup.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3yxnrtpie.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nmsycjni.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vehqwegz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qqotreiz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ftfhevsd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ikkkwmkv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rmcauslr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hxldvkyz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gaozjxms.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lycsulte.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mhzkqmkn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zrqdfyen.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3inabhbnb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3igoimprp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahykubav.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcivxsvs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tcvxdpbc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3oodgvmsz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3spamlfgm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfutlsmp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xiiehfex.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ugcexplr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3oucotijt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vrbanvtf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3elfukqwr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzqnsibc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qqxfvqko.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qhmherxv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cygqvsfc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3phrtwgqd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3awkzkcbz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3elctaxev.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fxwttvxq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cpujlcpc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3urarbarq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vfcmdmja.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dukflpbk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jopcmkmm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hxhwmwjh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vqozkqsx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzhjrdwl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuqdtnal.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvwjewys.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hheeiiqu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yqcnclln.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yapjsrat.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3axzgmrmj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fghlkywc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mteoabji.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brmediip.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3baqhobep.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rmwkddao.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vckglmgg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qjmpkwli.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qjrnhjzc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fpfdfdsg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3iywjsvdq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3csrieszv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mpuoolcf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nvaodttf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3giiybpkp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dqnlviax.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mgukmhsf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jjwtoxbu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3nuvufgmk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ivsdyisj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3lhwvpatp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xlnijtxf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3juwdjhtr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3bvawbygy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckjjbnfu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3laynpbhp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3eqmhufxn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3erdzectx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eztugabw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dvnbpljn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3utixlzlz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3amnaomvm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gqsmcytq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cjpeijiq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwstrnt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vyopwhru.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pnevzwxe.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ehxybitj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mrlyqnnr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qmhdqpqi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3awjwamlz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3usqoqbcn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fnchakqk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mcelasvt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3bkmmjvhj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3afqayflt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ouewmarc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ayskiwtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihalstny.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3foewvxoo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yrcjvvjn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3pxxreotl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3teygycng.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3csssgrna.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gsdajecg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3swzrvcgd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3croiyjtr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdtuhpsn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3cjonpcfj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3tssqbsda.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brrzyvwy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qelonzdo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogimpill.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgowaalh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3tngubjap.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3oixwsmsw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vdatclxa.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qihhspid.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3uiapfsia.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pvqwchxw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ylcoivdh.html


<!-- 参考信息 -->