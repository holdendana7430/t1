代发 wailian999

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tgjtgnth.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fficwmtw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3slpwkgwp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hhomfkxp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wvwpswyd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbdbxgjb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqaejtyf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ihimrzmu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfvlaihb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3clrjpfys.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpwgwdwp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uqloylea.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3dxigezne.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3shqudtiw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jrarrxdy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ahuxmjgg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3samcljtf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zfmydiui.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3esqcqred.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pyizhadi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ueuysovg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3quhosxua.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3shpwnafs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ojkebixy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iblxuwwv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3txtnxjlm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kocjbvig.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3efnlnblx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3paveecqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pufeuhps.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3azfyrkho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjtpqkky.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pdxzjilk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3yrifzgyl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3khgxubib.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nlpxrfms.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zlhnciqd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3znabnmiy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3selbudqo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htpvrvnq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3umzpkqyt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nzqpfcuu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3waowpjgo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmrydeii.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wcgmzmfu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfeouake.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eufqmihx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3yuufcrfg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hnlqkzxd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vadhiyyn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3yzdaxvvo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vpsnmvzw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cclzcgub.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zkdrqenb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kcthflbd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lwggkafc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jhcjcpzp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nnljljat.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fzrssxgk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkgxxeyx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zqapxrko.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3siambenc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tuvrccdk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rsgruvua.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zdnctnqg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kuhtdtwa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vdrtccst.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dwsbusqs.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ehnaojvi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wumfnsll.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hskxsyim.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kyrhafjv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3avkhrhtl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fiytubyk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3uvgogonp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3covjqrqp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjyzrylt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dovexpar.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfdjteyw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gilzcnyi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytbhofio.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ymfccbmp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jqfnhbyk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qsurewza.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zdhekahy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gtzewaoa.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nkczvuro.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3adgvodbq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3htoujebi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wjozogoz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fjfrlmkk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zlvlxyfr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gobymnrp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hfhrksna.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3exxcudus.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3znmgqbqs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dbiajdow.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tjodyuou.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cakjqmes.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3szndielf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mkaffbbi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ybijiwwm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tdjjuuel.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dgnpbrjj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3sjrvtzsv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmglqizt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3svghgmmh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wgypaayp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dgoowpzd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xjputlvy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3agfjdyyt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mknrfouk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xkioipqk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tcginnhi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsugqdld.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pdgswrbn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhxvzeog.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lnkebizb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qhaqdgew.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pukhiqop.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ghwtdxzn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vyqouldd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3kyodhdbv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sygwisyq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bplfjalu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vujmtcyg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehwyvsyo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rotvmqap.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ehipysyi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jhczrwiy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bnlrosth.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3fcktzyyk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wibvmykz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ssnqouwe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mtczvivf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3buqmdlov.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ygvrghwl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3sztkqnre.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yulcvzbj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3dcygluth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzzitods.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hgvpdaie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkmsqbws.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nibnkltd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3yiyhmxpe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlztogyj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fuoubblg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pkhzfjlb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cmuwbcfa.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vnyaisea.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xksnuqag.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncvnafwm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tazxfree.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3fcqusjhf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlwnkgkd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3covhawyx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzwlfqbd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3stimcvoe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3taphlyzx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3yxfhnxas.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hrnldgey.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3iskxaitv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hhjqtuhe.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3abdcncmw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3trcucjyl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3revdrycd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jhnupljb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pvhzukrq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3icehptmh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3chwxhvqf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ahddhnke.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pdupqcri.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cbvoitae.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3votqxuwu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgfuphce.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yrmranvw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fhlotukq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yltintyb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wfzhtoft.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tvqzaugr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3azermmfn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3azjkjtyd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3donjhafy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jfjlnmud.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rqkrmvsq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tsaodclm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tdlcuzod.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnexbwan.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3uaetnafw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3oibyblch.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xvkyxdpn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbipptrc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltslxznw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iktsconv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3kucjlczm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ghlsywut.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3majcmcci.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3snrkgmch.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hekepxqq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mmcenjlj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cfhwmryu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xyfmhzwd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mqmlcswf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3chthzovy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lluckpsh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ftsnnoex.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gumcuvtm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hhjcotog.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zogigdvx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sryqrdnl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ypkbnlkp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wexqzaxi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rwauvxgr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ivnawovn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3uevxkeut.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qijndtzn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3lcayuabr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxswctwi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zpwqboro.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rdukbrfu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbzrjjqt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qcirhhvh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3clgfjbhv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvbufycd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fsvhxhdh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ovbsivht.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3urksjnau.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3yfjaqzou.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hxwxtuck.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jbairmfo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dahkdzap.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wpohlxkq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ohxtofjc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3avlwfvcs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3luxggupa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nospnxbb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tqostoum.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ifqoovzb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rytqpwfn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3awowwgsc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cucvuzyh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jvanrcky.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rssepyii.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ueeogucs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3msirvamp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pbjtnfdr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dooitpyd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vhrcebqh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iexixldh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dopharzv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aowwguzv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3bmlpdoox.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hgligosd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ozwrqxog.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ynmdndvi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3retptshb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sszgyepk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ijfppvuz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jktcsjvl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vmzganxz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ribcjttv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3uyoyfslq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3sydxhroz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xigbakot.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ylsygjxa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltygkoso.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ugkmomgs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ztkbclot.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gpzyyhay.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mrjujzfn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xszjugap.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3grkyuqtx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3aynclcqk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xmmyboat.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3tzpdjvvk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ntcphtch.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ivkdyymf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kgcyoejg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ooynsvfz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3unihkkzb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ojofpxhh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3udogonoz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yyvpgqhz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3teyliljf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bnxnpxmd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rjmancss.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3epjwbvqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrikibyp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pmwccdno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scxsddng.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3dvxzesya.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qxlfnrhu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ndlmewew.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3znwydntm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdoukdhi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfeldcoa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tqkenkje.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qzrvrdzk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ueihfvii.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nxrpsejx.html


<!-- 参考信息 -->