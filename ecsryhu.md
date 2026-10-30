代发 wailian999

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gkaosszcj.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gdpshmuke.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gmzhrrpkf.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gwgeotsln.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gklfduhty.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghjgcijyq.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/giukzrezo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gfybnmewm.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gtfnxftow.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gmpbylkif.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gcjfsaqby.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gukkkxtxd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gajaqvpuw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gkcvhmrbh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gatxpzlmf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gjlswzsog.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gffrtqqjq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gpbkgrbue.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtvqoyifd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gjbnxvqzq.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gzuklfmek.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gmirzyaii.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gqqyyptkl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gnsfbdjtv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggjsgzajk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gfoygqwpm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/grdwjboyj.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gysphlpvm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gwruracxq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtdgblglp.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gstvwjuoq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqjktiryy.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gabiudnlm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gbnpelzmw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gbgkipabd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gcpybhuwe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gqducolhj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvujrcjfy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gjccemoko.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbgllbdgq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/guvgctiqr.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gzkbnjquv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gazabhlpi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/geqrxyrvm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/glauwqlgt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gqbpsraoj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gtphotmtr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/glljypcfe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gyslbdwbm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gjqyozmca.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/glencajsp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gbvlzchej.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gkgokllyv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gawdzmhuf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gbwjtbkem.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/glgrzyova.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gvtfhdqqo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gicipcfma.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ghqwcmkvs.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/giakjztce.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gjxoijfga.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gfcklvlgt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glehrpeay.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gmszxdrun.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/goycuakxi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gfyhbdenr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gsugmywaz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gehmaztjk.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/glkslqhig.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gihdiicso.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfzhamyha.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvebfxzmd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpvptifpc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gijclbell.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/goygmnhbw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guzwenngg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glcuemuxf.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gjwqwupwc.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvzywsclr.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxniynuks.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/galtfnwif.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqmmbmfjt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gcrrbahkc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqfnrndhk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgyirkul.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gcjpgtpsd.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gcdfgwuhk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/ghsdenmkm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gulzmkhzj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/ggcfdmlks.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/guospjrmn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gclgveoih.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gzrhmcqla.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/goodgmiud.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gqdmdngdd.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/ghjwpvoty.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gktthgmxf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gqjkxepoi.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gofsxdbog.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkuhzvus.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gfkdiuudp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gnihscols.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/geojehzii.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/goithjpma.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gdfzskpfg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfnfulyhp.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gpqascucv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ghtpoqayu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gjgfmygju.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gwldgpdge.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gazlvutwr.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guxwdnfta.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gwlppfqbj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gylnlvabm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grrjtwdch.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpczekusf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ghaetbxlf.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqyubzfcu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gtakkkvtl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjjhaegdx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gatrdheaz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtcsrvcvy.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gvacjnuez.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gezwjiabb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxgsejwsq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfmngksvz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gppfkpmxk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/ggpgwozpa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gfcweqsub.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gbthlahlr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gogxqhezu.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gwispauvx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gmhvphtbh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gfsemahwk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/glkxzitgt.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gavhvjono.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gvprenyic.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gdvuiftio.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gljqlsnkg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gdsweqmxk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxofponeg.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gvizxucbb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqoaeglop.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gsikuafgu.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gmlzlnxxf.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gxpbhczqy.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdqsicrkv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gzifipayu.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gujuzellr.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gvsrixxix.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gyiiuonpw.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/grzvofkfu.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gjantfukz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/ggzcfuckp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gaewaetaa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gurypukeq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gylzzbngl.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gopreunje.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gzqiucpnn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gxqlelakp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gpakblahk.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gguixduwh.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gpnvwofvo.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gxexgfaiw.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gqafjqftw.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gzxnpibai.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gjdszhpaj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gmvnronfd.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/giodbxgzm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/guyyizjrt.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gihaihjid.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gheccytkb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gfrxbvujf.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/guilkrboo.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqnsayiar.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ghyydlcdc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gvwlmxqkd.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gkmkfppjn.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gqcrsftrk.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gwnhkxswm.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/grdhmmohz.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghysluwaz.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvxvohwdu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gttjrzsaa.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gihejakep.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gwvvcuirh.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/glmwqkifj.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/giwuclvyd.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gqqtitixa.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/ggouvvdhy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gimyuewod.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/glpyrhpkg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gjguaqlqt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gzzmqkbsj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gnuebotxf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gxctfzpcs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gacrjgzsj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/glwdjpife.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gnhshsble.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gjjjdrlos.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gifkggqqq.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gjjmtjwbv.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gaxgywrvs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gqnqtoaye.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gzvfgfzqd.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/ghcyukqrs.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gbnzcsurv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gjprcwmap.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gagouoedk.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gwjxniqqa.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gnycderjn.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gyngwvyka.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gjytjzugb.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gwmcystil.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gkxcbwnmz.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gblivifll.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gwuvdugjr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gyiepscia.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/ggyngwsne.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/guhkgoiet.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gijwpbwwj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gmtazyuxc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gizuwjyiy.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/goomwbzsn.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/ggjmpjack.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gvzhssrlm.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gbnamnhso.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gxobyhxpt.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gkavgbgow.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gbivhvtcn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gyearhkho.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gojpgbyxw.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gvufwkppa.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gulqttwcq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gfjenurcb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/grkralykq.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gicvpootm.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gmpzmgowp.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gubkdjjzw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gtorejlel.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/glvzbgikx.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gbkhoqeyg.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnavokdwb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gdpijvyrx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gvslqmurf.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gurzhtilr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gccrrfspd.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gjjiqzdub.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gcmdxdevu.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gtvckqfva.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/guqmjobyy.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gzxkgpdky.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gotbfvilw.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/guhlscvum.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ghtesodql.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gplrmmnfw.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gqzjlweyw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gyqqotapj.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gipqcchuo.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/goctomkco.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gjccovmeu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gztnkwszj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gizeduhow.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gelznxaeg.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gftxihece.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/ghgkprcad.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gghcdbkol.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/geesxcoab.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gkmptpakc.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gctfwdqge.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/grmifrfct.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gitdpqerq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gqurszzgx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gxomgzmuy.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gohfpmpgb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gtyjoqtsh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gaeyyilfc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gbvpxzdtf.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gzpaneqyr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gnjeaslyq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gjtqcqscg.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gyjczjduq.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gykrnffzm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gbrcyfbeo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gbtuakmuq.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gaagegocu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gvsbzkikh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsgrmytgo.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gjiziofzh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyuytxvab.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gdstrjwka.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gsdmxucml.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/grtwdqdys.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gdjflxskn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/ghzbvdqsj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gpztyonqz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/ghwaimzvk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/grbcmalij.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gikrugdep.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/giokhbnhb.sHtML


<!-- 参考信息 -->