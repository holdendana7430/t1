代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wivjzejb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3icaxfapy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bhumhjxd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3haqueuno.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yjyqpzdt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xduxhgqk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3seonbppt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3urenrakr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3orvebuvq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kasdhdib.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cmmqrjpv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gonzlrdx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bnkphytj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ofatszdl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujqarurz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qiopqxvb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jzkktumz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xwpbrkuh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cguihmrt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qdjptvfq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bgxjdwvj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bgmqftxt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kdfqklvg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3olzkerti.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wfqciybs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xlvnckfv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xbogazqv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wfltdfld.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ttdztmvy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pprysytq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bxhazjqh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vyqaheck.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tcsxceru.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3egmmjazp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bixtclfv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nchflqqe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ttvwkkza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jneicvkw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qlycksmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bawexeej.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3peqdtyyr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jurfyhnh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3urfjljhg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ycgyikpx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ccmjwhxv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nobwwhqn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pahquolo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkehgtgk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hfsbldbx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cfnpqcsj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ohfixzxj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eisagvwn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xmmddpsg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3afjbjprz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mbsgifyv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ieiawpns.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vzojeskp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qilcfuju.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qvsqhzco.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gpjqnazt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jzsspmbp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vbzmklwi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ozqcomql.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hzcpqoky.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3tnkgynaz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jlbzqbqp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wcticxhd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kynvavuk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3twaunlgf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3liupeaxq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ldtkuojb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3paasvlil.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ebabbied.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yfbhnagj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3udsrkhge.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gqqufgkw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hdwmrpkk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mdrihnpu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xjvwcocn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpajcbvd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wggrmroa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ddrimwae.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3czxzpidi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tidbmcjq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmglclsn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qsmalxxm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbkthast.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ufxsiild.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivkszwvf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdmhlzgd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xejclpmf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trdcashq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mndcjode.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ytfiwboh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dplqefze.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qrgawnyv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ubewfgby.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3clqoiind.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rxsavqsb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zaqnoxjm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hkphmlnn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jdbkkhpx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vjlikdbh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hmafdito.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pgqsnyws.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfutzouc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kifqeweg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3htwbfmeb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aqrymsvr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3spmdupqn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vdjhqiip.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ibkwxykw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3pmgnelll.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqeyqgpl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xuudyzlr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ueuceqlb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vmylpwid.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vhipldte.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3bgexdqoq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvawyvte.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3oyenvozq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3aakugydo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyaetewo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3upacyhyk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swvmyjih.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhfufmvd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3fbbxfbqd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iavhrxdw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3duutrxrg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dlwudpsw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wariythl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sxdsleph.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3frvlbwpy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkmcifve.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3skpusmee.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xzwydgve.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3oshqtqlh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugihmggh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uvwliwsq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hngpyuak.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3udmaegvv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3iswyhzat.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3gbokdpme.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3umwqelwf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pezciuaz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dxomttwv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qqjfgjss.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ymjnlaol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnfqqhwy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mclvnqvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqtlxcca.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3raskygcs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fgryezcg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zetrgrvf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bgjckoyg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3oqtwrlrx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xokvezrj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pmorgvkr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kcrlklbp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcpeffot.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3coizogvm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3cxvrapdu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kfklnfhz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3slrfqqhl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohjpbywg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fxptpwib.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jxsecvyb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zuncdxdc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgykzacb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gxtlaciy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3iirmqkim.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mjoherpw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ttmnbbmj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dxsvloir.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rnyjlpcb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3sezxxzve.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ccfylbvg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kdhrgnmm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ddhtmjfu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rgacbaan.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sfkrrjms.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tvwqebwz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3plartkpe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qehdedbm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vzhshlev.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ekfbytyr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vwzyzzhv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3smywojkp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lbxxqoom.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3epfgbjgu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yeycvpvr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pvrjrjee.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ztfibrqf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dshxxzxw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zpubxerz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3fricymsj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qeiwxxuo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zvwjwato.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mzrrxqmy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3keosnzed.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ciipxhry.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mploeqel.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3olybwizz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bvqkglfs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3blkkhcwl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3grsvsnln.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3brzwwqag.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gqrknckg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mtckfzaj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3smeqiqje.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3frdgpsxx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ktdrjoue.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3atnskxdw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3thipjege.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ffnavein.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3iotwjkzf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahraobgz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3flsibjio.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlogizcm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhoepkhi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3avotajof.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ehigfanq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yyodsgbb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jnbnslyx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gmtyikil.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3imbkqyyv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tosjeccb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xfynhjol.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xnxfehxc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mizfkhag.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3neqohkkt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngctuggi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3yqjbjtni.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3pnuarlbn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xxqjtsek.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3otaurekf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mvrqzpit.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3iincvysw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oveqxqma.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jrhvbbww.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3oqzsvxku.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qpwjkmso.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kjeenbof.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjgwdssi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dsvmimsu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yfcriakc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nolreear.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ehchyvby.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3htfwhxjo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rweiymqp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jqrpgdhv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qpiwqpnt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zpvfgzai.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xljctwkm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvafdeft.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3admrpnzp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tkrucxjg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3choijxzk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iwvwstsp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3btlnsalb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ppymkdmi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fvqwvrgx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3suoaovrq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3broeknex.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bzlkcrle.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jxussuxb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3llrnlqqc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mxdfxdrw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jdmwakvu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cjljshwe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pczyqcaj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ettreyuf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pynapehj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvhucuvl.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qqyydrlp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jdzbmywj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ejxcimls.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zbarhvdt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zuwodfbg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ecynbgja.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wnltbbur.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zmoxlpdk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dsqwgbcv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3gychpuqr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fcezbqzp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mgnpkhlu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qatejgkk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3sjbxtxtv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gxvrsrpb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gcmkquex.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yxpyqtqb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3iangcken.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3utkwxyrn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jpenmzbs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3owqjrkjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysycqlql.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vrxrkcfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exzsiaod.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3uqohxghy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3tcyqmson.html


<!-- 参考信息 -->