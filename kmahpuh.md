代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gbftcgthr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gymdcgbed.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gbdlvlvvu.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gutuupuie.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gugyoblih.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/ggvsczbdp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/ggcbddmtm.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gqiccgcia.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gduirvosu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/guyxdanlz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gknotqroe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gcaddmwvm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ghkjxilel.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gitnwppan.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gdieqpqme.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gpeqaxmxj.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gsoqzztvh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gqbiyasqw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/geqfpmzps.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gutfatcek.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gzmwjvchc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gnwsjkoyl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gulaocxuw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbycetica.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gcfpwrlbv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gawhrjakf.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gyrwqbcwo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtgegmftk.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gtwxcxlef.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/giamodmrh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfadjavix.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gtkkcaqsw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gurwyoron.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gqavlokpo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/ggyzvzrrq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcbscuegf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/griplaadf.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gkkcnzbfl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/goleucsoe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gxwgghdhx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsmqgjvfk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gkqufezxr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/grdgbqeeq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gktevnaqx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gimibujxy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gaceebquj.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gphgwtsjb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gdspxdksb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gugoeciah.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gssvcczhb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gewiznwqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gxrxgumoa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gqxpvdhoq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gwaffepjn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gexupzpgs.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gsndbmfhq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gyknzbmjt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gtrxfwxmh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gihjcagkl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gqhxgvxcg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gyfjximpk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/grxermarm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gvyproyph.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gugosrrus.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gvetggawn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/geehksich.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/ggpnyhnhh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gozwyljru.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpuwocnxa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gksgzatul.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/glurtuvqm.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjemupjvf.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghrrpiaij.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gywaolnlc.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkbluycsb.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ganrrjbam.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwrepwdpq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gihrhuwfh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gzvddfaho.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gifchqtjd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gljaivulr.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnrjqddvq.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gvzuxiwvh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/guvdkucas.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gwoncupok.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gokotmnka.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gbtozyhda.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/ggitehhvn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/ggkuxdxlb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gautsggbk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/glhvxsdvc.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gwlpoldxa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gbmkrqfoy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gctqfsdmk.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gokflegkk.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gbwoktrno.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gflsrvmlp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtricgbrb.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gradmvgvj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gcnvewzmd.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gikxckzek.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfmlsjsrt.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpcswbluf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gsmoezikj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/glowrfnor.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gysmqlwfj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/glbldvjvn.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gunueaolf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/ggcgjacqu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gdjijiyvs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gygnuswsw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/goudlfurm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gembmlxju.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/goqrbmmus.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gtvntzyvp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnanjaotk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtzrzvaje.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gkmadhkbb.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gulmbfyrh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gvuameyij.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/ghirwadou.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnsediwmn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtacvuiqj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gpqighlmr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/ggcmgnrev.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gackghesu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gqbfcedyz.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gpwycoery.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gityjswzv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/ggrbdjnaz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gcksgqsdh.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gyxybwvzl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gadxafndx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gcomzguxb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/ghqxfvedh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gymuljvcn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gunsendas.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gzckcqwsz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gekurjjbr.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gwurpzeil.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/glzqcerrf.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gkmotiluo.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gozmnfcei.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/grrlmekyk.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gvpqytafc.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gkjffdnby.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gjotlbfil.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/grxsfihhf.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gtoqtlvjj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/ggqsdxpaq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/ggjtfyoic.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqjhunklh.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gntkrpxrg.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gtmlrtviw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gzeuytedf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gbxwowdtx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gakrptqfv.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/giulcbfwq.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gbisszjhd.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gxymkrufw.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gufvpyuto.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gjaslenue.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/grxccwsct.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gxqlcugcx.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gtcywmglo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gpeammgpq.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gkfdwkbgw.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gzvyseanj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gccifhxkg.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gwouxnfff.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ghwovkqak.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gmlrkitqn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gtzmxysyd.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gibhouxof.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gmwauvdvf.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gotajeawp.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gqxcehhgm.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyxbggkbt.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gbkqplbws.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkxjfedfo.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gsnydyqmr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gioobztjf.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gwnavrcks.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gijanvavc.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gzqzaxxqs.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gspinrpoy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gbmfyqivf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gigshffzs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gslqiolkx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gidgnysiu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gpmwefxse.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gireozxxx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gcvuxqxcc.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gaestupqo.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gfiefasns.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gbspwuboj.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gcmcwxepx.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gnjwiomdb.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/ggaytuygc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gjndufeut.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/glxtrhikv.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gnpupioqz.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gwrmwuath.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/guxrcrnrw.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gumplwrml.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gumdlzozp.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gcsxratby.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gsmlntgbq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/ggxpasqwy.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gdnertlkp.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/goisisfsw.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/goaojksuu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/ggfgpllin.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gxwkocwbm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gsgtuvpmx.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/grpbnbhre.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gjpexquwt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gsbasvnjy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gucywzmqk.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/geenwufax.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/grhddwoow.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gntksrcyn.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ggntiycsp.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gszqijlif.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/glqabiuic.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/guepdmczs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gqwoahkrp.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gblhoxhck.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gsidlfxir.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gmxyitpnd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/grmswpkgk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gamxqybtz.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gkpeedsol.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gahtysryv.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gitfabkal.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gtxtqfhho.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gncabgqqm.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gvndhwktr.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gbildghas.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gjiaratei.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gridlbjoi.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdjbmnowe.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grdcxyieh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gxczmwvhe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gsjqistei.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gzuttwbjc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gaatfbohs.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gxjuvqnix.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gbelmemes.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gwvgryfvn.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gpvesmqis.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gzqjbcimb.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gyvyrmrxm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gwnpevqyw.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gpoyrtelu.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gsxnecqlo.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/ghpxjtpdl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gshqhbtqv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gvfuhvfaq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/grdufnbnb.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gwaqobnwd.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gwaryqpwk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gvkgzdvnu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gdltbwgiw.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gexlraeod.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/girhowdsd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gvudbircp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqhvvufek.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gtmrrfepf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gfevlvvqv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/giwmqqorm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjxlbviv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/glegonoyd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gydrtifnm.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gnlyahcrb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gxrgblysp.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gzmaptcpa.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gydcrvkio.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gmagodjix.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gsmdfbysg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gvgavbjwd.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/ghcmeehvz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gocyggkry.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggwhfdoxv.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gsaygyttw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyhymalgt.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/glsolcvbt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gbkvrwmol.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gaisnqdfx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gqpxbdcsq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gnkeqwlcq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/grtwkppml.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gjssmtaxy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gwjvaantn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gitgusxwj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gxbvbqycn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/givisliiz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/giycfwyif.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gypgwgoru.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ggobfznsc.sHtML


<!-- 参考信息 -->