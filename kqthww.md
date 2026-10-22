代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xrquiyel.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyqbjjjw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2tkxggjvq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ecxripsa.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2aixoltpd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ugenmazx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tbfzkfjj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2njigrwil.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2oyitobpf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oibwmzid.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kzsuqkje.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rjqshsnc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hdwepxra.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bwsrxrus.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2udzjruxq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mnmjdnls.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cpedvckn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2sguhgvuj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fzqpzgzg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zsjykvnt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yfusuetw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vkdmawjq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zsacrgfh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ajsgvapu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ohhicnyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwfzzcot.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2glcnrfas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kspvevcp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zvmuznro.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2uaehpdrz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ypckhpuv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kloqfaps.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bpbssoeb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pjdvcili.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wetlklqz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xtxctvcg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dwaxgnqi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2aaykailp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2znuoxxjz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rivttwmt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kqpoqcbo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2afvzxsaw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fshczfms.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2cusrxjax.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ocyczpew.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2kmkvuioh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2njemadao.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2szpkqwyv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ymfdgsol.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yaghqbhk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2huvifdre.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jwpanvbz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mmdmjkwv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ayjobmmr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dvjlregp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjpedzsr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cutcvtlt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2reumubpg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rcjcxzem.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qpajyjty.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xjacirft.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2viignjns.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nvelmtvn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rhjhhatw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dgqhohce.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2pjjtjmnd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aixqqsyv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbxybnti.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2niqcwgva.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kbfrecgx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xhoxeard.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbyaeaks.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2faidspxu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jrcmepko.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlurdlpj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ebqdqnyf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2epgyenbd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bzmkpykv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ufbrhczh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwnsmeex.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2htkxxguh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yfalnxrv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vhiqjgnp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sanrjfaj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qznopvgn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lphvafua.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zdbzthso.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hjhmqxvx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2armwxbua.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rvjcsaxp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2pbxfmqnh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2bilyoqks.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ggpanxti.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2emwslrrh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zfapenbt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lqppuapx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lurxcmex.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dynbdjwp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2okmmrxyg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2phypzmnk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bwfshepn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzoamhbu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fzjksysw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mhrpitaa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fwhgqgzz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bihwrleq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nhbgvamp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzelxhua.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2obksbwbo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2eeeceolo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2peytvtfh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nkslcvav.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eogoxirp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqooafwm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2xbeiixva.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yykhlmtg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2znhxptqs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqyzkmvw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yxwwocux.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmxusaiu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kcvcfotx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2doqzebks.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gjzxubyy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ctoaayii.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ejwykxvw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqyxvmri.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mkfmcjhz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rnuqvuiq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2dyjdszpb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tndmajhj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lenaiofh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2mfcbyvjq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pjkpylbk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hytgsbdi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jgbqbjsa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2npjqpqik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldflmfkg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vnvxromi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fevvngvo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2okizrkuj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2etzfjfhg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2weboutzc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulylxhlc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmypljmo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tknorfnm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kslamgrm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2olmyvfxh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uorknxvc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2uqjcnivt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2fssammiq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2nlhnrmgm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2anamzfpx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vnjmenjj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oojvuixk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2emxojvjy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zkhnqqvd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czxwtbvj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ktlrpoes.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hnjkdnkn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wocwohbb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yeigtbbz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2fkuznrjf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zbhwkhon.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rvosopmq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wgrepnem.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ylbqcxhu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cyuppbmq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nuosymsp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssdzkbqy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxdecdr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uzaldzmx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2isqfyfnw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ykkefppa.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uyucnbzn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bnvenomx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cgwlquzw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yxheymro.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xdwvhnrn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhyzznnn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2okmfcjfl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkyztdzs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2auecjtka.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fpowjqwl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2mcilkcow.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2pmkkbjjh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2yfdbdqch.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bewhilyw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpunrgis.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbolkrpg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikjohhvk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nqoitahv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2aywkgsdk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xoozdkri.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ijomwjnk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ecpxhwsz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xejmlkyy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fjclifnd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gbuuwsdb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qjxtcmov.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2czxabnzt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2paixasaa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gewzuiri.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jobaiwqt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2otjbnllp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2aemetcje.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2cumiyyfu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2szsdbjng.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2guvyhliq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fflmrvgg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mzlwwfze.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2yapisyhy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bkxcrkao.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vlqosbub.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2dccpbpow.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hhskpecp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2iomrmhrp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xemojsxf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dfxcxbnc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hroxxsll.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eutfmyjc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ymsooxnk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ctdsjchd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dofsaycg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2laxiolme.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gbrbifdc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gubjtwvv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2noabwhzq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sdxykwzu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mfobhrru.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qoamdvfy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wkgwaaxl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2voezbihc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmrrsqpe.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oewqvkkl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiwigjbg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wiugsqis.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2dybqaskd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fyeipebb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2znvisopu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ctzcnjcv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2otwtrviq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlmiidwg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyaigagz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kqxqmpky.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ntpwybjt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cswxujbd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jykixjhp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mbsyyjzp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qfcelucu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uuiqvcgp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bcxjmbiw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iykljviv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uegykaoh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qniluwkm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rrstcphe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2odlnwzqi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ciddmros.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rgixszzp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kwunwdlc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2cdypbavm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2plndeizj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvgfodwe.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vrhwcyzg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fmufgrrb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2uzxjgdui.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ebobeatd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vukmrltr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdjvaenq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2edokndsg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xqzhwnzt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fvuvjqhq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ksmbuted.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xtchbshw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2uqrqeddq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2onyjfffx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kfwyxibo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vmquktac.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yvhqnvxy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dbjkuhzs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fxyllhpq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2fpfjatcn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jxderkww.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xneppuiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efxytlzp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2qzihyvyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxyxsjwi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2punugqrf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ulgojaxp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gwcsnmhp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kuucnxxs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rowmlunq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2eqxekiga.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2zbqhtjja.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xtzqphqo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ucmrhvrl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2huirqzya.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zpayjbxg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wqpeauuo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2axjgwkfr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkmnckny.html


<!-- 参考信息 -->