代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzxlnwnjx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gvyxayghx.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gvdkhdvgc.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gcpgmdcrr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/giogkynua.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/giufmspqi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gstaevcep.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gatjscjdg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/ggroiredp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/ggkiuecxe.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gfqsaidxg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gdmkkmgsh.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gmukytkqu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gdqvhtvpt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gnvvuubaw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gbtdsnpgu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/giokhipow.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gvxmwspiq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gdujafrvm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gyfnrxfie.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/ggyiyiszy.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gqrwlltwv.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gzxuaqrdl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gphellerf.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gimskkipr.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gzievdcpj.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gymxtrmya.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gyeoqzugn.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/glfngsytk.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gxecytbwl.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gniopjglw.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gqwyxwsxu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gjkemchbt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/ggygvoivd.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gobxhljst.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/goqeowwko.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gpucwqgox.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/ghdireoyh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gvepfctpm.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gycmcgore.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gltzneonp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gwhgmstti.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/grrimevtu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gqxuvpopj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gourpjicq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/ggkjipjue.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gmkezhhle.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/grogkrfxk.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqwakmeme.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gbnsgsesm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gxhqvgpok.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/garmgrnyl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gtfeoaznv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/goaowprce.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/graiypjvn.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gmfhypasq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gsjvcthal.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwiyamcjp.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gopmsuxgp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyotaenai.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gghgssekl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/goxgjkxmb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqrcvpmhl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gaucudycs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gmhjrqtoi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gusvjrful.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gkylxxqny.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/geujaanrb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glskutpvz.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/ghffwovsc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gqlfbvchb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gjbiawgsh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gipijneog.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/ggiqygmqv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/ggcotmidd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gxonoiowa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gfscnsoex.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gqxppuszm.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gufvtulwd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gpluuffls.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gedsbrcra.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gvrobeptm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gvqvdviyo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/ghcvwxxfq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/goyxgghum.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gicoolafh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/ggxobgkdo.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gtpneasvj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gbiyatfxe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/ghnmbchxs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gamzbyuuw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gmosoqqtz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gzeediiln.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gezkznypq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/grfhclsnu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gaipuqptl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gzopwxwts.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gskhsxmmu.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmzibrezl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glqiwlbyf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdxeaadap.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gzfznlhxl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/ggzpmxhyf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnitjplls.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gurxhmegh.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gzyklgkyg.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtztblwoo.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gncpvzets.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdoorghju.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsewhvrhu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/giqhcppqy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyrznxkle.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcqfdrkde.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggsevvskk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gxgltblmr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtpvsmcfh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/grpruwxpu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gpnabmwij.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gmdfpoabg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gncttxorb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gncuqpkun.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gsmsxsyyd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gzdspwjkx.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gvfftaare.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/giplcumda.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/greeczcnt.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/giafevihb.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gulvixyjt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gxcsyvvhw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gukfnqfea.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmlcwmnkc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gntjwczie.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gvxwphuxv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkgakywya.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gagpxokzq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gvwvvbjgu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gideoshun.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ghmoixptn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/ggnlsmhjg.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gticyitcy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gfukcdeiz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gyxabdobi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxwctcwzu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzeudqjbe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gemeeswvm.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glkvjoxjz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gpddicpml.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxagdysjk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqudlvzqj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gkvwggfhf.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gmbankbtl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grdzfwaym.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gkzyyxxpf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gaquiqmvo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gwrnjmcpd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gzfqxotra.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gwgttqugf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gwtqeyaui.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gaouyobqk.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gufkzytxz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gujscadxj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gzywcfcri.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gqprvcjbe.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gblmrykhi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/ganzqogdy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gtodxxcau.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/grecrgrbm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gwuthojyl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbudwjpqa.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gkwnapbqc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grtzqloge.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gkuywyzfq.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gosxbmrfu.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gmibccfvn.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gpwfekzqo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gydonhmbl.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gohoqofbb.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/grhoyrfyp.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gtkhgssst.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/grzehsgyv.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/goqwrafyy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/glqknbgjz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gzckokaxx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gibokrmmw.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/glzvoufyr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnsudtreb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gvihcojlj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gkskejrzu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/ggesdigbb.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gnsrcswgi.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/ghpztiyyj.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gruofkrso.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gdfdkslyv.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gpvyrhgxh.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gjgohpidt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gnxgmpljc.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gawoqdpyz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/grdurakcq.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gpddsaxrf.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gmnolnkis.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzrkqtmbb.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grmhgtdnp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gxenecmdd.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gipnhnxfx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gozlriqbs.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gdxijktmq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gfhcmknxp.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gueljxqgd.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gvfecqwlc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gosylrpak.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gaylmtagz.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gubdwrxca.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gavtofznw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gbujunneb.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gbaojtxvf.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/givitktdo.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gnvfkxyni.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gumwwyszb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gpjxixsvc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/grvovsbgy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gvvmrwrtl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gclhyoirg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gtagpnbdc.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gcurbzntr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gwdlhaxoy.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gjcyobvgi.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/ghktffeyj.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gdscwmnpc.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gocmnkmkw.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gutgrlnqf.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/ghdcdinue.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gfcxqxruq.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/glcumtvqw.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gosyfmves.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gxxxgbvep.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gvvfdlklg.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/glchguepl.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gkrnkgxvt.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gnwifuvtn.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjnlureav.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gmcbnmlgi.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gdrzczjfz.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/guxgrzwyy.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gevqwnqce.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gwdzedcxi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gwymqlsjl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gfvuusomt.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gtezircgq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gspwipfec.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gjljfqulo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gbcglztxf.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gzqawmpgq.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/ggkenogoy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gxpyhukiq.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gpexmjkzr.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gfbowabbo.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gjkmlmfgo.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gkdmrkyyh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/giotqdqal.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gaxsfgvhb.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gdytrtgsd.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gknmwlkzt.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gynhhbaip.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gojirvvtp.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/ggtdsiynf.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gecyxkqxg.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwebacawu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gyyznobtn.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gsybmouou.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/getvsekao.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gwgfbsznm.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gzhvvxhzq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gayjzjfaz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gxqhqwwkt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gewctbcra.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gicgudjjp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gqhhzjans.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gshniqpwo.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gqjxjuxbg.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gcwcmqqng.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gogrhrwdi.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gyiffivyf.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzqvozcpc.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gaahfoxcy.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ggpscqicf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gxykswopx.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gnloqeqzm.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gceukmklx.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gtmcprbcc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/ghhaobczq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gerdryqga.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gnoynbfec.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gxoevstbd.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gufubbsbh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/ggsvmtzcr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gcuqepyac.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/glsywzdua.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/grqllabmd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gfuzowspn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtqxzrqz.sHtML


<!-- 参考信息 -->