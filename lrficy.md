代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3awedfktp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wndcaefe.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3keqindqy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wwwimivz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mxirvkkh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3axjyadgf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3tcnkrulm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ypxtkymb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mqcvkeqs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gawvswze.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3utijttsl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpmlodgu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgphwjys.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3umutwbjm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hqzlwmzo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3pmxvndfl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3atrocxla.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pnivabko.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qoknqbkl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fhzimylw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hucirnie.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qtdmqpio.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gkvjngdf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3twvkoruc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3yiptjkmp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojcupbgp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3limrcxnq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3grdxqimc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dxjamttu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jgpksjqj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zisktuxr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mmpmvuyd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fuejjdal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnzregef.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mgtbxmai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czqtybwa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3sxfnzwbq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3utsslzug.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mghkfjba.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3arvynrqp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3szzuquby.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eswbpkyp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3socvgvlz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqcgszuv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pegfgsoq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3yraifjsj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bsqnfnag.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqqkyeyl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oaupntlr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ihhtpoxk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mivhasza.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wcpywxlq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3npooieme.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hwbmrabw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fqecnpjm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sfnzzvav.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lhnldago.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rkzhmsik.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gdzznpnn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3mstrbgqb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3chtnspyv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rzpusoau.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3reolwnrj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxdvcygp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jqswkbce.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3oqlicupy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mqocbxif.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3crbqtgnt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3hzrdzkyc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nrljtecj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nfnvoyve.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ojmxmvoj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3paapkaag.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qcjudvwm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xmdyvldj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtsselmr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovacllys.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jtlalwkq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3cfubatui.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afazsfll.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3audkfyoh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cgaghubw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spsevgvm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qdzxyejz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tajfroyn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ldimpvhn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wredsmxj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpagolxx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3huwrmfau.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rgkinoow.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3twihczxm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3eipdykej.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3suuutlko.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gjpytcjn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3amqyootw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zoxzhzao.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3exfritbj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3uzcdeemr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bjtrqzyi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nvhocrhn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rznwmmwi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmqttwrt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3keehmdpf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qjrezrka.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lvmxrhxp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3plwboywq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gpchamlt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bubliibz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3nkgqljym.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mesmdwdq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nnfjyysn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mmevkfst.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rdgstvjy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hibadwqv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3efslwhmw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrttqxfu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zsbrquop.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ueqhbqaj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yyscpwlj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ujtscaxa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbmnktvc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wpxcjmci.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3gipxigei.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oltzokmn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mzmkjahy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohadpxzz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3yrbbypmo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szaeoorw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ptmnvgta.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nixmhnpc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wtvsifke.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3poyroeij.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xtstlhwq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouhfjotv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3fhzjftpc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ghfrriow.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uauokthp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3htpfadnd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ukkxocqy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ekkdtzqe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nvrbqdtg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3dzynchhc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3spjukokq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3btixxbzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmvpxnur.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3bflicdjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugjbecvg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vlbjrfed.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dgzodvfw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3twhzvspc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fnbjniyp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlhrfxwv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3nelivpiu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rkkirdbq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ctxhwkzl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ekcrgwur.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylzcgdcx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3froayrmi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzgqewwf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhmlvpfm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtichsbs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jnjlfwix.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ykdymqfn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ioebpezt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iokxxyay.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qiyhcdlf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ezhovrnk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cwnfiecy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xskboorz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yqhqrgrg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ckiolhpz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nmqgnydo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xwdikkkf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uaoyactm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xtranwkz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mvxclzst.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3srqrfksk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nqkytcid.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kcdhqsup.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfusboid.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lrnlltin.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qfvvoieu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3inwedqku.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3yiswerpu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vufahigw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwlxwjdt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdcenejh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlspislr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwfkcouo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jmddtzor.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3caznhuvx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zksdfaoy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qvdigdrq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qzsdyzcz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdlmqdca.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gqkvakkl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jtdcetvw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odivoxrq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bbwbkmer.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rjobejen.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3yztaddnd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ybteknst.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3copisohs.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3wnxqlbbc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qlnwcegv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cmdbvpct.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qodfnxfv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ydubhawi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vrndwpjw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fevwqqpn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3uoifiunm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3odacyotz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewfgeyvl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3dqhptsop.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zstgzlxa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3nytgznel.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3spmfjfnr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wfclgfbt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhtedqoi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fqrpldgl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vdvabtfj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktdqnxvy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dallzurx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3blkrzeti.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trtizchs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lqldrzop.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pcxqcnpd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3bcvohihs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3tiizcyns.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qskddvgs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hnuibmuz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3okvqbfic.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nwpycmqa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3pmgcqocx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dmvnouof.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rvtkpmos.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jijepngb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cygqvlbn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3htxiafnj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qjpreqkm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unxxencc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3alnsaapk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dflzjquv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hmavzvvv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3eridcitr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgxpflie.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fnsxmwcq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dsrmoaek.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bqhfzkee.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kofxuubb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3orlryiqo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phpsjuao.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3njizfedd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dnyzwfze.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lkgmooaf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lieuthhn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rfyuktmv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3weroiekj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ycabzvkj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tydzolhy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ptkycqbc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3yhdeywtr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zcsrjtrk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yxfxylag.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3eatzfclm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zklpsqpd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xdfbcgbo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3csbbfrlw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3abjkbrfr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eaajfdjl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ofrlkray.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ncjkvteo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dasuwrkj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3sqhbobez.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qqsuavnr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nadcuhcw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qtwhlosd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xjzrrwws.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qkivpczc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3prrazezp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3iqfoellz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dwpkrnup.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3yztgkwen.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xiroecca.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3lswhssng.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kaegfzjj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ppmlajgu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ieeuwgsu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rgkhnrbd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wmspfsqp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xjsqlupu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipyopwjg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yucgqofc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxpfxveb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3vlvaqshv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rsoyuvnc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpexyqhj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xzqodspp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nsgzemlu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbfpaiag.html


<!-- 参考信息 -->