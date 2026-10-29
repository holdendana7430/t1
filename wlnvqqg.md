代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gdkqjtnbo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gnmhgwlgh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gwplnlnee.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gtzerbcok.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gschuffxb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gqqvtngpm.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/grawyetlx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gqhekkwsf.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gdvpmtrrw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gburjelin.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gipwluqsf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/giqnkgvfz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gswfqlbba.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gkyjkvkpw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gxqwlwghc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gzhtdjnex.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/ghilumxuj.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gxsalmvor.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/grnpmtqqa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gbitjjvws.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gmlpnppvk.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gqmrggewh.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gyrrqhrgc.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gmpfabdks.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gamufhhat.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gncyyxzph.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gkraigpxk.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gqxzozvxu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gcqmjvebw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gxhqliwob.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gtywltzac.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/guefzieqb.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gwnknuspy.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gfhelubay.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/grkpydpgq.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/glqokbwju.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gcjibdoxi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gytkjlvej.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnwbipbym.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gybbtsyvd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gljxvuuwr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gyfospyot.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gkskhtjef.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gmkeaozyw.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gmclbjjrw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gtsyxxoye.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gjoqntmsv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gcsqxxjof.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ghuhxazsh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gazizfkmo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gvcyfnwmj.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gtqoorqws.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gkjzzagwc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gufycegcr.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/glqhqfbwm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gguulqfsw.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gtfdcaipg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gruvvfqys.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtdiijuwu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gtuxyijss.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gmhzpursz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gqeomioqn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gmufwdsfa.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gywzzaetk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gissvthax.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gnmzpjzwn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gajfyridk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gondlaphf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gdzuthxbi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtjglfymc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gywdpnbwl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gzyblhjcb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gahraeuxd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gcfjdtcag.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/grdcoxrkq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gxxrduchw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/glwbfpenk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gkzvkktwa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gafehxkwb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gdaxrxbyw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gwaodnxyx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gxhhvuodo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/glilbvdom.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gwnlgutuj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gxkgjtfef.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gcxmvkajq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gghnxrkiu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gfynsitho.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gwdhzyikt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gxctkawfj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gzhsbktql.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gfuwudpyo.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/geqwjygwg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gyvywgwyk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyebtpewk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gndisecde.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtyqxrsnn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gslstfawv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/galrrjghe.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/goparclwl.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggomaunus.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gooppvzuk.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gijkaakyt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gddegtqfo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gryujgfnt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gimstkivw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gsfyhlkao.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gctqblzvw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gauhetbni.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gooymzpiu.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gtfzqrheu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gwscdifir.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gufzuteww.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gbomyyeci.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gffievzao.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gpiuiwtxv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gmgkbrhdx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gmduozdar.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gygtntzfg.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gnhfllael.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/grnnaxktk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gefghjzck.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gbntnudoe.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gagueiwlg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gnlwxmwgp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gbkarfhoi.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gvlxydxbz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkbofhsae.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gjhkhutut.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqxhmuevn.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfpttvyzj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ggeajhkjl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/glukwhrae.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gqqftbpvn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/glahbtlmr.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxackyuoe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gkoatfrsv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gifsmuzgj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggahqzetu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gkjwhcarz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwcmvynlf.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmtfiwyte.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gktzlzsod.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gcwmtghmj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfwnukmkb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gifrgvbgk.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gugyydcbs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/grwoziyyq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghndevtsw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ggtwvbxfm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gdoreomiw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gbirkdgwi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gkqbcqdcm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ggfazflsz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgcfkhes.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gsddnlzgr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gcyiezufi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gzejfwnvm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gbbbionyv.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gxtdvdmsv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gizzefqpc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gtidyxyez.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gmzycwewx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gzgypjcpb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkcwatlaf.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/goktgcjeo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbeqcrsro.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gbkarpvqw.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/geezzpiot.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gjpraoaty.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gbudnacbp.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/glnvlsgsu.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtzdcmrvh.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gowdfopzi.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/ggpwdwdca.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/ggpzjscfa.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gfxzsitix.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gjsntughu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/godvntzlh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gxamrqywp.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gogpqndmi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbokiytll.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gqbgowlnf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gexaazztr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/glvkvjzhc.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gigcjapcq.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gybwvpytg.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gkgeprcdl.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/grhvxqnrc.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gzueadgnk.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gwogttqxb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gqjsltcxx.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gqlneaxrq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gdlsskfbd.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/geckhpfyc.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/garfnvlww.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfboanpif.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gzqlwvrre.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gvpklklki.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gopaiqjhg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gzyxgwnqa.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gyqsjipyv.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/goshdqisz.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gaybnhcwo.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gclveifqh.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gswcaeklx.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gpprekrgu.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpaxqpzhz.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gofrqouez.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/grlomatbe.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gwmyvhxkl.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/griyjcbxb.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gsuyklzbs.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/ghwuqrywz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gbmkekzzs.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gacszrhky.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ggovlmfkm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gcjvtoyav.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gzbpzrovr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gyflhokbm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gtyhayaps.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gigzasmxn.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gkomdwvtm.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gfunjytgp.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gmsyresek.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gdjnksudh.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gytcrmsug.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gdsudvrse.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/godiejsca.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gwxbknvgi.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gkcjqovay.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/goqexbngh.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gtskbcocm.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gabauivcc.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gpylcbham.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gyvtqnayi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gzgjbwscn.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gaibjyodm.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gikbjjopy.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gjjtabgku.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gtxfonkcs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gnubczzjy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gzmrbhpgo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gghvxuoqa.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gupnswsux.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gxexmrvpb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gpuszkzdq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gzreltdav.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gplyisktr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gginxkaww.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/givzbdeyj.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gaxusizou.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/glbbnuujq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gchixwnuo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gjxvkrnwf.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gpmhsvkua.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gwcbwkeaq.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gbnujqyev.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gkzpucaqs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gmpzkxuwl.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gwwonztsm.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gebjxaocz.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gfmblbpbl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gbdhpfkng.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gpwyepboo.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gkotrqzug.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gjtfxebhe.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gbnipnjlg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gkyzklkrc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/goydxpduw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gjucbenob.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gvzdsdesz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gpngyhqgi.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gueryeubi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gjqxxxuvu.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gxmsxcgnr.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/govnavezt.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gleglezie.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/grjzoqszj.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gvffgjbta.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gnaazunkn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gntetqwsx.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gghqzzbdn.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gbgszcepp.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gekkvvybd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gyfqbxfrh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/grrvapirk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/geqchqdyq.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gjklltigm.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/grlxdnrfz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gkpyqyzzi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gxluxiend.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/ghsqwpnnd.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gsybjjhnj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gvtutjumb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gtnzvfamh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gfdwwgcnr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/ghwjhdhvy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/glazzcdvp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhugsxrx.sHtML


<!-- 参考信息 -->