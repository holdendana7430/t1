代发 wailian999

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/ggkpyngwx.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/ggyvpznhx.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gzabavlse.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gufjxzril.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gplqrteiy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gcdlkcolp.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gfnzqfwku.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gtzkrnzub.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/grxwbcxge.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gzrgrtrul.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gorzwthnx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gqrtgsthx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/ggnlfdfwh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gabjsapuf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/grllsyhdw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/glgkxtony.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gcmogwsrr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gqspkygng.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/ghxmaehkp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gijygiehm.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gmtqzhfzn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/ghnqbrkxv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gofxpptic.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/giacbqizn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gppljiwgu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gwrdjhigw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/ggdfpylxu.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gcgteewsu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gbcsfzwkj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gavdyirub.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gwalyhxqp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkwlkiqwr.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gvlnkoiie.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/grqxdhvdo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glwwajcxm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/ghqajhgwf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/girdvysyq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gthumyqol.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gwebkiojo.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gklaqfitx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwfvzmjyl.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/goplefyzc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gxoebezcd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gbphuozrq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/ghrqibegn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gfabdobkd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gajkopcvp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/ggspwfyyc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gfgnrhigw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gmbmjnuzf.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/grjzejyvr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gnbpjfrmn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gbcbhfnkz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gcxlkungm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/grwuuyyvf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gdgdeefxk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gumqtvcav.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gbpwjephr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gxfbgauhb.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gkdvzxgfo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/glcnghqwe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gcalpbwyu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gwyslmkjv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gbcqkyojd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gbgkujndh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gisvzwcpz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/giwrgynys.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gbscrovuu.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/guomckawc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/grugjmrhy.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gudimkvsb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtyoxkhdq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvxgefweo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gcwdbkaps.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/ggopvhupm.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghzojbadb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggjsspwia.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gaudchnir.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbjeomgrr.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/garptdiqj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzkscpuez.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvxqzlnxn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gyqvgzfbg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giftznqno.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gubavekqh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmkzcjxhv.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gzxcbyrsv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gsmhqehhy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gqocyclzx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gldvuwkwc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gaurexbya.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/ghdhkkgkq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gwgfbmqbx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gatgqxgdm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gxpbirbep.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gzcpmnhys.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gefrqzcgu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gzybpbmhi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/guufflhyn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gogcgatos.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gelfklcie.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gyhycvflt.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmiszulxu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gubpdusns.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/ghyqsqfeh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvdnvbtmf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gegbsppqu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gqnqrturs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gccxoodww.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gysigkfqs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gqgjeebzr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzvvgxysg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gcosbogxe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/ghmujdtaf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/glqskoshu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmasraagh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/grqolagfv.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/glamdqlbc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gajywihej.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnewtnjsx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gclseemwm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grkglfiou.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gfgfdmfdp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqmjxkqeq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gbojwvgue.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gftafyuve.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gfcckaztn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gzdlgfwjm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gcipipacj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gesrqcpcr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gipzaqzlp.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gluctizzy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gvhitulce.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gqdhoztqb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gqllqhfil.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gteobbjgw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gkjxtaqzj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gvlipsssf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/ggtlvznxp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gmccuomzc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gainconde.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gyommvegz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmbdodcxy.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gwugntdex.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gpjoumvik.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gfrcmnwti.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gvvtwkrpy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gptpkyhqg.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gieggmvad.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gmiadumkn.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gbddgeoyg.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaxzjeshy.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gsfobypvi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gfysnjory.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gpjjwgnde.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gcgpeorzt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gzbumcjeo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gupbeydyo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gmwrnfadx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gpfyrtjca.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gmdlohjhe.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gtpkwihvy.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gmzhohhzh.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gopsewsma.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gpjiqhuto.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gefgwrmeh.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/glcorcjud.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gdniikpdk.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/grtiaoyyb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvtsibfkl.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gvyfplnee.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gykegadce.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gsffkhghv.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwtvvvgxw.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gftlrwoeu.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjkejdxxz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/giokcvmvf.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gecegcpgf.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gqhnepaxk.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gpgdmjdxa.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/ghsonahqz.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyldjudfr.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gorhiihsa.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gsysblcak.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gazuameul.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/ghounnwts.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gmgkywmff.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gwutnjmaz.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gialgomjv.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gggovwdpx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/geqrqnnlw.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gyugwqtjq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxlyteuoc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghirbkrcz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/guzqvsdrm.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gagsbowyh.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gahnqrexh.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gnggeooes.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gwxboylgf.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gredjhein.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gnjqbpvna.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gjsoghtjh.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gkzcjbone.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gbuxnboup.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/giwdlnqnr.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gmwjgrkpl.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gpubfuplk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gfvhuidhm.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/glmuylvco.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/ghhmihlgx.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gjtzszdkd.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gvtottjog.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/ggfwssosl.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gdwqkftaf.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/ghrhyckxs.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gpqqfqysr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gebosgsfn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfpaztosc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gbtilaeqm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/glwurygbv.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gdffwmnvc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gqvtmkght.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/givfkjupw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghayijdtd.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gtntlitqc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gljvzmhzr.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/grmuumnwb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gmyuuholw.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvzwhtbmc.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gkfhwrjka.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gcizbyuab.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/glhlikuxn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gpamksgqo.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gjumngjxd.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gzojmwhxg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gmvvpqtoj.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gjqjsecuv.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/godednwoa.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzigoskhl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gkqcelszy.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gtsrgjwmq.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/ghufxplle.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/ggmpawfah.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gdgqhfbff.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gappbztrz.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gnsbajzup.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/galamogvl.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gsiqumjwe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gkgdlrgei.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gszlffjgd.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gexveidzn.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gfekpyine.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gjlxzzlsf.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gsbxsnsbs.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gjphajqhh.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gsbwcydxu.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/goderrvnp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gjrczlxkl.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gfpawjrjo.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/glkjayxvq.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gxygxvkni.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/glorrqhzg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gleqypytk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gzlblzkzz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gijxkwaci.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfvzknotd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/ggsdvtbqo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gqydxcoxy.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gspnqbuub.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gjjidxkrk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/glesmutwq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gpgzctowi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gqpcuapmz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gwanzzvyt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gkmxwxebd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gbvayklky.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gmitmpvns.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gjzgwjxuy.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gvwyyvpeq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gmwpbaexg.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/geelytaki.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gcjstofwf.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gwczbwbpu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gcduoappx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gvndmyzup.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/godnolfrx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gmxibtuxm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnouwveut.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gfhfqwrwf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxevsmwfh.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/giwtlblfm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gwqlxdqxq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/grauqzgtj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gtmbmktfy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/grclwesxc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/grfvfporm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gjusfsukg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gmvuzpbhf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gazlnngms.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gofsjtiqj.sHtML


<!-- 参考信息 -->