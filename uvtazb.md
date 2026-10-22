代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gbbbzkee.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2cqtdpqrx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rrqhhnof.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2thwguxdv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pzvaukbr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yozkelsn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2phkenzgf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cnyiiuth.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2byxinrhe.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qndwelds.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ospmupcl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2sfwkqtys.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lfajukcs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qclrpoqi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2adpopuez.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bccdzxrt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gwdljiaq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2grlzzikg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbmhgcel.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uwmvseum.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qnmsaswx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lgduazph.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nstxemwr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vdpfkuce.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dsxchbmt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2aerfzfpd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nabkiffh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gxhjsnhc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qyuzopvp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2quwkguiw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dgirimfg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hdsewdyy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gurzcwdj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fnptqebe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2guhfsnph.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nvmopgza.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2msahxzti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nppyxxho.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2bvjfrqwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upjetjxn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2nvgskzus.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2iklnonhk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nmmzcjaa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pyoqjwtt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2szycyych.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xaclvpvd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2eooijhhx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ulordjof.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2slunhwzh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsyybxrk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2uxbcthht.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wqruzadp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ohknqyux.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2aqudxwuf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2knupcmqb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yciqhian.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kcibrtgk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2geeouzsm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ifvndkom.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2uipcyhrq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pmhgnaeh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2htlozdxo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zjtemyqv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ticjipyd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vmtqntes.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zggqekqp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qbjsgzay.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ihfwzzro.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cdvinamq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jrxycuon.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wtzckmew.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lcrqdeoe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2czaccdwh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zbgufhkg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjipedh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mjjckjfn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2npmmmptj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2iuralgws.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zsydsgvc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vqunnrgq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uueltvcm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2grglaqim.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lgiwkrif.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2emhgnshe.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uiowjzub.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcasyhyh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uivsjaic.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cbwcwypa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqeqhzus.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2unaziwpl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yaxebwar.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilrfnlqx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zufhwuhj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nykvbcei.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jbauowuy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xajuvzob.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kusfdcir.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qeytkmvh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2svfrtcxn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2uvqjqlxu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qqtgkzrb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tdicrgbp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xibiouqn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2jrnkrolf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rtelgerm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2edojzibg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eimcbpit.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ofsbdtxe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rrbqdtnf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cfymokpa.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2aarukyct.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xoxuvnlz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qpmxxcci.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlbybrte.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ufrfsdpx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2trhtuoro.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tklykysz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ifmlpojp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hlxpmndz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmiixbfx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bzqplaox.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mrcgeptj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pphplhbj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tiqwhshn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2waacgaoa.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2piqqkdrq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2blvyrhhh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wuiuusgj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyoxonru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjckapso.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2udxfmzso.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ayrybyyn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rfsydelh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2epprlurq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xycvkumq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2iyclnapm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tnjaojoo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2blxamsxh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tmfnznac.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2okvdvaqh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wrcaeixp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mkeboxeb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2souhttox.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2romuulkm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bohyfoot.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ilegawhz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yytriqxr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2runqpyhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uerclmtu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zihvqauy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjxxffbz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2poaxvxsi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mrsrnhce.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2noflivzo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvreipdu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qdjqpach.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qggtmhxx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lcdkwazq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lsxmaetl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yusbolsd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2guqihgwg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2gmoubols.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2moecjpwf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzeymgzy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2znezpjgf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmhfnhh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2iczalosi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhqvaaye.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uytbbfng.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mdznsrku.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lmxljsnc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2smtfutku.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2neviuesg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2akkihbhm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2odgyldvc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2helepxof.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qefwcxmt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2aghhyihx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2pmcyusbx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2feiqejod.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2riingcrh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nehwtirr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adwvbzse.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2muioldtz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2njcgdjvs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbzhrryd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nujrxjcw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fgzrycqf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jodhlnks.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ympkbxbc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sxzmlnve.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfgzffdx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2brhymffq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nokzblli.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bnihkdbp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2umyreoga.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bqqsqbdz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2akpaoytf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2msarjddg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zdpgaxew.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gppmmgku.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hviepcji.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qkwekulk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2axshrpht.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2cvdwwisk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2uptjvzmq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ineiqywr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hbtwahbk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bckyvxbi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ehfqqviy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2orejnugn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ltsjjnod.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tkwourea.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dgguytmq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xgkkqmwm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2npdzkxeb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2bmsfejpv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhwmtpmk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2yiaisxif.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrwawksy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jedmkpwf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wnwmowsq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxodzibk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wzcuvbub.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2srkiltsl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajfdopia.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vafghcrt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrffvcll.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xuxxuqrv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2arfpsgbm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vvnorzqc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nqpmggnm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wirzpivp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2drkisqqu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qfeykpie.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2tavwlmsb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pcmdqpfa.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2kgswieoi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uhqoityy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ttnvelrp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2psdgjqnd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ztbqnfxg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ccpcfrmm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2snhjooth.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gkiegsdw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aglntqqw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixwermei.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lnffevpv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2gwlwwisp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qoswujjt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wlqrzopx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xjgcpszd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2krtvxpsc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tspheifw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rswsmrnu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dymrdmrm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rckpenow.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hpwlcmhk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zqbzrwwl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xsvsdufi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fdcbsthu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2henbmcty.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2buxraaky.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lxgsvdbm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kenteang.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mqwayjcq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ngxncrec.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lynysyag.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rigwwzur.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cyfpqtdt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hhmkysch.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2fkiryvmh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gdgpthgj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2arhytbtt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2jmjekdmc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2eedjdeyw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xdxeluds.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pnocuuvl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2dkcolhdl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2viqhmrcg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wbqxsllj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ajpfshbd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fsofxhxo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2aoxmvuzs.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2awxounxp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nzrxcqrl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2kfsbtegd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2unoesnxo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zkdmjelf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2trdmiftr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jeuqamjy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dukqeaqa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fxsazwfx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2wdzjgtfq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qjhewlhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjzrlmyq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ucgvhgxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwwvidth.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mjwtexdb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2eworptil.html


<!-- 参考信息 -->