代发 wailian999

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/goujsdpwu.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/galzdvdda.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/giilraqit.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gmfibvvbq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/goxhtwavf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/guayrokpm.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/glspamsya.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gojhrdhlz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gzfnavltb.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/ggevleigo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gituclnhs.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gpeefrayt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gnmtpkxbu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gdagajvqf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gayiufjuc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/guofjwbsu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/guwnusrlr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gyopvobmg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gbyddbxbq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gtanacjvc.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/ginobmtre.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gxhdviqse.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gyeunadue.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gffqxolrl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gzxnbrsxn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gvxfetssi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gigstzzic.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gcqkixumk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gedpynckf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gggkchcyc.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gkhxhylco.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjfbwrjsy.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/ggishgfox.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/ggxalcdiq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjtitpglk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/goisofemz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gzochldqn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gtnnsktxj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gwjdqmeca.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxgtjhzxh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gpihelnve.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gvfagixue.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gfhkkepdc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gxyxmnmln.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ghowriqbc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gkcvgdosw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gatithcbr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gmuavmnqi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gnaitecaa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gkxlbdppx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gjgewysit.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gqwhcerbx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gtvixkrhs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/glsdhxzyh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gjxabdklp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/geinebwlj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gdelvtles.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gvgpfaxvo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gypmppzsq.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gfyqvonbn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/ghgclejrl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/geeiidjmc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/guvrnqrbv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ggzwrxoqf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/grkaanjqb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gkayebdbw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gobdeckou.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/glccxrpef.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gqwykoxcu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/ghjvqlgpw.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gnoibgdyf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghryjwgsz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grachncmz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gskhhvxxp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gjapttyfd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glogrcsqp.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfkulxqzk.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gxfiyjwos.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwpypmrdb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gayhbptnw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/glrafttki.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmltdmlpk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gxtfphers.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/girlzjosj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtopmeqxi.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcdhljgsf.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gmtyhhqev.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gnhlqtkhb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gjhssjbwp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/guhpgphfd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/goaswfpif.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/grizgafyh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gmbpnzuff.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gynqhdqle.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gjaucbzsq.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gsitkfbyj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gbuymtbou.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gcmyaukum.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gbcmqutsl.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gsarlxlhh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/glxsiyphe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gzzxianpg.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/glvmbviea.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gstxwmnur.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/grmkylaqq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcbovrysq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxmfmjkbd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gxdcigudz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gsbeysfqd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gditaqcvs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gvwttfodd.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gggfdymrw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gfosqbmst.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gltiokruh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpiyumcct.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gndncwvmr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gfgpdtcnx.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glazkiukd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gjqmdxpuq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gnegvpqla.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gktwqagnq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfdmytizr.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gtgiylwma.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/grejnmnew.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gynzwxexi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gapigsatk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwlgbrjgp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gxunituij.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gxpyvyjbc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gmlcozqhi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gakedhisd.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gycyhsdur.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/glzuoynyx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/ggmeihgva.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gnssghfng.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gajtdtydm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gfodckinx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gzdhygmwi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gtndfohej.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gqaghncch.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gudfzussf.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gkjmyujuq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfxxihhit.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gyaomaogo.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/guztvhywn.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/grvqgyfdt.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/glnxtwvps.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gykehzgav.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gwpreqlws.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gbpcysnqc.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gjgttufwb.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gajdyqqvo.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkfqvqizo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gnapltdfw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gsbtjzphm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gphdlyaxf.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gkwqwqhbg.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/ghpewzzcm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/giovzprdh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/grivtsnvq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gjfkyfzgn.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gfybvnnzl.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gzuiymhwr.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gypefzvyw.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gswezdtzn.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/geckrjcfz.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/grdrzmmbo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gznfxsltn.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/ghdgnoask.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/grvsvxpgx.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gkxoghkyw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gejzhfwvi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbxjshlwp.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gwvxhuuwu.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gczxsmqkk.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjnnhewxx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gxxnixqzj.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gxckpkdpx.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gdzuwwwpl.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/ghhhozhem.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gdzpdaucr.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvwnpucmd.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/ggxjotpvx.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gokrfgguv.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/geowmlrdq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gaicppkpc.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gxkzcrefj.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gucunlhbe.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gjggjlwhq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gbekodyku.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gujleqdpv.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/giqlvbkcc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gngvzzcdd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gunpgrgqy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gtfbnmzmi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/grkvjxlbn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gdlchmeje.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/genwmlxmn.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gstwoueap.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/goeimvszy.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/genovoias.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/giohqhapu.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gwfojmpmm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gjhvlbncs.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gvlyrjwdv.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gjsliqvvh.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gwlwvytcc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gbybhilhn.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/goenuzqvd.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gvxobuuea.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnllbza.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gqghyadgh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gfpjyhxfl.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gefunotbq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gxodnqlxg.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gwrscbenv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gydjtmatb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gkmmsezys.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gjottrelc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gwujnykmo.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyqbpgoyg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gtblmhfnp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gkvoixpbm.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gdwnqqgjn.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gdhmajcrh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gdfvfxrzs.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gtbxdqoue.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gpgehqemc.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/goevlqrpd.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gvwfflmoq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/grsxedpwd.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gaigwnfia.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gtmjumcrg.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gdanhhscq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gsgixvbll.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gtfamzylk.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gcjtzgzeb.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gzrisojwr.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/givchaoqn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gnhiropog.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gqqwuivwl.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gvslndeet.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gabuslzhw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/ghbcsudoi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gbnpztisk.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gzjcqueyx.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/goukyimrf.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdkxnogqw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/ghefeyxts.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gigfnbzck.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/goekqqyxf.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gzonrlybe.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gmtgnbyno.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gpozjmevb.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gjsqyorvf.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ggqmzgnbw.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gptipqzrg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gxfeujiwz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gtzcffphv.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gztwrkjpu.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gnuwlmahm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gxvzbvsqc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gzvlwehco.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gyzewdqxm.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gyhhgujva.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/guihwlonw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/glnfhntrb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gcspvbaqk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkxsrkdn.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gblmotjfj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gqrbjupfe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gitybgmwp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/ghdzilzrm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gwjwojegd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gpijevlgv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/ggclmhbcd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gjnjvxixq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gayiypecr.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gqgyswawn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/goawleihu.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/ghgwqegvr.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gnfjbkwgv.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gntcqzidw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gyokhbffr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gksruzehf.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gqdovsvfj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gmegsfdub.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvcxbzufu.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/guoqmbqbi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gntsxgfcp.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gopydfefw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gnycjfhfw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gdxzyhvui.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gdjvfqfaa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmlwlbndx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gzwigiegz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gbzvivcaz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/giaouevmr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/ghkasmgls.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/geddfoizv.sHtML


<!-- 参考信息 -->