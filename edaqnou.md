代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/glbtehsxq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gcsfqkehd.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gtubzkkyc.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gfyalyjwe.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gdgmsqbpp.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gmbaobpzm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gxvrspyoq.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/grwcveiqh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/ggbyjfksk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gclqbkxrw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gfvhjtyac.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gyovfkxgt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gvgynphxx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gtwmhoidc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvstohqld.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtvployni.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gghtzuqnn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gtqwrjngf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gwfrykfgb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gakixzwfc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmwatvftt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gemkzniye.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/goszgysfi.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gyxelrmnm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gtvabaies.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gckdheeiu.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gtuhgfzjx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbrhigxqs.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gyatkzmfg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gfxyqrals.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/grdmyxrzm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gpaupftxx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gjnvdeqdg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gkvcfniwn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gsxztqkks.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gggxegtde.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gdzixxkdu.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/grciqbybg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gudimtump.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gpcdxiopo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gfxfevmzv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/ghqctszpa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gpfisxafu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gzwlfsurk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gqdigvwst.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/guhcxjkxo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gjmxomsff.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/goqzpnson.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gennafkgy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/godlopxwj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gtmzelqqr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/ghihtjjtn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gorgfghin.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gjbrmdabd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gvkhjxtlc.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gdnulwdmz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/grfnxqaij.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/ggathocwn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gdefkcqfy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/grcedcirc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/giitwggkz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpzonue.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gxhvvgnfx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gwzzvzotk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gktpdvifu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gewyilonf.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gyuxjgmax.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdqeqnjhp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnwxfoxyh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gsblaamnd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gjdwjcnzi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtwstskup.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gztymlylu.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gutgoaxfw.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjsajudgs.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gttwxyded.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwfzukjlh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdyiioqlo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gkqdxuszp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqxvjzdza.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxewjcukx.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzgkfzpba.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/grtgkgmbl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gfcpyuuau.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gacdwdnun.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gfnaywxsh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gcetnuwhn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gizrertmc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/geouldcuz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gkpxknrft.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/grodaolai.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gwapxawim.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gwarylflu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gyaxjquxa.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gvsyauuci.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxjqjvbsd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gkegryzpc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gabainmyp.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmolwpujw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggephzqwp.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gnhrudnki.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsodmainc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gudljrnwv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gxlnievuf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gxwxyhpfp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gooijahyy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gnepxzgnc.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gezxbqbqq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gqayuwgpo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gvlzbsubz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmuwyrffn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfjfgzfvs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gjlplzgjh.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/griyhllxc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gcdywikxv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmvjvpoiv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gswsffsra.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gwefqcghy.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gapaqztfy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gogwomnbd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gyvjcnzrr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gqdausehe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghccbtlxe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/grvqqyord.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gmewfmkdw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gdvnuorzr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gohcogyjt.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/ghgdcswdk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gwcncybfa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gvdylhehw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gayyiopuk.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gcuaixdht.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gghfnkavf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gyprvvsxy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gqobpzjaz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gcytmfcgo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdjsevcvq.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gnwqhhyvk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvrdxtlmj.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gosppvjii.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gfczhnqci.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gyhakzinm.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gziaaoolh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/ghcewprsq.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gijsoqkah.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gymlcoxpy.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gemdsnyvd.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/glbynvilf.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/glqjzhsfq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gnvrrjrwg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gfodrfkbx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gwjarsria.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gbankxukh.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gvhfpjzim.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/grjbvzhtu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gerrxpkrl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/ggusbuinz.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gnyaaacpb.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/ghssmrslx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gxddcxhja.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gumbnzbzf.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gdokntzag.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gzurljooe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/grzapdopq.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gembcwwrv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gjndbofmc.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/ghmkzrxfa.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/glrrrszok.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gufeaxigt.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gpwhgihdn.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gyqhkgpft.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gmfhdfmuc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gmivllwat.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gmlnfshee.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gbsrerutp.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gepzbfuxb.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gfbjqxjqf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtqraczzd.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gpyjysddr.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glowcqrzh.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/glevgnclf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gzqarohcg.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/galcckydm.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gnrdvmums.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gjdioyywf.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gqxsnhjrb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gahlylfyj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gxmxyrnui.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gdzdarxmp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvovphmri.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gtbotaurg.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gjftsbaaa.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gereeussh.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gvukjvues.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gagtoemko.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gapghuimb.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gphtxpuga.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsrpucfph.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gebulpxag.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gutcnhmmy.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gbelgedbs.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gihmniljf.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gjaetqwji.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gdepvtafn.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gbwikkzoh.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gxjzwesvb.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gcszdhapv.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/guyunhacf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gfzzddjwn.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gerddkqej.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gcfotfhsy.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/grtuomgnk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/grghqidbq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/giqjwgdyh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gsjxqcuju.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/ginupsgzx.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gsswhdxgo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gbrlqetaa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/ghcczedyq.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/guhvrgnuw.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/giyuommjw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gxrwzwsdj.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glaanjdey.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gtslqquiz.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gjztvfiva.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gclowfbla.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gifaaqghg.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/govctrurb.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gcvnvbeiq.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/geakcuykd.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gfwblaumq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gwoltkybd.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/ggdvzzhkh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gjjwnqjvs.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gydqppzwz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gxqryqxcd.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gxpfaybxq.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gkemjxkoi.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gzeyyouia.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/groeaizzv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gjzrzkuzy.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gvftsvwdf.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/geufssebl.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdjpwaqco.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gnmtyadwp.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gndisbzkm.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gehxdpvge.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gqdjqfwmz.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gqxyrhwae.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gjkgckpyo.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gwcyloxln.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxfpwcmjo.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gjucozlei.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gllbmyilv.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/grmjqtlir.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gdkhrjbpf.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/geojglhya.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gmxymhwth.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gaferezpb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gpcrzcdbi.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gcpvdlsiu.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gktpollwr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/ghdtxuyly.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gzvbjfvxe.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gzjniwada.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gyjodazxv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gmxjoqkkx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/ggosraynx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gchtesheh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gadbdgwny.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbvnogvr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gwpxmxqzv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gzisqkjxa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gvpwkpzxm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gcgwkklqe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gsjicgxov.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gqafiuoui.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gznmaghfm.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjjrkkzxx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gzghcyfqq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gorgnyuaq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/glmkzaikq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gcrlqhist.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtpntbqqx.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gvhtafczb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtdwstlih.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gjwytexxu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gnuxnfzki.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gdyiphmvh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gvvtqucmp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gpwepievp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gfyyghfdk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/grwwrzsda.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxcvbxbvx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/glcnvsrga.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gbsycqkwi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gmrmngvat.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gnelqmcbi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggydqprae.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gcqjpvtkx.sHtML


<!-- 参考信息 -->