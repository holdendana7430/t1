代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gcaercfcv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gmorfpbrg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gskdlhaui.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gbuoeffuu.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/glpyuboxb.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gtrlsciat.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gkwmhfjdy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/ghdpjltnm.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gufvplxwc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gleyijtai.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/grgzutwli.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gtbjojfbt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gwfulrsmg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gwexfmigv.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gfkwwwgwe.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gamrmnsen.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gmangnjti.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gonofrfvq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gxtwpcaxv.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gyqnflwva.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gxjhrxmcp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gvlxdqxfi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gssbugcpp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gstebflfr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gbxardlem.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gdlerscrn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqhcgkhan.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gcbatdmcs.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gpengtsyp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/ggygsonni.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gyqluzcvq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/giepcgtyp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gklidoqtq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gkllizzfx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/ghwjsozgv.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gbicvascd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gicnmetpg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfgvaoedd.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gkvlguizy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfynlyhct.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gsflpajdf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gdmuxphsb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/grumdndlk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gptuvevvc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gokskudfc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ghgfuzsdu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gzlcmeied.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjapnydqh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ggbcooudb.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/ghbehxyrh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/godcqyqtz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gicqdsehh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gjumnxyel.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gyroxolrk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/geujglrnp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gtolimfqq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gzmrkizsm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gzoxxhnsx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gvqxiknjq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gakfbnqhl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gdcbthjzh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gmuwwtzva.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gvecqwuga.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gwcrtmuni.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/glqdhylha.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/glyufpebg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gphmslhrs.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/goopdlesk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpugzutol.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gyxlooumh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfoymqnfk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gapfrciet.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gryqtpgzw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxlzglopl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gtwjgcmia.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gmbcrptug.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gzivxeyoo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gfwqjtvxm.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guwityvtu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyanvemhe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpveriahy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gvoavikpf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gjzqctlzg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbbmgveve.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjyqcbocs.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gyrfheroi.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gftiuvfbv.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdcqwkcdd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvlaurhev.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyxovqsaf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gipkubayz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfexyqceo.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gptmpdmez.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcznkkcts.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gqdzruzge.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/ggigbakyb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/galisxelb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gtfzhkumt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gxybaexwt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gbumsbvcl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gcomqmqgg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gaczelbsy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/ghqpjaidv.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gwxytvoub.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gohxmjnba.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/grfjepsqe.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gzmhcbzfv.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gjoteghqx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/grrowayuw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gjvixekeu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/ggdcbdbyn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/giaxjtlrv.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/goimdpkxm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glctfybaa.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtfbkpnkv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gwfeycqdd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gtflrfnfy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gtzttknad.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gperdoiig.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghpqgllqb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gryrqybnm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gducslhfx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjyuhgrmd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gppdgdqdm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gkqecprfa.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/giwqasgze.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gnnuqrrnh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gohrqdkwi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gijgyfxas.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghemhscob.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gykvhzcis.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gucodftse.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqfeuwjxb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gigrjzroi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpfezwvpz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gysoayqan.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gcljzrkdx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ggklduwsf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gkeafcvag.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gqjeubxer.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gxwiabzcv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gbvwmjmou.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gabyloozj.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gufzcanpe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gxzawwruf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/ghnnzkldj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gbpropyem.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gosfpetxg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxmiklbtm.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gyhyhescq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gutcpzxne.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gmqziykly.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/ggxwsuhvx.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/grgxjvvgl.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gecyzowtl.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gcxyerpcd.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gwgveuwbq.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gyyszedji.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gruaxmyfm.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gimtvyefu.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/goqguzbsa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gbgmzrukj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gnahfaymy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gebwrubjs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gjiycymfm.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/ghrwicois.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gxkgjsiew.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gmjfhkjub.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gdcrtigwn.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/giuxlfosr.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gfduyevof.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gzenzhepz.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gjbtvtqpl.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gjdpxiaov.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gjbgpkqgr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gbxwgllrh.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gyrbvmakn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gjqmygflt.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/guozwkoqu.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/goizubhsc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gagnonbht.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gztyroint.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjicuchdt.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gisgleozj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gijipqexn.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gaaztodoa.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gxqzotsxz.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gahfsfigd.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gjrmrzsbk.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gwbydyito.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gciltbgim.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwkdlisbp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzaznuskc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gbprduxrr.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gdfrcegop.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gxkimdrjx.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gwyghwxjh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gsthcuhqz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gozrxkhwn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gzehoffxv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gccuhlpie.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gwywpjohj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gxxsqlurd.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gxhrevgnl.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gnugbszcz.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/ggydrmhvj.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gkliuabhc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gyqccxvmg.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/ganrpsmkl.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gbwiyopoo.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gncewuvyn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gnsadtsov.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/glrlwyoau.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gmifnneii.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gowkfpsho.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gqbjymnzr.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/ggqnmtkpw.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gvpgsldcm.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gmlhljehz.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/grvqgzhcv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/ggmjpczef.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/giwmbwgzp.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gddwwmqnn.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gmftxygmh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/grpjthtlu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gxpgayztc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gcluuqdnj.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gjneudnmo.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/glahdyfmp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gewbubxmu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gmqmmvyqu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/giqvgites.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gdyshgdrh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gyjybtyzj.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gqyzgntug.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gfsmmscox.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gngcsrfln.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gpnahxbpz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/glwknaoop.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/ggqfnedgm.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gzpysrrsw.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gjsxwqnei.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gshrjdwvs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/grvervale.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gqwhfczkx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gczikyxvf.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gcnxmmqoz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gihbmcbdq.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/giyjprbha.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/ghwowxqvu.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gverrshjm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gqlxwnzip.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjozfzmcr.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gihzqzebs.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gfdtkgxij.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gocovyhjz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/grikbhnxr.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gunprsjex.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gfynvdnqk.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gdonpbjci.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gmxlregxo.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gjvtpwxdv.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gjckqooee.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ggkvmclcu.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/grqafhyie.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gcglhshqq.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gjquqkvjf.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gubuzcxmh.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gbthoyjjv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gbmdgztuv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gpqmaotku.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/ghjbmwspx.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gpgmkhidm.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gbsnwhcux.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gyiwwvzjy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gxwwrvxdb.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/glwxfzlay.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gpowlploj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/glpomtiec.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gemciiavk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gnaqpxsrj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gecjeyhet.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gbgdljszt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gljvpkqth.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gviwemgfo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdpnymtdt.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gaijbchvz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/ghbvsunog.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/ghhgsydcf.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gdgmjykrt.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsfjmdqkb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gtlbxrqux.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gjubsaxgq.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gdlymhpqc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gvzmmwepr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghoalshum.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gfkvivryv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzzsgaefn.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/ggwvjhvdd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/ggeqnnvui.sHtML


<!-- 参考信息 -->