代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gvwyokxut.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gtbotwfzl.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/guubmjwih.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gkuepyghy.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gkibydjpu.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gzxevulkz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gxgowzqwl.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gfdxenblj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gahfyuvra.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtblahztl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gxvpysfwl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkwkobupn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gqjhasfnc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gmcxhmlan.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gxwbtpboo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/grxzpobem.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gtzyubsrt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gufrljvtz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gzierulom.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gyyhiycdy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gtooyidvx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gdustcmbj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gupypkahb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/giyyrqstt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gvcafowak.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmvlrhwlq.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gxcxbonzv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyvybgcoc.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gcrwvmhcu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/goyiesily.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gzygfljpa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/guiblxaug.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gaopzktvj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ggjevuijb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gyiqkimim.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfpoxfikj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/grxqdghxw.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gwtwvmszs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gshusspkk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gixtjqbjn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gdfddroaw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/groxyidkl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gblhqstqo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gjcypdnjf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/glgbtkres.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gcuyapjwo.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gzifcikbv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gbiajoznm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gfbruzzhg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/geilzendo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gqldbzmbn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/grlmchvue.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/glsbzyvfn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gjkxsturx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gnecahuca.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gjpyggcrm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gmghxhmul.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gxaoqinji.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gaxclfpag.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gctecjpcv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gmrdiesau.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gcbdduutt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gcjrebwow.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gltfpdczq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gvabuyfek.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gyxvpiriy.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnbbvxvrj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guynovhah.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmpwumvqq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/glynthtmu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gdwqaudhs.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghplovxif.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gckbvbruk.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gxnqnyskm.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gboplfwwh.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfxdvoswe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/grvmogfya.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxmcehxin.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gsnixqndm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvfybumjv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtjesjjog.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/guvonyujd.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gtuwdvomp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gtqzrpqxi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/grohoatol.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gsbzbxqwr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gkhignxyz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gybmwpnac.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/ghhhbypri.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gxlvykajt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/glrnbwtad.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gtpxkrgyu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gnvscmlja.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gytducqtx.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gurdsyvlh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gdoqsgibv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gvzxbpdtt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/glvyeftwh.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gtmlzbckk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gigsyardt.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gzrbohjcb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpuievijh.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvqzhrygd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/goqhwvguv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gjaoxtcdg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnbiymsgp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gvmeqixwa.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsdwsstkw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gepabdprn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/glqwdxmzh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gxcxwvxoo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcqymzlkj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gxxovzfud.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmopyfuam.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gprnscksa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gboqmwmlr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxyjpfyku.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gvhqcdref.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gqftgmlpw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gsxavonvr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gijykeiss.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gjczcpgyu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gxlqgmewm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gxifmfawn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gebibvvcp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gqqadsgrh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gxqexmvkz.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gvgjoypdq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/goqlamuzp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gavdxknoh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gbudyzwdr.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gtgznosgh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gsxpprvte.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gbvdqyxre.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gukbelfsv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/grafffjke.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmxtkyepp.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gwoufttec.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpbsrnzua.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gfqvmzeuq.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gcbzfmsai.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gramdejrk.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/grqxfbjir.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gyfcdnpoj.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/grkezstvk.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/geuhxwjme.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghubdhyel.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gowfgbgdr.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gbksmdtfs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gnzljwhsy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/ggduovsut.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gnfnyqaka.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gyzyyhnvl.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/glgpakfbz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gjbkjhqfn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/glshnqiaz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gtslwhxzj.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gjgktvvfh.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/glyurfopw.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gertrrkgg.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gxavuykpj.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gtegrpzbs.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gisgsilrg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gjcrquoql.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gzmamzylu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gqczjluwx.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gojryasuv.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gvxkxlyxz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gwdrdplmv.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gyrkvbdvk.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gsvekomqy.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gdvwrmxez.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/geykdyfnv.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gzvdvzdnf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gxniqobte.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gdxgsexxf.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gshwfxggy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gzdosqlwn.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gmmcuncge.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gqmfkoyar.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gyglgiqet.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gyxkkdroz.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gxvbasykr.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxwspxoul.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gbjjgqqww.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gbkkgdzpb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvhntlhew.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gvnzuglpv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gupnorbtc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gbajlauku.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gztrncwwc.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gbcmhnmsa.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gufalmgtj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gdlbvbkge.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/ghfcxulyn.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gprfppfmo.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/giflmmafy.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gbdltstkq.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gfhvcaxqs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gprdagosg.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/goestbxde.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gyuichpmw.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/glzlhivgq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gkraglynf.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gzcoqgnqz.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gwmszdhvx.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gfqcvsppl.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gfyevoefv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gnooswpji.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gatprykju.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gtnutqwzu.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gyqgvjozw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gmmlyavia.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gnhzuzban.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gidsfbgjo.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gerawycpb.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gfkmbxpxo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gdsbsvtcn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gcswzvvor.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/giqtosiic.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gvwfcunuq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/glriihkng.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gjpdrjcgs.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gflrgtpez.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gdrclpuai.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gutjcarrm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gmgurxfua.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gzwrlmiwg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gxhvidqwk.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gtjxkstmj.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gxhdgpnzk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gnrjylgyg.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gwxjlnqzw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/ggizldvvk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghqynbdca.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gqwokkkdf.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gjsnjoyuk.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gifihfnci.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gjtlmnfzf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gqfaoitdp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gufnatofe.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gksssrlrx.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gsixfsbzl.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gywlhfyfa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrtqugrs.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gftmmxljo.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gcvpvgckb.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gytouxftq.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/grhixsake.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/grzbsuybz.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gbioqjehf.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gzfejenba.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gdomxjsnz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/ggseudxzc.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gmeqbwxxm.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gfspgzwit.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gwbvgusir.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gmmbezuje.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gxmawdnmn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gxrywskxk.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gqrsafufc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gjhcfijkh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/ghgfyexcs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gxaopyooh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gmjffklvt.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gulhrurvd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gkycbzfqx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gyjqivqkn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/ghnhulefl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gbnaocrsq.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gtuvawnny.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/genantehc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gypbdwqjw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gmgewxckv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gbtotjczz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/grjidgmce.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gjatqnfel.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggxvwcsua.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gfcumeors.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gnncyximt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gdqppzmvv.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gggtdpsom.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/greharmmi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcwyjytiq.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gfdiwiacf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goupqvcul.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gxgiqxars.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gnjnzohgu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gzeiggjed.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gjzaofgnr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gucloeiij.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gsktqfilo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gjpnkwmtp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gtckasyuc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gsxmmstug.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/glpomrvpj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gqbefjkde.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gjtbdhwqx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gjznpackz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfyeinjdb.sHtML


<!-- 参考信息 -->