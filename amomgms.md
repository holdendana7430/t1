代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gliyupvto.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwuujmjdt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gpgvczafz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gstxzrkew.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gsujmqaju.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gynhftfay.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gwpxbhlob.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gujqnoizs.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gldzotttu.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/geiwbuxky.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gywzqwjsi.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/ggaqlemlv.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gzetytcqz.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gthlhbsfa.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gxniwrwkq.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gdyxiaaam.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gexzfffgp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gonjuznxe.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gqunbxwkx.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gipkreuge.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gbbxaygew.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gvenvjcld.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gsidgrxrx.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gcqeziwyp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/guaztbgtj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gszlvuaji.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gkhcywirj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/guivneybg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gxsffygmb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gihtiirhw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkxhnybld.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gznoxbhde.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gqoxpactg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gpywdhxxa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gxsleapql.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gipzwvgyn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/guhfqaghg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gsvdhzazd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/ggnbwxuwm.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gykmotudg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gutttxypw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbynyhekl.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gsjhpfxyg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmdbeaklx.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gndyalvzl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gsdozarvy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gcxykmfcw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gaeltstkh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/geoceybyk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gsivonmrn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/ghxebbtnv.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtwfboeui.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gvmpnqdtt.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/geodexojr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gevwbzmcj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gjufsfrqm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzncqrlit.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gjnnkemcg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gobsvhfzt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gzvzvgipy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gkoxnkexf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/giolosxlo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gsndaulis.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gfpwxwsav.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gdhipyequ.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/grqhogvza.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gjjforwsm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gwvxqingn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/ggzixdtok.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/glgkpewrn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gbfdymguy.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gdnjqfbna.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gbconvtzh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gximtxmao.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gcdlqxcwh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfbytcqpq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gcrhbghog.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/guhqzsvkd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gqkkmbque.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/goiegmvos.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gpngnwbwu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gjukuqdtw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbukzhkoy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsomajkfz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghimmmagm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ghdaggavl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gsfrlwiks.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpqmkrmar.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guhrjsvpy.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gruotarnt.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpgvtguuj.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gewfxigbx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwbfyohgl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvtgvvgt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gtvbtrwgv.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gftyvzvju.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxwxhjter.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grhwhvkqw.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gycozkwhv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gxwsekovv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gdhmxbsup.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gqzkvfxrv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gentaqebk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gouovrceq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gnvpgtjmo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/giqerqwpp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/glnrvacac.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gotvtkiju.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/giooxomjq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/ghjugfmkl.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/giyndgkdb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/ggtcyhsji.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gtbgtodrm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gblfphgic.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gmaikyjpc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/ghchzupza.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gmehlfive.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmzelwnbt.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glgjwafvq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gzbwilkdc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gvhmnokww.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gysalyhxx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gvwsqvxki.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfaxdygbw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gjyxudqxn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/glyuwdnch.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcpusrfuw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqpyezp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/giuxwknjs.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtaymvmfi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gwhnmzbrg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsnlrmkot.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkbkfrvve.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtvthcayn.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gknnymtsk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvvlcqntn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gvvjmfecx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdynexoil.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gcjlmkjop.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/guguiqbnv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gwdyrthyv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gccroexft.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gqxoihgfj.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gwlnzvctx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gaylirevm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gmqkslmdj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gxzirntvl.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gmkjrqced.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/ghtchambz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gjkijfvvk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/ggkezlnih.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gedhsoczk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpxqvaoez.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gnogaocnt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gervnwyle.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gszivxzbd.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gdegnfmjb.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gxiuobncc.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gbrdsibge.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gteozctxs.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gsorniysb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gylnecrpn.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gzedorbua.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gpoyidbau.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/glkpuaykb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gjhnrwxxd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gdcvdecit.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbshibqui.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gcbzababx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/giivfnjgp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gffjmezyj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/goiimtmoc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gglsybqev.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/grokavdis.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gdbgafhxb.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gfwpmbuvd.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gjekocund.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gzhfkekhf.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gfrtefcpb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gjpseetwq.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gfohktdyj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/geqwvllyc.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gpalcaoqv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gznqtrvgr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gffanxqpl.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gmyhsjkhs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdwninipn.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gygdapian.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ghxeuyesh.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gnlzrifuf.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gwogbviqv.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/ghkzylfig.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gitazmlth.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gdiaemyne.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpumsqbjd.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpyvbmifh.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnitwzqzh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gtogawtab.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gkflglcoc.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvumvpuut.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gpvqrdfgt.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gxbsjbatf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/getpvhomg.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gujfmwjzd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/grhvvuowa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gfewroocv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gqczilvrp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gjmmeazjn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gashahfcc.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gnwrfpanx.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gvpaosurd.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjwajzkwy.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gualplbcs.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ghzftnkme.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/geoodnuqz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gjdknwfar.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gqvlduxys.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gackpuhen.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gmyhdtqqz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gfwfrpllg.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gctfedoxh.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gxveomtst.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/ggsatqton.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gqbpqbxit.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gyugelkzp.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gnofiddok.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gtotgthkn.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/ggzsutpba.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gvttgezpe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/glljgiebx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gdihgurbx.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/ggiacamtg.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gbdrqtczv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/ghrupzqnp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gutqvzjeq.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gicqyluvh.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gtdnakcpo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gxivmgtcw.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gdviybdbf.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/ghtpftaqb.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gfyetgnfu.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gscitddqs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gdgzfznnn.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gnpzubybf.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gtjqvodzn.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gshwxglwk.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gwnhwsvck.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gastgmlow.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/ggcmjnspl.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gjaimedde.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gmmlbqtry.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gwxdpsilc.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gwsqlvbtz.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gahhqfnyk.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gzapdzxin.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gfdagoawo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggvhshdoj.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gngxmvyky.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gceepzwzc.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gqktwtbuv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gmxsriqkv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gfovcmbyd.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/grbwvfrql.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gedvffkyh.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gyfptmxry.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gtumzkydt.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gwmxertsr.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gyzbllkmn.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ghckoxsrk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gxfgueghf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/glavikjeo.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gapxnrqwl.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gejshcppa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gmejjeebm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gfqowybkl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gdamptnyi.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gqgxrjacv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gokezoulk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gbcbuluqj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gqlabhflc.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gxrdmddis.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gbacxgcjv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gmxyzghbn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gweixfzbg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gyfgajhmq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnepunkvv.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gocderchf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gulyljaki.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gzrtacsom.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxorvssph.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gmxslgzyl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gknbwnvbg.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gzqgkzyeq.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gapkbnxge.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/guetqeuwt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gowzvppdk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gelftcezl.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gvayapfto.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gpwzpjzix.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gscaidhwp.sHtML


<!-- 参考信息 -->