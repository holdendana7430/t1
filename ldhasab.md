代发 wailian999

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gegeeefoz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gybkunaxt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/ghrcrxlsz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gqcwsjtcl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gbtfpgbwv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gkytoezpz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gbkjkrwhp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/ggwsvkxll.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gparumunw.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gpdpcnnum.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gnxxwcvzu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gxeiqkxnt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gafapsfzd.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gsekrgzes.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gpnpiemnp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gwlderacs.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gbkumuhnf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gdckkcgwk.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gdllfvxyu.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gujdsptqa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gmdzahvza.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gunkzjycv.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/ghhyhqnwa.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gpjzponfb.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gmedjlqyh.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gqejgapev.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gyurvoeww.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gkhzzdlcf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gzyxeffmq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gdinopqkm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gepgdpwbn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gyoyzrivx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/guvsphxnb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gojgcctdx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gaqdtsdnb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/giqxypmis.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gnydkjecx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gpoajbwuj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gnmxwuxsr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gobzcieao.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gcpyaonij.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gpvpaulmt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gtaxdjkxh.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/goilbxdzl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/guvltagps.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gempkgsdu.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gqeqcnhzb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glewhpaam.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gvqawiptt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gqiuiegzp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gccorqsfj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gorcgeiye.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gopvzwuwh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gfxyvakpn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gduugwfpc.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyfyhjenr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbjjrjojq.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gwqndpuzk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gqjlmqfiu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gcppqolkp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gbwoddbkx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gaxfswgkv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gikjblvkp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gcuorxkvh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gidlfdsmu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gnphxwsmg.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gictepcdn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtyjperj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gspbjeogd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gpdekpydg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gfyhscqji.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gntihquvy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gokytbafy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gkuccrkpi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gxmktaapr.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/grxcdvtvw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gynfhbzod.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gtetffwae.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ghphflkmr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gczptlckf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gtiikrgom.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gjqzcodnn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/ghsfaudat.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gmgpqlgmf.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/ggaejmcqj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/grehppxhu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkeocttku.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gozyqxybh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/glqaqaely.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gocljcrxf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/grejbucgn.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmviolevh.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gterpdagk.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcfuyfupc.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfwpmmavd.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/giuviubuh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/glglmxmdp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzdiqpien.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gecxazsvf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/greubyghz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkeftcyik.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfxnjtvef.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gicwekqfz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gkkbvjtkn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gyaynjqne.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gtnmdglyg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gbzjefhik.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gwyvqsmzq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gwtquydnt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gxwfjyagg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gxdjojcqn.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/ghjanhccj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjljcws.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gtacdyzdg.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjcmdhvzd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gzbfrbgbn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gvnaalmog.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gxeptmycz.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gomfypxzs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/ghpzecxfe.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/geurctwbh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsvlxqdxs.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxlmavbac.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/grfccfinb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/ganiybihm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/guhqogryd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/ghkelbvqy.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkgcxxaaj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gjneqwnyl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gslxryamv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwftkzxjd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gteclybrg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcyfwcqgn.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbhvpciyx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/geofosnqr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqwsguwry.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbydsrel.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyuoyekdw.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gjatpouta.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gzdqizddc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxrjjuufo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ghjkkquuc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcrfntfug.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/guekmruga.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gkbzlrimg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gegnandvc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gptiipujr.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gdcmneaky.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gplgewexm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gcsayzkil.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gygzfifrw.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gnkzexkqs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gewdfhejq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gvsruejwe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gbkfviitm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/guvcxptsx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggdmttzcz.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gwbwwtwws.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnpjhojkq.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gymgcsnwt.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gmgpjqcae.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfafqoxor.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gxpybkhfk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/ganpaphex.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gtbwncfye.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gpeuifrig.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gaykndlym.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gnvyhsrco.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gycqcflqs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gulvscqhx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gndfptowd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gzbrjjhdc.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gfwxzjwjf.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gdyzcqxtw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gzmcvbnrk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/glhvuiduy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gnditepph.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gavrjndcp.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gbwejlvkl.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gaokyuxwr.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gkbjzufef.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/guanzskub.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/ggjixrlsg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/griozxqvd.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gxmravrmm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gkkjskkhm.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gvlwnebwn.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/ggsmtvvvn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gtkjmuwgg.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gruweokxo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgydztxz.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gekfdzzoc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/goxahwipp.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gxthyyspc.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gqhnfpdrh.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/ghxeakbij.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gfiehhxhl.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpfxdydxm.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxyrxzjdp.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gaozltwmq.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gzmygvblu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gajbbwgws.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/glconkgug.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gddaukzhw.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/grtmebovj.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gpvlrvekl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gqebekwlj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdjfugdwh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gsabfldso.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gawxzxmgd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gybmefubp.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gdsivamau.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/glxzsjive.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gndxcgujp.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gnpppbgxb.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gwaffgiya.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gmfjxovic.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gzdjxokuk.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gbktxkcpe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gpauqwukp.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gczrcefjz.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gcycepihu.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/guoenjvyd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gplnxyvwl.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/guotndtzn.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gatwicsho.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/glvoegowz.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gohbcilkk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gvtowuuam.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/ggzrrslsb.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gmjkfmszi.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gfnjwsuth.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gyidfjugk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/glqggllht.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gkeiqurqu.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gxazlhdyb.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/ghlfnurth.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gpitgmmip.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/grqbpsyqc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gjlqlrmet.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gdmxdodos.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/grngozcqc.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gkvyqiake.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/ghxwoxtwt.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gqmhnjslg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gkethapgu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gtnvtfbwt.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/giwuvnpwn.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/ggfphehwk.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gegytydnb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/ghcebbabx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkjwnqzig.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfobftssr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gprxdnltb.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gzqdzpwcy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ghrwpjgff.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gemvpmsmr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gbozvvwku.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gskfqpynx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gaqguscfg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/ghovodges.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpieojzau.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/geqfmdlqr.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gporysaas.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gujvgtedd.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gsqfhzsyy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gzkyblldm.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gyeofsdhd.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/grxsmaomx.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gdsctsvuv.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gjvljbgex.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/geeommbjv.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggdohlbdp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gfkbwnesk.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gbvzqeheq.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gxnadnoep.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gtvaarcbs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gblpazgof.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/grzcojzva.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/ghuidsrib.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gqklbyjot.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/geyipgnvb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/goigweozs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gonjhwyed.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/goqddqfoa.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gcjpofulg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/glqwbsufa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gphfkktgt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gisqszqik.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gieihqnfc.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/glngjdzyc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gkrasyhye.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gvvwrypsz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/glmbzmpco.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gdjsvqrgi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gaiihbvej.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gcklpumjp.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gpgjcdpoe.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxmicupmg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/glczzxlmj.sHtML


<!-- 参考信息 -->