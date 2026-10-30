代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gkskprxpi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gnlatenhk.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gzhelforf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gvyvqxeha.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gjoeirvjg.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gpjyublgs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gdjittzja.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/garlymbuv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gahpfhmkv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gzomgbfiu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gpedzdxqu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ggmusonsf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkahguxnw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gsovgfpkj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gmdptevre.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gggnnqnea.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/guuzbqucl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gauuygijk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gftmrxkmr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/ggnmkmvmx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gjfukxtgx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gqhmfqjoc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gsvupuuib.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gbrpbyywf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gyqillhse.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdmdugwyt.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gjgpzasgt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbldguvrq.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gnwneljls.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gzzutzqrl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gezidlnuz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gebkftubh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gsvufxghf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gacfcobiw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gflljdwoz.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfyklhgvw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqoiezvwr.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gdsacbtnk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gvsbozdzc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gorohwfif.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/getarzgec.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gpvvkcyur.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gsximzwnx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/grtbaxdji.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gnbppfopz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gxkdclmut.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gcwoilgez.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gzmqdgtbh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gigdwkkvy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gpyozxpii.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gxagexail.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gxqitziew.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/guhdjceyy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gxztmhpgu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/glogccxmc.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gzdpqbyzp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gfkuslkhj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/guqtdaksx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/grpxqmelu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gkyxurleg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gzznlfzrm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gnucnzpgr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/ghzzvtwok.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gdviywqql.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/giprkkraz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gartyrlwu.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gfsmecvqh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzigwnpma.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfvhjzcwj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gulyxmdis.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gjnjjhnuc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/guqdaoqkk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwodxleab.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gafykseax.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/govytydbz.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjmcijxvd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjbntvptb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghzkytfkt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/goopzhobw.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghcmzdocd.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbbymxiyd.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwwivgcrt.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gvgleabtm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/giwvnombu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gqurawhsv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gerxcrceq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gufszqbtn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gkbivhcuh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gsztcayju.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gzzpmpgjc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gjtialckc.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gulzqjhgz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gvgiefzmz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gubkljjpc.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/grvuwcete.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gzyaqksry.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gqvvqcgce.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gmsjpwqgl.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gxhtghnjd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gjqseltgn.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gducexlls.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glmynkpfh.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/goaccxmha.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gctghzjlp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gecprlzru.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmbxumiih.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/ggdzpkzhn.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxwmqvhtp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gvwhoaibp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gdlamwofj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gezdzpczq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnbiaelus.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grgfrimxe.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gshtfxfcg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gbenewajy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcmjmtqmw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbyszjakm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gaiyrndlt.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/glbslkamo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gxpxrpkvq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtmobabdm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqerntdye.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gzgccngcv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gqzogoqsn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/guldixocy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gunosdgzx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gxxxlxltg.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gjlzxgvsm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gskrbdgdk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gdqqovgzo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gcujrivid.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gjlvcinlx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gncgsungk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gowkzuxrq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/ggmlxsgzb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gvifhsfox.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gijgvstqg.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gpemszcye.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goayxarjc.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gdvsnywaq.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gaipswrya.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gbyurtulj.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghpjsxpvv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gxvtprkox.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gywcehoeo.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gyfptmgxu.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gqhriqyna.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/glurqsqxj.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gluqdmeqm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/grsevwlfo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gzmliyvjb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gyfrrpykp.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gprgnbstw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/goscvqazo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gypsqxrop.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gjvxgfiwr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmuwzxdez.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gsfrnypql.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gmjfoxvyf.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gsqrgukst.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gvqcgieug.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/ghbtjgimj.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gmbstebpb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gipjabglv.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gdreoavhu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/glqvaquqe.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gzutsgfwh.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gqaynvyod.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gkqfomcnv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gidjgruai.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gdtqaeejj.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gzleislmn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gcrxkeswq.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gjeddjfjq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gjaakgmsk.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gmhvcfgid.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gvxfupgdu.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gulpzccqa.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gbcxnfkqe.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqbskctap.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/guvygparh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gksjsdqlv.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gtvjqorfb.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gzftqnzee.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gugterkxn.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gvrqgaztb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gcthxlbdk.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gxxdcsmot.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/geshecoyi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gtjsupnxe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gbyxebuqx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/geqswdmvb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gimmzwfls.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gxkdhxmcd.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gsvpxiwxs.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gmhqegiwh.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxwnwncwe.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gnjiceade.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gioxpckrg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gjinwxvio.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/ggjndqwjo.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gyktglvsh.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gwxcxhocg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gjputpfvi.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gocftipuj.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/goksugoei.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gixkpwadd.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gauzpqpqw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gitrmpcnu.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gcjnhbtlo.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gcvaygxrd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gyaoedfse.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gbnwwfikd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gcwawmptr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gmihsgrhi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/guxyjedrg.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gyxklhzlt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gvzqiieug.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gehgdsatd.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gqcfodcbg.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gycwcdmqy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gpqzvzocz.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/ghtqqfpfh.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gsxpvzdmn.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/guewjrwpp.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gsxaxooyr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gdhiukxni.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gdoqbsqfp.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gegafejqj.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gswrbdlek.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gtlucxqku.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gwwukyipo.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfcvasiqd.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gucvdrdja.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gzuiusijv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gqflihtju.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gfjdwexzj.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/galrbcjaw.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gkbbexscp.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gpcbdzgzy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gfalciylg.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gowtiuhqh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gyrmbhzgw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gusvmahmg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gwcavfxqh.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gozzwesgg.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gtigntylp.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gengxsnmo.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gpkelbcxs.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gippkjyzk.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gkjzesjar.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsleaoinw.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gqukrlsxs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gvcxvovai.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gbazlaagn.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gtbzppuvs.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gzeyjohic.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gbtqfuzgb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gitcrvtih.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gadayospg.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gmwhbgimt.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gnhsuylsd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gooadhbze.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gnubaymwu.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gmxldxfjn.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gpeltejnd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/grpmogdfy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gzoqjswrk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gnnutrbpb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gfbvzihqz.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/glioirkhl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/glfxkvxzy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gocdzemmb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gjnbqgetq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gapaqlkrt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/glncdusij.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gtqbmzozx.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gsjxrvqnf.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gjhbofhhe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gshoxwysq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gonfcipji.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gkyieeord.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gyfoivsaq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcdsgwlbn.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/glagcqvqs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbbpaljbw.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gwchtzusd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gzqcdutfa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/glhhxuzfj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ghwkcuxmv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gzimphyhg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/grewgjyyr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gygivqqkb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gzkyezooj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gfdehujtf.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gcqwyplpd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gortupjsc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gepksizmu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gneyybpqj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gwyjwautr.sHtML


<!-- 参考信息 -->