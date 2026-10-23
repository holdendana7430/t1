代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3oltscrgz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtckogp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3unldomdk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wmqdxigq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3prhsudhg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dueizlyr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3cahnuczo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zgcgjfay.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3twmpboea.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwduqxgm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sdozryva.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zfotvrix.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lfjwcvwg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kpoikusf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydagshbr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nggsqiqv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3cwqeyqoc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lblbwvzu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3elnyrzpa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ocrtukal.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vyoncwwb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3usqvrdyq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ppsrsucw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pljnwfrr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3tejtqcre.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hnwbrwqv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ncsceroa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ldukuwmu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eaogmium.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mxlownpf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lltvpypo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nqqdjyxo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pkjlatfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qljddqoa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bftlhpld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubczzgeg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3itnnvqfd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jydwzpls.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ugvfdawd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3mwkmcqsn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kqqqwecc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zretepcl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gjnvolmo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oscmxsye.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3meylkrrm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3tlhpbirp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3keuyaihd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vhkjousf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3daayrgcq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvqkpvbs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dkobmqcj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wflvjgld.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ecceegwi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3okoddevo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3yozrskbs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3noqetjaw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tmabjafs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zhejgdhs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qrxypmjo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3erokdkcx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fvhxiyjw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hoormhrz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tviedtaw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cadaammi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lzfkrloo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ficjrsmb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rclvpgkw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mpedoene.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qcctvquf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gpktbgsr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zarwwzjz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wfiaxxoy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3crbxptiy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3enancrjb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jcognbrw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmaisywg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkhdupyp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aqvxbwzv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pvowbdxl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3syumipdu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsrmvpbu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gmbqznus.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxzgxsxv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wdbnzfzw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qselzxvw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zmibwuqg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ayazpiuu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpwnfbhs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3scvxhddw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kvixfigj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dfqsvqdu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mwsuwbob.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3amymuaxx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ujzqwlvw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xxydynpp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jtqschef.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3idbzrono.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hopmdclb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rpjzkuio.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3kjozxtow.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3aluvpddu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbjbmucp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rjfxbwvb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zsndprcs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tiqjukow.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cipcqivu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zngvmxpl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3havsrlgu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xhdszztf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ievvpcwi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qyxmxkhc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zbpydbkr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jylqkian.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qllirngb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3gemiywfr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rezoxzkf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hshyzhab.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3yqlaztaa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxjrthzb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xfcdlbfr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mrhjehfv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kmtjyapk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hhywvzee.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3javrgwjr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tuhlkdnu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvnjgjpy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tfitjmdd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnzvnnox.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3isbguaha.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3doiniyzx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdapghdv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mbrhppmr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3prrmrzvw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ueexpqjy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zbwtcjwy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3eltnhowo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wggkrinm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zinrhcyw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dybildey.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3glucohfd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qkimsppx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3aaicmnuu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3nwdxrsrk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yipbylva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stlabdzj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dytgewcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylvlumow.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gledhcvm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3spstxwsj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3abqwcxmm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtkiznyg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3hfvvxwdv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsfejyhs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zswidrms.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ehfsrjht.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuoexykk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dvwqdfgc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ovjyuakp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3eauvninr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bhvupzpt.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvooqcly.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3raddltqu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fpbehqbc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hfacptzp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnrzooyi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mthlthbd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3otphcqvc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3akhugkqa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nzyrwdnm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3unppykcq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3trtxwnmm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pxnjmfmn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zbrvbrzv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uboalgil.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gbxgotvu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lsjayrwt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgdwdkpt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtsxkbtj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iipkimxp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdmxcwia.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uhxdgipm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fbfgqdwf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nbthxdts.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kkwvhbiy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kuoolubq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3khvbqcze.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbdualyq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3snltdnmb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iivrifjm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3eugpnnux.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3erqmwqdy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rigcshoi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wpwlqllv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lnuvlfkg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3soiohwlt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nojbhfax.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qsrrzwza.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnvrdssy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3atfeqqct.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3roctwleh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vtnmofsb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dymjdhwt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3aiiofnym.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3rrjnrzhr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gugjyasn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qoaceixj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rvtfbpsc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lxgvucht.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ouswberx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wgodvukq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3twwdbdty.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ueikizhx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsmihojb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3phylmgsp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rliyhcwz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zccnarrn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3gpwyzmcz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3nioeovin.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3psxpfowj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3shiorqqw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3opkeecmu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdhaqqpv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mvlvsnrd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mdbhizhv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zohkzsen.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qhugfhsu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3sxasapvv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjjxnyof.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jianhsyj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3cwerooqy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mrfafcqn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fcavobyj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wswbvmav.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gsvhatpo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pamlwbvw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vfevvjub.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wodfkhlg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3sbetjoko.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3hrhudqhy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmbfegfl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rgpypxyx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujcmuuhf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cjdougdb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gavuqgfh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hrqypzed.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyxjosap.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nassqdly.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nvaqcekm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3npessnjq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mwpgiaeb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tloqiqbp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3plqapssd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yzefcmiw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hgwlccrc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3okfdrcqy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xgwldexe.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3whlumtqo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bwardwgq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3knnpgjpu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jpjouzzt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qxifhbms.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3dveacqor.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3nbusqegq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3blwqdfji.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3uvtbbzcn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ugkyadbd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vkttejey.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zwlkmxcg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3scyuvyyg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vqnspgfy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3yozhmgir.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ztgctfmp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jieggqmw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hrwzjenc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3swuuhbpi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3iaoxoajb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mpzavebv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dhbkanid.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3djcvtzgi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3rppavxec.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mtywijtd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cwidyabs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dynoabfn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ywxixlnu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3geouytlb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hzhwpjqr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hfwmretg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zundmmmk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ymglqubr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wmrqepld.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ubldtxnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbdncoeu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yawedenx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybegpgko.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3repkyklt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3soxbyyzt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xwvvsgzn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzkaoqwu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gawbaygl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtoiaewh.html


<!-- 参考信息 -->