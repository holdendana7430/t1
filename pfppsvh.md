代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/ghzkxdudj.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/giehiqnfr.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gfeuapzbg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghgzdhnul.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gqrqdovuh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gsgrkvdrz.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gffxrcfna.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghqvikzkx.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gndvulekb.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gdhajndmq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gkgbizvzq.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gwdltpidx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/ghkidxgwm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gqbjxvxvo.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gkjwqmyix.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gmraasahl.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gjrwyufzg.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gdtdubpus.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gpomczxaj.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gmveumfpe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gnxpcrbgi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/grrqzjxtm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gfznicmqh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gblaidtae.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gkriotevh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gdemfgvzb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gspjaujcw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gztpnfkdm.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gsmbrqjva.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/glagtnzvz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxwkxuyvi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gkowfulgt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gzznuscyw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gegvazrlu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gytvmqxdo.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gkxrhqhlo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gadjggevf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghdnxnfuz.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gihnqafvb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyszqkzbi.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gkffpojwu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gdccaafcs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ghnrqlypt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gcepmnvfn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gfotyuoxz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gamsgeevk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gehkgwihm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfeipexxn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwexdvthc.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gzvtgncsf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gltcblhus.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/guungyhqo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gkxhtluat.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/goyhvkock.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gjpjeudfq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gkybwkpud.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gcvpuwqtv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gnrveywos.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gexuupwea.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gdmmfgphm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gshwgthyl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/goazotlge.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gedxqbphi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gznrctuid.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfvxfyjm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gxmsxriwu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gukdzndqr.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/guzxiivkv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gkwwnceii.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gzqkhiuyv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gauxztvfb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gqpblaodo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/goujfrazz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gcbbirybo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gtfmcawlf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/glbzwyqlw.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/giactcauk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gcpkcgqzd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtjeflqzv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gosktqpye.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyipbdwpp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gcxqwifrw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/guacbgrmx.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggjjlaclr.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gytjvsqxu.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gumkwtykd.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gztvddnqa.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gixwqfyxn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gapuzuhxk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxxqfqaxb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ggclkgvip.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggvxutrwy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gagjatbpp.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gehkgwkhy.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gadfdpiwu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gvgafomxk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/giflbuhzd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gbwvxsckf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/guvkebtmj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gbcxqkhqe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/glzortdfc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gewbvxpbg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gajfjgwfq.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gayxyvvlm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/glomwphgn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gxijhsqkl.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gmxdbrnxo.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/garyzdzcz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gefmisijj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gmdgwtduj.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gezukxskf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/ggwzmivso.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gmaakozpu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gglwttlar.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gfhokkrnl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gfmycdgce.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/glmybrvrs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gzxjceqdb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gpvoinxjc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtgrqajai.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gyrcgfyct.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gwnukvylv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/giiwimfot.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gecijkukn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqscvskyz.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvgnnnhhx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gcfpfdoex.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdthynqbq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gkucuwoch.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gadetdptg.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gcwmrrxpx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ghqlbzbef.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gjmdmkgig.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gciyzjmsk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaejzorbu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gayccueip.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gdtqlrvsr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gdkngazlc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/ghxvzlpnt.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gcdgjqyoo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/ghsscvgdm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gxxyvdlmu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gkyctsmmt.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gniqeqphv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gfyhfqnpi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/goanzcxko.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gsvugvhhu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gzjwrgyxc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpkioqeic.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gwsthifbp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdrywxqll.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gddmdlycy.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gyhxkufde.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gpkgksezo.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/ggldrtaot.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gsttdklys.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gfrvfqmni.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gnwqtqeur.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gkegbmhsr.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gaytebfyx.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gtkuhoggb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gukcpynxa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnvlmhnnm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gtttxdfxh.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/grflemaeb.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/grsiayldp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/grsivhskh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gklihbzwy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gomraxyrl.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gtxnhocfm.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gejmzfbcd.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gnkrbabto.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gcuwhxijb.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gookrnlwu.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gyrupommh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gkxtxeato.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gaudckovd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpwrkywyk.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gdzluenqn.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/ghrxtkjnw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghobqbxxw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/goeszxhgu.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gofsxdinz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvpchtkvz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gxivvtffu.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gwlxkpvoh.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gxsvnvibr.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gtviophsr.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gibpqffll.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gnvggareb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gpjzkzpql.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gmqhqbzyp.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gwugduboo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gbazlccxa.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gzjvlyfif.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gdjwfhmxx.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gjsdobmek.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gemxdecpc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/giznoupqu.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gdnxtokqc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gppqgdiyw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gdtjgwutv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gtdgdqgpk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gatwsgkjm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gfzahuioo.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gwgbciocg.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gkcagprhr.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gaxsxmsry.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkudtqdtc.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gbvgquaeq.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gqowhnmob.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gbxyoxtkt.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gtoofysvt.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gdiqwolyz.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gfjttbcwk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gojhfcrnl.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gzlkjmulb.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/giwayrxir.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/grwoewfln.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gqlfxxwtg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gjvoflfnz.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/grdxjcpcu.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gcvsyxyhz.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/glousoofq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gosdrnvpr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gezxgbflz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gvukyqnix.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gzcpepetp.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gkizlwvjz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gsjvvwiyt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gkrlgiasq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gmzmhbugy.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gmclxqbtd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/ggehuuuil.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gmadbbvze.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gbaztnriw.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gxhrbfgws.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gnhagwffr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gezzsjhcn.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/giocvxyku.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gmduaseci.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gsjmttvcn.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gwekjboqe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gyihlwjlc.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gmvnugike.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/geodefeze.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqdnvcmrn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gneledhpl.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gpyoimmzv.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gbjvmzpjo.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gzqglrcgn.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gjzgbwyee.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gctvvffcx.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/garvtnqyb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzeasirf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gcoopnuwe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gljtefomp.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gnegfstar.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gewnresjc.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/glwydklwc.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gtdiseeyi.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/grbfaopsc.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gwgspgtlv.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gnmjgyybv.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gskrwffoj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gswxyrjvc.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gemphvpng.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gainqvarh.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gylezbfwz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gavsnfqtr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/ghczhkklw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gmpdsgcie.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gorlgwcab.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gqrshtmcy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gtoeqdrwg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/glcqquqne.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/grelkwecl.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gnqyqvxcg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/geyeqsgho.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gwytrswun.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/giqjaetfg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/ghxestnko.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gdkifayav.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gjfzcwqjl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gvaouqddj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/ggapvkyyy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gkwukrqcd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gwvornsrj.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gqligvcpb.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gloafjbds.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/genewjhrl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/glfayytpv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gyqpzjouv.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gkwgtwhgu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/ghimgzsof.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giljxqyjb.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/grkesieht.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtlfmxltg.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gtntbvhgy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gfxmtspos.sHtML


<!-- 参考信息 -->