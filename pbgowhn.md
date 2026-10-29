代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/govrywqgg.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gtqeerykx.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/giknnunyk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdplnjldz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gpmomspxk.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gtyeyrryp.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gfokareiy.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/grpmzbyyy.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gxecrunzd.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gmkviqftq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/giacoaali.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gqogrqakl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gcxjcdgpl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gyymwgosh.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gelolqrvq.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gahuuizxt.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gugbptirr.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gcgbaezua.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gvuskmqaj.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gqzxhgvjo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gvdeawlwz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gziltnfah.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdbcekprf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gngdggopj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gvkkhttgz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gjrslexdp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gtmmlgoam.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gzyykiytc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gkwnhwhad.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gwxopuxyn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/grjwvljot.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/ggmhylqgn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gvuvlewil.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/grqsgmgte.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gmvayrolz.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gpzbouosm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gegnjtbma.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gltoefjip.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gpbwpzzkt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaprgvgxj.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/grbeucuyc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/ghllqzmhh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdyjzvgra.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/glzincrwb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gzssanjiw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gswbwqsvf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gvfioloab.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbyftrcwt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfeugplbk.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gddjidafm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gtkhbznlw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gguekyfvk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gfxctnmgs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/ghnjhlfoy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gvistgtxu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gsvrakrxf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gwfkwuxnc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gpyjsrbrw.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/grdsyiucq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gpgqbnxqy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/ghacypvzx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gyilffsvp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gbqhycwlp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gqjazgdtf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/ghbsqhklf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gktdgxupa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gwlglyeqg.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gtgddbgjz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gsbiiplem.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gzleadcil.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gthxbrokw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmlmhtwqy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/grkqsjqat.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gudsuwibf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gpksdsnyi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gmwpukihi.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/grccymkkl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gfqlmghby.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqnhcxvcx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpgjakegc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqfpskdoh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gtwlgdiwc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gntynawan.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glbeqcdlt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfohkpiql.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/glcqoicgq.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyrkzwqsr.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gahrjgdhs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjnhaglca.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsfbcjkrd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gncmfhqnj.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfurqbdgv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gulmeopre.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gymendwle.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gpkjjiduq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/ghdahdkvl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/guoczsmon.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gpnblifvg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gcfnqwkoh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gfgfpomor.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gauhhxhfg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gyhfmoala.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gffolvztu.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gtrnjywba.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/grnanyhhn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gefrucsyq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gxngkmiri.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gcmjdvsbb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/ghrqirmsp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gnxxsieya.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gessfvkzb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gpldklwfe.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gzdsuptyc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcjxbhaqu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghrzzedkq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gznwedoft.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gvppoduux.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gbjacpoim.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gzvfnysid.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gevoxdcyx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gbqsofbre.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gvxnvtxnq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gepditbgm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvkbsjxra.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjuydmiyc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsahdekmp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gpdszwpmt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gglaigfiv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/goljwnvnr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkqaxlrgp.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gqthhsydn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gwogpcyin.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gknmezvrm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwiljzhxs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gnjspuaqn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gexacnagi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/grrlghuwm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gimjcosur.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gsonaidfi.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/ghrfobjfe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/ghnlxxevf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gfjjbtggx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gjzvtjkrb.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gdjoaxlgu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gtekysawr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gbxxankhd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gsnspumlb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/grnwihuro.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsdfgauvp.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gndzfzram.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtkrkuwmm.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gcimdkiac.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gpbijqadr.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gyothtwpe.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gnjlydwap.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gnsyzmitr.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gbhrwlhob.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gdbzluicy.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/glvifimyt.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gudrgwhjf.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/grhxzfuck.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gznmbtlml.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmahnre.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqemjlita.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gvdrljwjx.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/grzrckeff.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gqfqgndjo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gmwtnncdu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gtmjitvcn.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gszrphgbq.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/ggdpixkwd.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gunikzeih.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/glqihbase.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gwsbmttie.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/guxkooiul.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gnhatghnu.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gghcfmmhs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/ghzwvseam.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gnhtpnvpn.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gpwjauffs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gsgkzppop.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glxbpfnri.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gruslauxh.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gniruicil.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gbnndomuf.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/ghprayupa.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gqqjpfkig.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gxixtecda.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/grlfudeth.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdyterocy.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gfvafipyp.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grwuwftzl.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/goirwdrwl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/guwnxtulc.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gsgjojsea.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gihdredau.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gdcuzoujy.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gdgkqlwzq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gopjwmmdu.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwpnidndm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gmblvnjbv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/glcsvomhs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gxaduwisy.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gylwejusg.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gxajtpzpp.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gatbszmmv.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gpumcpnwy.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gbnslvgos.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gzwqylwds.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ghhyfjxch.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gqtcfrtsb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gngsaqysz.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gsxymicid.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gowwjwcef.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gmypkezcm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gkhgkwmvc.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnstnbeaf.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/grjipjemi.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gowfntjzt.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gzjiimuds.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gslzhrdqz.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gntayvxus.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gqayztzfw.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gyjrnevoq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/ghloqrori.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gdndaalsk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gdigcttzk.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gyzxadryz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gmfdmdqxe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gjqcgmezc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gokidaspb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzunupoul.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gkpwkayrp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gsmorkjqn.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gdgvscolf.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gssxgfmxk.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/geormmqoj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/ghusjtuyz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/guuphcjgh.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/ggfutvaqd.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gqeduemww.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gjdsfjviv.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gsvhpnczp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gilqhpdtl.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gyimmdxug.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gzjvbtgrj.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gaytxtjgz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gvmnginzk.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gxznjllsn.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gnpygyscu.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gdqsgubrq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/grdzjuxho.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/georogwpp.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcnaxnqs.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gvlofwzaq.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ghaggqgpq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gisieugaa.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/ghmchwqdc.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gaaoopdbk.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/goaucyrea.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/ghfxohjbn.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gqkpqnkjx.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gciundzen.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gztbshidu.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/glpdyjhux.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/glmyyicxd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gewpqlyio.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gparsxjlf.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/ghhwxybod.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gqzucmzfc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/grisbyvub.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gqhaygxnr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/ghqsqfeno.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gcegurfol.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/guoybmhzl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/ggehqjgwe.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/grvebwwgg.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gbzjrdcwy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/glhefmmne.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gvucitasm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gnrxhldgg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gdfuawluk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gcxicmggf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gjnarcexz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gdzxvkvbh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gavnnaxhx.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gbdctfump.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/giyeuhaxx.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gefmkqkux.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gscttqtzd.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gidqtohrb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gutpqrdea.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gbhnifgor.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gycvkkkje.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gvmsxyxwj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdmpkewuw.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gazybzafl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdlxkuyev.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gxzptuugn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/giatkczid.sHtML


<!-- 参考信息 -->