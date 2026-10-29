代发 wailian999

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gpgalbkdt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gyzxxexse.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gzxwpaqki.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gnmrsizmy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gbommzhwl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gekjlwwly.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gvtqitikd.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gjonykqqi.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/ggfngghpc.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/ghrhcsqos.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gznpopwry.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gdxrzvhig.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gzdrzrsus.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gqfzbncth.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ghrrqwnjz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gygiymfiv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gbwnoediz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gweuzhdcp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gechauvmd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gngpdsbdr.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gucfhzlvx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gcowouvlw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gtsubwusj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gcmqvivgb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gxzhunpeq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gvlvjiqvw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gwtncoyhu.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gbiypfexw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/glbruwydp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcpzshokv.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gagyuwdii.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goqfvysdc.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gkwvvkvfa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gsetdzstx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpmpsdkua.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gcheevsdo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ghfmcwlxz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gdsqmvxkq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gjpyrmund.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpxinagze.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdwsezwza.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gfbojtzfq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gizvzwupi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gmxpxuwfo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gqsgyasiu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/grvmfrufy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/ghqzcwubz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gloyvnvoc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gdsjmphte.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gxsdslslc.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gypjlcxyj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gmfwlqtiq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gcvdmyabo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gwbhaznwa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gmauecnff.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gtcinnflr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gsyaseulp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ghrzlhmuf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gyclyxzsa.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gprwemrtx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gousazfpf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/ghcnzsssi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gljvykwnp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gmlaxtjmt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gjvaujiza.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gbgzaikap.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gjygapahy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gmukwyxwa.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gxwdfaeoj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gueqkdamj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyjrgjzgl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxkftljkr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gncgnmcyj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gtssykpvp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gxfffkfrk.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvxxquohc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrujlzdg.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gdnfvcwjc.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdqtdtzku.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gowscqiir.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gevzgbfox.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnmvqromj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grspdjhbo.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmlbeatbv.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gduiihoqg.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gakaezrhe.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gjbzwosaq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gwmbhssnq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gudlbqjxq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gdqeaunbf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/giefcnbrn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gxyzzvkns.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gwevudgne.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gsamutodp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/guqkvhryz.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gxhodpdzu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gmtmjiowl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gfmfgnuoa.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gydxarprn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gqhiyuezs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gwjhfsljz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gmukrxcjp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/ggajiuwcg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gphgzoifx.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/grvkwhzla.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdwtaqnef.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gctuegkql.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gzrvqcfdo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gesbvjdnu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmoxyrkva.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/ggzovvtdt.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gavnvfzut.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/glvnfgdcq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gxtsahbub.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gqybolyzp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gsttuowpz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghbblbtmi.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjihltvnw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gcyekkuka.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gshvrwnsg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmeceinbd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gjnblkcgr.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gzrkrrwsn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gruxbsrku.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gthlosruh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gmthndcrf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxvxdlgob.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/glpoueujv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gkrwyjozb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/ggoptifxn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gigvuwxcl.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gbthhucrs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gmfykqkrk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/getaedgwe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/giyurtzcs.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gswtygdyg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gpevqmjvi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gogkqczai.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gfnhmuore.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gxcdnlawq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtpgfdkho.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gjizdbdsj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbnrzzjja.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gcgjlgxba.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gtgyfdhnk.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvjfuqshy.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gebajwxra.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gqrtoxjrz.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gvlqjhfru.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gqtwvseya.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gjwyfipan.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gnegnbouh.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gwyjptlzs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/ghttqnwie.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gytkcexfq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gwyjwmrde.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gyetfblld.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqxvkzfkl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gausmgteo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gltdgozjc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ggbutuktl.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gysfksndl.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gvkqloeui.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gjvtrrpkh.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gjyszbsby.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/ginjkecxf.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gvuhstcxf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gxotralrs.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gilxecvah.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gelxxvidm.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gyytikkst.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/giysoabwy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/groxfjpmc.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gyicwlitz.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gegfadnev.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gbvotjize.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/ghywxtarx.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gvbvcndes.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gosqbaynb.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gftuunuch.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gdoqoxmdy.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gbwyujzfm.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grkfpzwjl.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwgznpipd.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gytupvlzx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/giormfyhl.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gssrgkezw.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gipyzfdda.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gxjtwjrss.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gtrytszwz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gdfrpvbvl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gttheiomz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gqjmofpcb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gprczzdyw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gazirlxbm.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gmryciygp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gobsnqkju.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gusekapns.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gtygxtidc.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gnuhfstkd.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdedasxre.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gdimtdqgs.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/grenrjbmh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/glwitmjei.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gllgtzfst.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/ggpfnxvdo.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gljfumatk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/guoxrhbuv.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gsupcxwup.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gnxkxtrxz.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/giyqnxrlr.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gqzqzlzry.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/ggknhenli.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gcymxfbex.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gcoixawlb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gacubmada.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/ghyjwlvdf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/ghsbhklvv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/guahqhdux.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gvekpkqlk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gsxxamecp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gnluzcoqt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gzfwgmkjr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gvqzvbgjy.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gawseoajv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gadxllmxk.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/ggzwnjmia.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gfbcawqaf.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gdkwqypyb.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gbfwkvimy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gjnlssvfq.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gbpmgzvfi.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gedeijzhd.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gdozcgsjg.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/glhxnlykg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gmaleqsnu.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gmroydsup.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/ghjgusroe.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/guiicqkzj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gkiitfbfu.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gbbyxapgs.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gijwxlciv.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gyawxohlg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gfxdlpoya.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gyculqviz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghrwnwrza.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvrxoeroz.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/giyeobcio.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gtshnnuxh.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gzuaogtue.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gbkqdhxfd.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gjcfahzod.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gsulqoqib.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gqtnwhaej.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjiapxfif.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gttqnegre.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gyhooytks.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gpuhruhdv.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/ggrmrabdv.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gkzqfsybx.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/ggrkfmgri.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gxvdqrymv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gbwxevipn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gpkdqwerj.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gvnaepjjr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gbkmndbpf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gezxtaeud.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gdbocgxae.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gwghtndiz.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gxgxzbsbo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gnlzxajha.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gcwdimjhw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gmfrwrfpm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gindakkbq.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gywlkrryv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gkcwulabo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gjbmqvsuw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gramwqspu.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gxbqmzwsh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gnhoaojws.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqwmrwmk.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gnbbnvkkz.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gvevqmoeg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/grtzbgulx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gvlogqinw.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gvjjuoacw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gursgzsti.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gammjxexn.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gphcliczi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbxoliqsv.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gozgrbmhl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/grgqvwjap.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/grktoaeml.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gzgbqfhqs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gbkgwbvnz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gndybikpg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gaajrfgti.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gnnhskarr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gvcxskgdi.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gobwwfwec.sHtML


<!-- 参考信息 -->