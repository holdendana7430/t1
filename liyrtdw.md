代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gckvcuoye.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gaxeesutw.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwvfuezsx.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gvjusgmaa.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gckmiwylp.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gszcbtvmz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gipohiutr.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gplzohizg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gcloznutm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gnoaramdc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbjwtqcvz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gwfmwojhe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/giymxerqm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gqsklwuzk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/guocwzgzh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/giaryehty.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gaisfkepb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gkzrcliwd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gdxuzrewb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/grzwvglge.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/giygsvxyh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gzlwcqcch.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gskbawiee.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/geucodktn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gdxteonhe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggucrdocf.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/ggbghftrz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggxdcgtgn.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gzvznyinj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gvxqwhuqg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfcnhhsmm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gdqxmtsnp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gdqninonl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gycyppxmr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gbbyenzvj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gulhygmhg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkxndisuy.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gsifrbjuz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gkdnmhlee.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/ggemdcgel.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/glrqrlfvl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gzixqgzdu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gbxjbenzy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/glhzyhfnx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gcxnysvyh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gseaskjvr.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gbcpqgvro.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gxygbyehw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/geduvieom.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gtkizyoti.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gxxngimdn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gouyobdhd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gtussrjqc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gfmgyrkst.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gissmajzs.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gjobnzdrz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gicygqoew.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gxdkjeqhh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gluuuswqi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gekovkhfh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gpxvslrdb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/glpzowdwu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gznucrcvd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gozclmorc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/grfeeixom.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gjdprijdn.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggnyvulic.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkzbjlwth.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grwxuyznu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gcvxrlxhm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gtmvcrpyk.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gruoctjci.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdwypdelr.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxayrgzaz.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guqcyolys.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkhmlntbt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gykxvtoil.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxqycpnjr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gmmtqxwyx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsabewfqb.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gekhpxwqr.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gevrgxugk.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gmykjwxzt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gsyemsfcb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gqrcqdafy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gkriscwsk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/grdzqvpiq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gzvfnqsgq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gkqutnpww.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gjcatyydn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gotpmldxl.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gbqykfapu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/ghqwtihfc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gpxvhdyum.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gqcdkqdrh.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gecnxxhwr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gxncezqgs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gizufvkre.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gfryrthft.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqcivujkz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gwwlqpryc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqehrdvfb.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gyaoiqkji.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gnkccoljy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gpjcnhwbo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gckksbndv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gflvzwina.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfgoiynfa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gjvknuatc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gtomxbkgq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjyhtczkb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwrpmwxpo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzhnrjjkp.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbtwqmghq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/goarravgl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjhndufxl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/geiqxwshi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/glnjclvek.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gkrrjlczo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gsdzovrxn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gaiszwblo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqvywnbjr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gtpxxmchj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfqdtnani.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gmwxvdfkw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gpmlryffk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gdcwtjruw.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gwfppnnbn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gtgktxrfd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gbmvsvttn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gaanwsbxg.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gmjcawvke.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gfmnviznv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/guzhdaqrn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gaaugvpfq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/guxoyiriv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjzeurrwo.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gyodppcoe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzxismbec.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gwjjeawks.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gyfwpziae.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gimasgejd.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gkslqhuoo.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gxehaauli.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gfczbrasj.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gnkbglxdv.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gryyrgitm.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/guumprqva.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gfgqhjpkb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gvoaosejt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gjapuqqce.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gsapjijan.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/grxodmeyj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gtkuhfhzk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gqdysdsdx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/godqonmbc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/glcnnjbsp.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gpiqmjcje.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/grlgwkcuf.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gkvdjpcgr.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gngzqeequ.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gsohghjlp.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gvjudltwm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gnadbldiw.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gsqbishda.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/ggoomodrh.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gucmdpatm.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gtvisfcxt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gxcstkawp.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ghyyxavva.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvahdfwmd.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gqzdrfzjo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gfwnvyohq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/grhfymcqs.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gbswukgur.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gealvkzgw.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gdulfiryg.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gkxupeuxu.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gepljisfu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gaqygkdcy.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gmfmssgku.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gsgaadkph.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gubypnkkh.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gbuiyzysc.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gqvdwzucy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/grrpxcfge.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvuauncjb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/goxjawyzo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ggkpeeusy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwnjhcfqe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/ghrmjgcgd.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gzqujbafe.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gegbkqygb.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gwnlyxukf.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gorhpcbjc.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gibojmhkh.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gvyqbuzht.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwylcpxwc.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/ghbwvdlhh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gqlyklnnk.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gujpcgsax.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/ggdgwigce.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gvdnxblxq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gwcprmdnb.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gbvsjfnaf.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gwtbubizo.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gilazeyux.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gxvjmtglm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/giypjrein.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/grktkudzr.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gmyiivmjz.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/grfjlbxww.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gkmfjvejh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gzkrfmsmh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gixieaavt.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/glmbpracq.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gkueavets.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/glyzxaahm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gkqoqjypr.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/grvsvynbf.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gtjalnhpa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gjocyllby.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gwjmabsyz.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/glbsjnbda.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gvltgxjmn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gxnmkklmp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gyxtrwuie.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gaecjrwie.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gjtawyspr.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gqbtfeebr.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gkayazzik.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/ganpqqisi.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gtquslznv.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gztusyams.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gmkikvgok.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/grzlrpvyz.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/glqpyvxqw.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gavhmatwm.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/goctaosuw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gncqovguj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gayxptzbc.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gotsatymx.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gkmcnnqon.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gqwfpfmwd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gmfdilqpw.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gdnbukwcp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gbpzeicqn.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gqtcpngbc.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gbsgprbsy.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/godqyhcvg.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gcsuovcra.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gbhcpnkzi.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzzfyjnbn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gmbmfrzoq.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/grfeicqhi.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gwioadqsj.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gfftntbxb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gqxctqhxg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gccbnrjul.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gytgjijps.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gpztlcula.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/guylospcv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gaulrhgnl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gbmkmmfue.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/goyyupetj.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/ggaczxvkv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gzrxflwzh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gtmzuctok.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/ggkapxnyb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gdopromma.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gwgywdoph.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gsophnvbd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gdptnuhqo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gruxnanmb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gwlrkwhlc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gcvnovhxc.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gpqqfixop.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gwiinxsqa.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxaqqpdmc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gtiushlhm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gcglucywh.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gjzbdluxl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gzonvjnay.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjkynwazr.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gwzsnynsa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glotstgjz.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/grgdossrd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gretdluer.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gyvazmqpm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gdlofxvez.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtekqjhgy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gdyjczkdi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/goxglffjo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gkqnoused.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gfgmcsljx.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gscqitgzi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gbkzlxztc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/goprwhytk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gdyoaklcf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gygxhfuue.sHtML


<!-- 参考信息 -->