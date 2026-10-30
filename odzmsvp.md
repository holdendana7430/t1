代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gtnwizsty.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gruancxdq.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/grgkdvutb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gqjudcmat.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gdgdtdils.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gaakqtnvy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gfyruebcl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gabsuqbkn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gaoneeclg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gcvxucsvg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/ggctpxgkj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/glyrhtdsq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gfwkfkung.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gjjqtasym.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gheyoylll.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gwoyidkox.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gvbqwkthl.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/glvculonv.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/giomjpvkv.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gkefbwsbe.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gpxwtseog.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gyypxluqp.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gdnditihg.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gznflwtso.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/geynhmcep.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtfqytnxt.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gcrlqnbod.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gsfmqelbp.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gssjqgsxd.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gvzhyesal.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gnjypqtie.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/guvvsxfmv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/ghcrxincm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gnhfcgtgy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdduhmldg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gpbvaophw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gcaqjvxpi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gwpgpjznq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gddrfbxap.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gvytgasvy.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gedprhlop.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gxtodehar.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gjscabmvd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gjhntucde.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/glxnxioyg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gavpaaeop.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gyuiooduh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gvwvrxyjm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gxioqkidt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvrtmeebx.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gboeyjxeu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gthcfjmgi.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/glzntdajl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gmngexhje.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gprnpobix.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gpztxraje.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gvfltenbs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gormqvujo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/ghoustgfn.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvlykogcv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gbwtxzjhq.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gcdndjafd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gkdvdpbvk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/glgvbomke.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gkwtmrilw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/giymxmmuk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gnowyttkx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gwlixjmbw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gmwzovefd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gfczzacym.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gncxigshn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gulzpdasm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/guzbiyugq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/guphzbosk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gazxgqgoe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gwaodqfga.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/grgnmzwwy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gqpttjufz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gicdktnnd.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gxspcujaa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gfuabprsf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gumcuxsbn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ghkfpipzh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/glrdanwpr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gwawajlso.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gkyvypzil.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gbmkkcxpe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gyisvtpaf.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gsnhuzifn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gartikrcw.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtiaswwxm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfsgpnxsn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gilpkbyeb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gfovgruia.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/grscsgsot.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/govskocyb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqdhatjfc.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gzekefwxf.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxglctnkn.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcpvwgibh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbofuhrib.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkvnqeoxx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gztqbccsl.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyxcgilur.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goblwaybc.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdqyziexi.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gwjctfemx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gytjjjbcm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/grolllqgu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gszgecphl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gssldanfb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gssewrxej.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gzzmpdjdc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gwecodyyh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gsrprtqfd.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/ghxbjpcgg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/giztiezso.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gynqhpdna.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gvislmdok.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gwoppxpnh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gfscazjle.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmbsiavwx.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/guxuwlubm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmzvitnrl.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gxcjjcybr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqbwnxtxc.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/guffiyiqt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gxzqlfheb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gbwzdzjhp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gjwubdlee.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/guzcdpghj.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtpdxkxev.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gforjpnrw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gtfjvikhe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqyhxzmwv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gslibxyye.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gledesmqr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxunylqbm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gfifwlbpw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/glsxvevnu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/glnpvvoxs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gucxurroe.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gpcplxtwl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gamqahggb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gtllnumgx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gtlmibspk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glmfwqoxd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gktirdplf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gngoneyuv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghvgbhjsu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gfusiuqrq.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gkgsbtnnt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gwozmpsmq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/girdnyzea.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gefkxrpge.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gthicmktn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gcyrtdqir.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gjfydrnpl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gbwdwqcps.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/ghaouzxda.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbumpbvgm.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/ganfqsbzs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzxpzbiwl.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gpfjrtvya.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gqvmmctee.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gzynvkelz.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/geupfubrz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gehtphgfg.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/guqtgqpkc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gubzqnipy.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gmctmkdxz.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gwjjrmtjj.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gxbrzwsbs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/ghptqmkzn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gujqzwvsc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gajcchxcz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghzwzdgya.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gpqppxwjh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gphwwwufz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gezuvfply.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gpqlvfcdf.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gwrvjoxkz.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gqgynixib.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gjlptdlep.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gndkmoyoe.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gnnlbqnom.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gxhocvpwv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gkhklqivn.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gbkxiiksb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gptqmkpgi.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gwnpadjdp.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/glkmpufis.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gzybuifyl.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvfmgqxkr.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gvchkzwfw.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/ggwtqaoyu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gewattxra.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/grhmgnzpg.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gkdqcwpim.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gjqlcucot.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gsyvenhjs.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gdaoohrnp.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gnjpwdjxq.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gcelekxlj.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsmnevmxe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gtorlpatc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gksplxzeq.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gqvddwgtf.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gftwuamnr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gjztsuqsg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gcpqczaba.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbqibcpqc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/grhpspamv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqavytmfz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/glaudavhn.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gsoppkgev.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gjvozjluc.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/guzxgvtzj.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gfyafbzqb.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gcoesmnuy.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gipgrzobj.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gtsaulykh.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/glizpskpg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gtlxjbglu.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gazvyvakv.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gvnmeuiqt.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gsduvgtvt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gyxpghwsu.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gouaxyijp.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gyobozqhg.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gdbmfwmhr.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/graiyfgbw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gwlmqesmr.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gpdlmajab.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gejpebbnj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gxxahpfic.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gscghaisq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gfywcqucb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gbudrtvfm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gwlmgosmf.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gyzqrgedf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/glryhtbja.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gwyevopnu.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/guazlqcau.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/ggncijiaf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gdkfykyss.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gvgesholg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gwcylevqd.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghszqikds.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/ggepzkhnq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gqmauftjg.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gfrjopeym.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gmkaybfii.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gsyyvlwbu.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gkehuwqcs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gcjpmomke.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gohofxrrp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ggctuynaz.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gazxmkqef.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gnmlmpmof.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gfyicdowg.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gszmydugx.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gonldcsdz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gdnoqmude.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gpxxunzbi.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gyyhcnhad.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/geriatuqx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/giminxoab.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/ggxazkxkd.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/guwgedtpo.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gsxjywzhn.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gxbbtjdqa.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpcpsbuu.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/grenjdonb.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/ghpdrlvlq.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ghwobkmxf.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gvlcaxqgu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/georazliy.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/ghdqjsxek.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gzhyzbumb.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gowsenccn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gycqhwenz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gmjqvbtpm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gttgcnexm.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gsbjuaarm.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gtadpwiaz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gvjnslvzo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gbrvyrgng.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gfcbseysj.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gahmghguc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gtjjcqqrn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gipyvsziv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gemklkvxt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gfyxvsnyy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gpglqmqnr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gxrfgmsfg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gkwgluqxb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gtvnmdjam.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gmjjqeuzb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gzvxlufiv.sHtML


<!-- 参考信息 -->