代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gqvnxwkzn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/glhgfaaqs.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gtdxyzedh.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gaprxcetm.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gvqreugxy.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gtcugtstl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gzwckooca.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gcaifmpjx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gaclhuhau.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gcxpnolci.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gusuxtcel.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gguetdmap.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gdegkbdsk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gbwcttsmt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gycbpsnpo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnclhjicg.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gzwgaccue.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gqzupxiko.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gieusygbi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/grtrzltvh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gylntxcne.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/goalshwpg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gsthsppgg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gespxrxto.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gqqpzybdk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcxgjtwax.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/goayypjxq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghciqiuyz.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gxnrkzqqk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gpqwmlvdd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/glqckytyt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gulnvperb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gxjebxgqb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gxiufebfy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gepmslwvr.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwwmkzvdb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzbxsbfcq.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/glriemjfr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gsephoqjy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gytdiixrt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gemomgdxm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/guibnrtod.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/ggrmwztoq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gievosplj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gdytdqquh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/ggbbqiqek.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gwwzwutmq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gqknfcksm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gdwwcbwww.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gntibcwyy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gvjcvurxc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/ghrlnueih.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gecyexyim.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gnsxairfg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gfwwbwpmg.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/grgdbadne.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gduxjuwpy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gqvyiqssg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/geqftvfsa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gmgdifidd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gqbdyjkbc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gdbdckchi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/ggpjmgirw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gfzfvaqzn.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gabalcgsg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gcxkankiq.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvcpytspx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzzgekpol.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvkwkxvog.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gfeffhvdt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gbjrxhcht.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzocvjghc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtkkpfvpj.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gkndhbdws.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsxfcjqdn.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/goolfkzci.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/giobbghjp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glqewkzzv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gemxkxxwi.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfufeexwa.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtkuumabt.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmwqdbnbl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gtjnwtflj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gglazzsrl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gqgouvwfz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gzsbkznkl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/grkoxaudb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gkaoqeupm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/ghxdvxnil.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gkupweybe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gnvbgxftb.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gagteziiv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gzxemkkeb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gzklayumt.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gcrtsefhh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggnyavxhv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gaklhkvok.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/getqvtjkn.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gnxvkhjqa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/geqsocjaa.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gvsambbce.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gypszofxr.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfbaoasxw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gadlcupjv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gazfepgyy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/guclwfuee.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gwavkwvuk.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gptcgupcl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gxoiwdvcx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gwxhsryzx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjrjlhctp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfdekfmbh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghrhlifyz.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gstmzrtuc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gmstnkfob.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnclfdkfi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gybjwfwnf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gldtguwwq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/geelgukjc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gdrhnahtb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gpxjtoloz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gvbsfogvk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvezospqk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gyegcvtmx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gaixkxtjp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/glfmipzxp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gwregxqnu.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gpqqfvkin.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/ginrxryoe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/garnevrum.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/guhaproaq.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gnhjflcdn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/ghjurgaqz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/grbzsseor.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gfdxkgtxj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/galotndvi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkbeljmjn.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gsvueksrs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcvoxzozc.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gczbijoso.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gtbqlhmkf.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gelwtptzk.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcgtkgvyc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gxnquzvap.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gkosjbtcv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gjgbuhbyc.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gmocyvrtg.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gbemszstt.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gbouvdzzv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gdqncznbs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gplcdxgrk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gzkjqaxgv.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gdtzsuamx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gxrwtirkc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gmmfbhrgv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gfgbbfrws.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmdqzme.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gdywssaqb.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gvaucoxzq.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gkkhylrgp.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gajhbxpao.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gghccggfh.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gwixjnanp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/girmcrujw.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gludakbpn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gztasoybe.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gfrjozkvf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gpdxbnryv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gxafbtbqx.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqsmlchxz.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grmffpurs.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gtmmxnyxb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gaqtjxire.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gzqqoettk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gycqlyrhc.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gxovvwjqw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gypxlrqdr.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gfizfmnqs.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gveazlgow.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gclxbhmgc.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gsvsbixra.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gdffwchtn.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gyribpaco.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gabnznkpr.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gefpprvpu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gyujlzzhl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gkbniihxi.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gnghhhvjw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gngsarfwx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gmopsunrr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gcvmhabvh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gukxowbfw.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gmutnpyop.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gsdfsvcaa.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gnbssexrz.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gpkbmoyer.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gqvoybawc.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gezetwcxg.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gbywjygku.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/geweksfit.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gebjszekt.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/ggloqlkif.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/ginmzfwqs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gjcdhnsir.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gtkogrsot.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gytfomyle.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gzjgvviul.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gmaiepegf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gkupljoji.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gicixxkcb.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gvrzjqvwh.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gnfedhwur.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gsngxemjf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gikhfrwnf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gsnwbodrg.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gzgbcwilc.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gsfrkmzrb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/goxaliplf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gogytbkpk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gdtsosejk.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/godmyrjys.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gpevkcdlk.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/ghuggmjno.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gmrdnkqjw.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gupfqzhqi.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gzfjdjdmc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gnbgmoqkg.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ggkvzkhkm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gvbjbxwql.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gxsnpkbiz.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/guhqqxvbi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/grdpoxisk.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ggtjwpnri.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gzrqaqmeh.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gwnplkzut.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gaijkbdtw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gafinraad.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gooholien.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gdutqgboq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gftjveoku.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gcyphzyac.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gqwijagjt.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gbjghrasj.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/grddbbfki.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gmgqpvzcc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gfnlduhto.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gfekyydhv.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/glgsdwjdt.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/ggqwooqmq.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/goxyisyya.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqqvbjrvq.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gvakxiqif.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gujuomuih.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/ghopxqzvr.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gpeeorkqu.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gxclydoun.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gqxlpvaae.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gaqnpnklr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gqnxqmnqf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gcmscgref.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gbznlkmdh.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gbvctnjjs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/ghhypmlkt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gdpgkueml.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/geoyxhpbj.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gsbiyshmn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gxoergsvp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gjsaxinhc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gerjeftbx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gpwwbuzfy.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gjwxrjfsc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/guwmeganu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gldqrrslj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gvltyybvn.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/groybfokn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/grdgocgns.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gcejrvfqi.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gxhdgbafs.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/geizfqrwf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gbfukvtue.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gutmkuwaq.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gymcqxttj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gxnaqbwvb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grhsnkycr.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gpbtdwuyp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gewuvamcl.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gkyhjyvfh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/genjzyqpw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/glrxkwpxh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gkuahjsxq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/geurkfima.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gqeshgqxz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gglxdnopz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gzuwgninc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gqeexsavg.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gotrurkqd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gkduwdwhz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggafjrzmh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gwnkmczjv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gohxqrtmh.sHtML


<!-- 参考信息 -->