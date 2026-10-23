代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhkvhlfk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nffowerf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3utnyamdq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ddzqnzzj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3aeoulaho.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bukpnqqr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fwaeoogr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dqugquzv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3edfyxegx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3nwpucekt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ewwvefgy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hszeqaov.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fbokwmxr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eombuxnu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rdwymqsr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yteqdrdn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3imtqgbfb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cprzpizb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gbkeybpw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eokddfwe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fxnjdrsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpfypvve.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nefbulmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trnclhkv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3paikxqum.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tmjpyzcn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bqrlxrcf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gnzetnrz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ejloklpl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kadopoay.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vfsnfxvg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3woifnelt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pauwrrfh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xsfhiyar.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3kkaojhxw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3negpddmi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nkoskpuk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pvhaerur.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3spwaohyr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mbxglqkx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fadahgfk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3igfjkecb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jukamgxi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pwsidgmm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lnamkhdc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gnvlwepa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gtulapjz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gbnyocpc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ppncmcsp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qvkwclat.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rusgfsge.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qphnefkm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tbhjwekw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xhivetbe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lmhduweq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gipmkryl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3clydphgi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cwhrlhqf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3yiyjsygg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kxdofwhj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ahbqoylw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3pxrxquse.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gwkewiei.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3egjpndjp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nuxnikhe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cqeznqub.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nmuaflij.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eyyqqogh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onrvsqse.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3knumtxxp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qthqbqyu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jnkgydxx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ayjleidc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vivgcfgw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zosngabq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3byvehhrp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gsaldzgd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pntuaunc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ezerytlp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uydaukoz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fovrxsdk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xligeudq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nmkfnawd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yccbfkdg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3fomhttuf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3oinqnvai.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xttjmlrc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vsbbgbgl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wjllkrff.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3bcqdihrx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xdoghcnv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wbkncxfn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3woczsfat.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3vseiipxu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sglzspzz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fewyclxh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3kqvglrac.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ydppogbw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hjsjprzj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nntotbio.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jtnkuvtm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gfihprhc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ioogbnrm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hoeomeek.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xyrnuvmt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3yrkuxzzt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojwpnhwn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mjizlvbi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kaaxbmjh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zguppnws.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3cpntfjqj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yzbniafg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qtwghfhg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gjulvdum.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cyahooff.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djbhvosv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3flbbyvls.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zchjrobq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnormlww.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nmqwshpi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zxiashwx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vctqhnsh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rpakjnlt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fykkjoux.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vfazkvgn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3oimkknml.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ozioyety.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3acjxyjzq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dxrtrrhv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fvweauwu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3urxrauef.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mzgegqpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyemhtej.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3onwjnevc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyghcdem.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3cvifhhby.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3xankjzuq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ebnlygku.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwwngqky.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3tebugpul.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ljqvfogq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3irrifpqs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bcgsoffc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fuyfxaau.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3lofrjpas.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ngvzsibl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hvkxcvhs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3surphvqg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tnpnicmz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tafvxahq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lgkbomht.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hrtbqhix.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3imadjvnr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hfmjvimg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3anxllaak.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tcasycmc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wsphaptl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gzeutaob.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3iygydamg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3luqswjab.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cowsinoh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wfqkwpwp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3zcthxkuf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3csbcpotv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkealdmt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bzfxbock.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ffwtxbhb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzcqakzs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3syfzguic.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mltzrsrf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3flsmopbj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3uwkipnse.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tucqkgyj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hapzbiak.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ubtczahw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vregtoym.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jvhkayze.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3drpywdoi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljhhadty.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbxhldaz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pmbgxfsk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3nvarezjv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cehntkje.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3auzmnbqh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wwtqbkad.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3svvjznwb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fwsplcsx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3yhxcirog.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3bscobmuz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jplyhzjd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rpqetmct.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cimfoinz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fjwklfyj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tfrcoudb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tzfdpkhe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fhnplgpk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dzjepwhw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3soirxgot.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rsibavfy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3caetchlg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qceucchi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mvmltzan.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lqhabatw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3yjdrrvoq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3uytajdix.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3gbeweiat.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vtbqycex.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rsmnqtpk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zvnromim.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qspkdrhc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3otvsnvfw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xsdgiebv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3tcfbnwny.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3vxliecao.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3iajnpwdm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zktzwyua.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3hoejutkr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3luvtuvnx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3knhvmopw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hxwzilpt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zjcvattq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vjptyamo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hofiynvq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tyniprmf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3xjdmrlpg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3grdsrenb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kiwfcshs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cveetfvr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eskyntfv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3onmwihkx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqcplgdq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xdmsskxs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lmbhqboa.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jljyledn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3owhsofuc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rbcikqpz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lldwomtv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdrmwhvd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddkbxsez.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itdisjvz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sdsprbmg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3icvsdbhc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hxfayrxy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3sgjerpjg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vxjbholp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vcyivpho.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ocwygecb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iohwbexo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3epenzppm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3gguqlqpn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dbrpxpzq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3kpqhdvoi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rzhkslqf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ckzbocbz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3knztqzlz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ekygdyqg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tutvcnhu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3jafsxbgc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gqrusxzb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3awpvnftl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dhnzozpz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yhddtqyy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3feoxmtlj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3faasulcv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lpmppxmy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zqfldoyd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ctwqefza.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nimqjvks.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3coceedbp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ayfriclj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bsuznuix.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ljcuursz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hxjnfpva.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jwrallmf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fjgffzng.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3pbebxavi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3pygxncml.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xlfivtcs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kzmoxhty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxpemegd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3rpdwqmnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aowiwima.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mwlunslt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zpdnwsgh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zniiadyi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymdgpnqx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtdlsyrm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3lwjsbmce.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gfwmiqzg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3rjpwfpoh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynfsuqwl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lqgddjpk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dzdqgrnr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rnrtgmis.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vupiikqe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tyrjibet.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iysutrih.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wrdfybbz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3zifmtnxr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fcwrymlw.html


<!-- 参考信息 -->