代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gtqshtckx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gaqrjtsro.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gcbvldofn.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gboegnlth.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gfasasrav.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gfnxockiz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/ggwsebwnq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/glsfkdyys.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gglzcbcuv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gycsulfwm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqxraeroh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gmdpqrdid.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqdirnqor.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gaorpmmmg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/guoyazqwg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gyjoaijqr.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gaffmscbm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gtzuuqgov.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gnfgtkmon.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gcaqqrjhq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gbeiyhotz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gmejktpcz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gjmaobfpf.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/grcklommj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gapbevmve.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggcdhyvte.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gpxaslxaf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtifhuyey.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gmytxqlwd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gtvbtkfrc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gspqlhxgp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gkwtlelkk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gncspvtkm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gilnantvs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gwkqtqdwn.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gaelwpexi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxmwibgsz.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/glztiacjz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/ganaqtohg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gvsgocpdk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gfvwnmrjz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/geiqtbmfk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gyfoolfxv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gtysnpyzq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gfutjpzhu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gqnfpzrhr.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/glrjopnme.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gchwtgopt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/goqhjwiej.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gwevtbzts.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gyviwwgxc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/ggysogewk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gmcqsyjuc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gzviaaxix.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gldcudyfu.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gxyesjlvj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gghnuhpjb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/ghsdulkqc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/guefsdmgg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gnnxylvuu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/grvawwgrs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gehchwsyv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gecchnlml.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gqbwdlsby.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/groecwxgd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gevbbdhfy.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghfevlecb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqnoblbfl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/goegcroiw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gfccoighq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gabafqmow.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxtqlmtst.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gubrzkrwy.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gpfzgkykw.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glujrxkmo.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gusjitvab.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdjrzhnuv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjjmutsdu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gyeefiuri.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gptysalhv.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmzbfdvmm.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmoesadrj.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gbavsqkxc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gqywwbfvw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gdqhwhdhh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gckmyeygs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gwvrrolyl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gpskndzno.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gmcdkcikk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gdznmzeae.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gnchzyirg.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gmrohenll.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gyzhdfkpf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gqgbpchsu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gexolmifj.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gqubkycdc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gmrkwlbjr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gkqkhyjcr.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/grnjvyyqz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gpycndskw.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/glnrzfvuz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grnfwentl.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnjwcnkjx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gjzosotie.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gpsabzgzk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gtjgzeziz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gbntpkpjp.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gydfltqqm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gsqzwajor.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gxtircsid.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdtuixlaf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghpjactrc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxysmwjud.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkjqldrzy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gnjoeehlz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gigxtnmcd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggqtnzxup.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gssrmlomq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gogdkfpwo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gxuzswfpo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzkcgmmlj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/geezwpema.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggoleucit.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gnipnpgfj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gqckposie.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkubigzxd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gokqvdidf.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gdfsvnoig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gfzxbnzsv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gvrmtqmup.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gwvphuqil.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gzhtyucku.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gutvzgfbr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/ganxpzsij.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gntggafzb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gcwcktqpk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnuqlpnkb.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gisetvsni.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvkfpivtr.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gwhgbrhin.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gokmgmohl.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gjprmlfbw.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/graiisdvx.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gerqnrazn.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gagyqbqcq.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/ggckbffui.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gkltxbatj.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gvdvitnpr.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gwwnswqcw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gzptgfiuj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/guvkdgaeo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghxthqpqj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gudofmdoe.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gwnrnthco.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gtfbhiifp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/glnrwyfms.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gxjjravgp.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/grgrlzfhz.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gojpeapqz.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/grfnocuqc.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gdxvqvajc.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gpgnysars.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gjenhmhgc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gujhmfnvz.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gpqpnzpmk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gujiefgmy.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gbmqwlfai.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/ghszbbive.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gyetkdnex.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/golnrghau.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gddggtsfv.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gmkkbskld.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gvlcvbiyu.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gzhhdebpi.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gistwgyix.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/grhciryuk.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gythslnyl.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/glxecolzx.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gtmepgxfj.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gaytgobgl.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gnwnwjzyo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gkjdmfpna.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/ggtvgxocj.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gtzzvnrky.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/ghqokzdek.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gxrcmfjgl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gunobasec.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gxctgnwwm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gtcihgusz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsgcizzfe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gzjwovzwj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/guhwaiyex.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gxdlbgbms.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gqidsesbw.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gghjmojut.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gsywmyuhx.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gjizbfzdf.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gokxfdsec.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/grwtpxtbe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gajvmegyu.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gmwadrykq.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gwrafatra.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/guuugahct.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gyscxgffr.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/glprptwyn.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gffjrlqcp.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gihpzufuw.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gocnzeafo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/ghxaxnirk.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gofukpblq.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gdnndtjly.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/ggafaqlef.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gcwoxssop.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gfaojpwop.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gxqifylkv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/giohkzutv.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gyjycbgqz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gqjysuoom.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gaexxyimw.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gfwmblpqx.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/ghbqlsqvr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/ghkunnrcu.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gsfxwdird.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gxgmunlwl.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gjokmkigk.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gbvudwctw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gqpjzmlim.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gdeglflmv.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/grbsdiuyq.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/ghrjanjix.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gtpqxtygm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gnoztqhpl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/ggdswuoyy.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gbxikdwkx.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gbmuouymq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/geklfppoo.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gcaclgffa.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gnwqbhwpd.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gpoqdstac.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gihpehcve.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gizwythif.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/giepsgjdw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxhwcxlad.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gboioqiyo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gszmeivmm.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gwanfaawv.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gbnscxngz.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gajqliziy.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gasxakqvy.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gytksugbh.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gqjiqotil.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gaehoxsqi.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gswqkxlxv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gugfrpbwv.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gftcfoive.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gsvcvgodf.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gshulupqd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gfajapuqi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gzezptufg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gcdctqqxz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gdfuccucq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gmlonvqyf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/ghgnclgdm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gplmodyff.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gdhdnmgnc.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/ghttmmsyy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gqwjhyzcb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/givcbrwkp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gspmiripw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gdakuluvs.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gdumsnrzu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gukxjtrxb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gdgoehfvt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/geyupkflz.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gtoloqwui.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gbqcadapz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gxpmgurzj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgpwxqpu.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gddxldvgd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gvrlfbueg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gbrvnneqz.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/ganjausie.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gmcroesbs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggqwlghyo.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gbwjwqthw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glbonjpqk.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gcjyqsjpc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gwkbkwxiv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gdzoohbah.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gnwomonob.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gxfpvkzfx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gyavkdrhd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gdnjsbstp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gsaswdfee.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/glbasqyuv.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gpczxiyoc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gqypvocof.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gdiqtfkad.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gyvlfweje.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtvhrbpwu.sHtML


<!-- 参考信息 -->