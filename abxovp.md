代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sesvkuhi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sfjwzdmm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gvxfdrwj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dpevhpeq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2pckbnkrz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qtnltacl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2kllbzklp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2eblrprmm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xvzxgynm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpzlmtcy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mvtswmju.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kjdhwfna.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmgmpwfw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2whuotycg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyclfsiq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2rajcuqnf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rwbkydat.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oxjlgaux.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bjirjruk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bujtxiot.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ymhsmvty.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2irdzxsob.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rxtmgbgr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jadgohyk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2srdkxcne.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nbdzzhkn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yycuvvtx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kgtlqeai.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sfyjloqx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hospirkm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cukmorvy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ccsviixs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2oufaosit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttgyuxyq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2tewcsgau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwbbctfu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ombueiac.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2tvkghpsg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ygaccahb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fzywvyeu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vytbolwa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fopfqqfx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vmlfkfwp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtoouuht.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2umdobwcp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rvpfbiqy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2rwgtlvwe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywdwtaid.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2crejqtbh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzcbwnmy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bcyjuwlh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2camgcbkk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2todguiyd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekuzlnjk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mzyjecvr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kjndyhpk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gvhpytup.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2trvszwxf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ffmzfpib.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fbncmvsr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ogxuzoyd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cyuvfvsr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mbqyqlfn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xrwibceu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fwhmcyjr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ilvkfjur.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2usvcjtrx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wclctxmj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nhvswyyg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2itjacbob.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2elwnfjgd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dytenczv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2legpicpz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2leoeviga.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ejmfzajn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2towoyjru.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xtsdgyug.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vyqdtdul.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2gsbgznap.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppxcjyzh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cuekjigu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrwxxtvo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvvgnofl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uqklkmla.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rndjzgts.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmvvdnvk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jggzzsip.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zuwddjax.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idvgigdi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2syxtcmbi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rgmgwcdg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kvfrcytd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pwnxclym.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tgmahmzn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2eompzsgf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ldihpidv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xffddtcp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2minljcgf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2grojqkmz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gwmijzec.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2memblfhn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgwedfnu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aswiehth.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xeylobhi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2havnlwcs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gizwkers.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ztuqlvtl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2toxkcsmw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wjvxiirx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnrlazbu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wfwjmctj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tkzcmywt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nxdyopoy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2palejagq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jzuchlwh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wxawcvap.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rwxronho.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rkjtlcot.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kopbxgki.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iazczzti.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqcsbbat.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqymcwya.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ptutbnbj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2neoztvuh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cadjpqie.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqednqbk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ufaiugpt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcsxtqzb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pllngklk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyatnsiy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2njsnknxb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xiwfqopg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2yfxasfmh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ocyxwptc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xvqxabep.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2urfqprdt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2cbfcildd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wsxrbvqg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jqiixsob.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jkdgffge.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2jbqxgupp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2snkwepni.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nvucnknk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2oismuxax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owosidaq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fmvarghp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsouksov.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xjfalurs.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kzbdkjgc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lumyjqbv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rdewueyv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2oatkszmk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttkqwbwc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tdpcbfvo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cznuanlb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zydrearx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cunrmksi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cvlcoxbh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2prckhycw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctqlfwsj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2quekkqie.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umvpccsi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zhjkfkfi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fblafkkq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2etwguyux.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jynmkcik.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zoepqssb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lpsmjtjf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pbfmpqmo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hkaoilij.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2sapjdasg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2sezmxocx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ldehiwht.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mfybjpvb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jnihejiq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ceusfllk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2igqesgoq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqenvtar.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rxuzlujl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2khibhrxx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fpowyiar.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2woqoypim.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2naoemjdr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rlghnbap.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qrdgbfnj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzlqqfxc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dyzjyizp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2duehuxib.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pplkezjp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lhgcsysu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2oyyanoeg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rvusesfs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2cjaquclu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2bcadxmhv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jvjbzzkm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcvprfun.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qngjqcgg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjxlswvu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ryzsleyr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtmszmnz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gkodcywm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pupoiqfl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2btkovjvw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lzizrmsa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pacflqnm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kokuzezw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sfkxjjqn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wbayvsov.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jfprktvu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dyiohqzh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xapkwrjg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qhmzbxch.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ndfmhkac.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2oeogkjis.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kxlcpely.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2pszsegoj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ltbqfiwk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2avhtbmqr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vakzwzbc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2uywnyfsf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2tereydlg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufdcecbm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2thjeupxo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwxratii.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2fylotkqu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qyssqlbw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qfllbato.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2laodhlys.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ojnoonrq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2krvzlude.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xxxjvlkk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2efvpimwq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zxrsfomu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dvpmqfrb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2okfsgsdi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rjbqmlvn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2iggavaov.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2uyuknznn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rkydodju.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xwvwmecr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqmqikbg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bsutibyv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rclalujv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tgpdbzzo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ruqhrymz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mxyfxhnz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2sxzfgnsu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ymiazasl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ocyadrng.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbjmhxxe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndcpnsfg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2osuaccnn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iuzzruoa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kkunnarj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lptnnjkk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2yovgzfcr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ppvfhyff.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hktohrca.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ekbqujwv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gqanmtqs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dfifpypi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yvmzgcil.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lathjwfj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wyrousse.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2kasnjqcg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2yhnjwebm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2arhamtib.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2whmxdxfb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2dfjpbods.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2fmmhrvgx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gwxlayhu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2scgcsjjn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2uivyoagb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vmyqdsnf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yobaagon.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfamznqw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2yrlimxzp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dtaogfwu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2anndccoj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lrsfqgin.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jgnaqhky.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2uvhqdzpa.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2cjokzale.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2sdcvbkrm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2tcknoxra.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2urezqacg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uaciwqre.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yjsenhoh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jilimymx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jeipwntx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ysyptywd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbtzezym.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kwvugfit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rylxjuqd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zatgxzys.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2frubmqsv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wtfzbxdk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eysptwuf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohnjzeeq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcsbgrye.html


<!-- 参考信息 -->