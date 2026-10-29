代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gpmzuwedf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gjgmmfobw.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gjdnirzib.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/geihzliaf.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gcoimmrio.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/glviogyrm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gunukegye.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gcaydyyxq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/guwxoxvwu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/garminfdh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/giwqlznkn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gfpxalbfd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gsezjuitb.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/geeanlujx.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/ghfbposmh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/grqycsmic.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gecqvvmuf.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gxgxecrsk.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gmfrjpvxr.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gtoajcjtr.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gnhdvcylp.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gwzttasin.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gcsptfmby.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gymnweiwf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gcaeqhgle.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gdxobkmyo.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gvgnyuzco.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gcqbdcbaw.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbbmrhlwv.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/ghnlhvzxs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gwrhuawwq.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gwisfasvb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gwjwhslfs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gvohfeatf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gaxugfkmj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gcuruueoy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gtenauvom.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gqtwhcbhy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gfgpcxuuh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/govxcevks.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gakbqbwtn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gmtubkfup.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ghdtlwhrj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/ggwgddmrc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gjizosjbr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gaqezmlxv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gvtaauvja.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gtiniirto.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gizkvpsdv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbbqgpimy.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gkoevaugi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxufyefpp.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gqjmngrkf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gcqrrwuge.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwprzoxay.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gnuhjlrox.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gxxxvsynd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gowptjknc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gvsqdnriv.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtmtjyhqz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmotwxdgq.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gadnbzysj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/ggslogzvr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gmiwxdavz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghzgyadsp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gwnhfqpej.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gmkcpeugq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gszzwwerg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gavoxdwnu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gjjswejvp.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gnuimxoqp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gxqiunjyg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gucecsxkx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gwglawkcr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gjaolhkwj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gljxtyxqt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/ggbyjbxjn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gysicytdx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/guzkdummb.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gkkamfyke.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gdvjevzpx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gdhfxwnte.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gicothfav.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbyalkorx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/ggtlmmikt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/glsagbzgp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkporbhq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gwomdfhcj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gxlumkpll.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gtrxsxwbv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/grwkuoagu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glsvxmeez.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpikqjayj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gfcfqkkaw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/ghtrknqnq.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gffwsfket.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gekrioqoa.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gcfuymcpz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gauaclhkg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gnwyjdhyt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzyvoqgtf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzjiiomdh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gmxvtoyvk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfjucikag.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gputmksup.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkqwpopda.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gfyemiaoy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gawwcidro.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/grfrhhxct.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/ghlkemmbc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gsdhqekti.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gjiegnqlv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gdluorkii.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gdpuxglvf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/ghhwjrchl.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gmsgttqfo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gfrgxqcpc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gzfpngjjb.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gibvbrsua.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gslxjigcd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/ghhitapqt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtsmyrtzu.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gobrsamta.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gitduytqb.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gtstgcqsv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glhgomujc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcgkajmvx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/glrsayxsm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/ghbufyoaa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gfczdtnex.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gorinuyfa.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwtnkwndv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/ggeobysre.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gqyokniyr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjmvjrpeq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmxmonlup.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gkgwmmgxm.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfldbzzdw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gdahpzsfl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gyjwcjuue.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkywuswqw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gepybvfqp.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/grflllrej.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gucqfcifp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/grjxsbyvq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/giuakgeup.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ghyvdctjg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/glvhebhfl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gxrzdkcpd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjezuuldj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gluradbks.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gmcvjgonk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gvxrworbg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gekeqmcfh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gmkiigtem.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/ghrjgeyus.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/ggwmbuyjn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gpkppafps.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gtvxvkogx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gldakccwl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqdzpqiko.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gbmvierjq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyljocnje.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gxajgkhdo.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gjufbsynb.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/grpztbxsq.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gecrwadxr.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gnpzwqqjr.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/grafkmhoj.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gkxlzljjo.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/guzbwlsre.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxeciakly.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gsdaglhkv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/giqalnuic.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gluveigwo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gpogrtmjb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/ggpsfmsqe.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnxjpvmfd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gyvjgpscv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gofhqxeyc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/ggmdelgww.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gfaydyhtt.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gltcfasoc.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gjqittbuf.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gkeorozhx.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gyypkhpqp.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/geeoqhosz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gadjikjov.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gxrrnymhb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gidchihhi.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gogwmaslh.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/guqmsddgo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gqiiwitrh.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/grbusfdae.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gypsxgmvo.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gwxxcvvqw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjqwdevpt.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gypkeazvp.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gisbxukwm.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/ghodgkpar.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/ghugxfyew.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gocrofryj.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gavcwkmxu.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwxzruido.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gjldrbimi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gkcqobqsn.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/grrbclbbm.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdxjfdiol.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gcevqnide.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gryfksgju.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glzfhrtsa.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gpbdejomy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gwspcccsi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ggcdihocu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/ghsgowwxn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/grfxrxqpd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gqcaelnut.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gbrsilaft.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gvtdqeyxh.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gponptwol.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gzaaqpden.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gjsgstyzf.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gqugdtdqn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gyevtigng.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gnxutfmep.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/ggzxuaglb.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gxvwccruf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gtgryacnk.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gqaitvlyb.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gqmptxvkx.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gjxklbjya.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gumomqrzs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gdfwsylaw.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/ginjxdkdb.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gdjjxvzsp.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gniccbnox.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gwxbfxtid.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gcsixvngi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/grtnokpur.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gzraljgev.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gpbdciuho.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gdeqytncq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gknfyjblb.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gfjxxvcou.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gbguqfttw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gspplwslm.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gkhvalbpn.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gmhvzxdtq.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gbmhqcqme.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gzzdytlom.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gvymexntp.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gsxhkzvyt.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gstfegqmk.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gxggbwzsj.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gxtkujxvk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbhrvmnz.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gckhsnszs.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gdiufpvyj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gzsgzkyoz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gnwdvgpqx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/ggtlczskx.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gmelnmfpe.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gmfbjfjyw.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gzywybwzn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gkejbraqt.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gmibxpkxb.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gjcuzdyco.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/girtvonpj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/goghxgodj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/grkqskxbn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gfytzsnnx.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gijdvrxlv.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gjwzsxmey.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gjmzxkwnk.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gdvwqkrgo.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gujmuznmx.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gwjjpasjb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/giolqleuj.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gpvxstgnk.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/ghxqalypq.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gxmzckost.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gplwpujyq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gwbkeedee.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gomuupdhl.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gxqhkucfi.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gmryakogh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gndewtjxo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gnrxqffpt.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gkdcigiqd.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gpevsqeoj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gdgjpuywh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gkfuwoshi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gkelpvwrh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/ggekrwtkw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/ghmzferac.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gmuyrznte.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gdpzjwayw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gwzdysjdf.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/grjtjjnlb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gbhogsidy.sHtML


<!-- 参考信息 -->