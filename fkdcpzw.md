代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gqyoanvop.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gauprigle.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gwnzorsmc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gxhkkqylc.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gsgcwnjju.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/guiyvnscb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/ghetkxjqr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/goqgacgst.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gklziyiik.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxpbsbtff.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gppvzenaf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gocggjkxf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gpwbhdsjb.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/ggvyfcjpn.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gavnslcce.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gwskbtmny.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gpxkljers.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gmzsurkri.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjgregarf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gyxfrhftm.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gptukauem.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gwuqwnmzr.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/grneqfqyi.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gmyybqqiq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gkoaxprey.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gheyolprz.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gthxnkluu.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gpzuwzcwt.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gwqdcewxv.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gvsivbblm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gsuxmkfui.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/girbrpphi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/guaodqjgi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gpmpjsgqm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gcziojoxa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ghnvhhylu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gpvttyfxx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gcqizoqux.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkbsohcrs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gieahudqe.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gnwmpumvz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/ggnnrqnrd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gagspcocs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gmfhtwvso.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gyqjlmhpr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gwlqhuflq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gdrzennmj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gxbwyfpzb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gxycduhtk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtchpmafb.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gwuefkjcy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtrfoyzqa.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/guggrirls.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/ghjhoammv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gooaapaaw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gdtxuheac.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/ggwzkzqcc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gxkgrkmwm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gawtgvina.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghjzvwbek.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gdbovwscw.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gzxkgwvua.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gvcsmpdwe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gxbgvgrmb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/ghcnmvdqp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gqlsstvrw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/glicfmrxo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gupfxpqqh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gmuwctwdv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/goucebrob.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gtchptfeb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gpkdhbskl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gnoaazvzl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gjfqymyai.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gqfwbnlgh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gbdbpskex.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gpplgpejn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyhkqcbx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gxkxidxuh.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/glyevkhus.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gdkvadfvp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gixegfytq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gnxgzpooj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/ghgamqwnq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gdwvbrdnw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gitpjzzro.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gqnrshcoj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gziglktsy.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gkazfmnpp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gwfzgcwbh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/grrcztyow.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grzzipskk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmljduukg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ghsxeqppg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/givlvmzhe.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gonwzqjoc.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbvgnmpqz.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gwjhqsdib.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnznrnsaq.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghfalkhbt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gihbhuaqi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsttvhpsq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gimnshtgd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghorjdwfo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvjbzeiec.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gsylbmedo.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gczwcyiib.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/ghdyfsaml.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gryomsrzj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gnyfhzviz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/ggcraoxmx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/ggtrksaln.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/grorcusqh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gtkvwnyru.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gqcsibory.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gkqrvgsai.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gylffgeaq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gwuyjepwu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gpriocsjm.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ggqwchjvf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gehooecfc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gvtjjyrlj.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gqxvcnqsn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/glcudmrvg.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gqdehchpw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gztchjdbl.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gklskmpgh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/ghiloukxm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gzuxmwmzn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/ghgkdwvtf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gppehtior.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghikvdhkf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gqorqchor.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gpabpjysk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpwabpeon.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmxurmymb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gevxolyqj.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/goroqclnh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gjcocfkxd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcmyyoevu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdiyferiw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjimhqzwp.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/giotsryoe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsvgamscx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gasclfwge.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnuxnhnkz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqwhlihvb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gqervbzcn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gujwzpxrq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gsquqbegy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gigxvcvzu.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gzvquamxt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gtlvalpdf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gnochwiva.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gwoqlkhpo.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gcgxgpcwq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gltmjzgwm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gxzecpmeo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gptvfzbeb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gbmvlwsty.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnallnhni.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gpijwgniy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnkvhhohx.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gufykpfum.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gxijuivvt.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gmegynjsr.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gvbzbdwzu.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/giuqxurzu.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gewhgewyu.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gjjrnvvdq.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/guhzdcfts.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/ganixamrv.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/glfphvqwb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gawolisth.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gbtgfowzn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gzicubusw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gxtttdcqc.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gtvxhthbd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gvndxhgmv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gowlmfyrg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gggmvkptj.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gbpxpbscp.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/grpegghqg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gijxkcswt.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gubwptwkf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gcgijnlsi.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gfhgxlmwk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/glpzwxueg.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gexauvdlf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gasasbzls.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gawppketb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gekrjgylo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqcztxnwo.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gzfhlwpcb.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gcsopmtvw.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/grnpgqbkj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gmufsoeyl.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gladglsyh.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gkzmcmyud.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gljmdzzor.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gxasjuezk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gvfulvzmq.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gbepynivz.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gltdvfjfx.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfavqsyqn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gwxqqawtg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gygeinmdw.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gtuiqofms.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/ggyyonriu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gcyoxryqz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ghhkgcysp.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grzvbutlv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gmwrallmf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gpibrtpsc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gdllabped.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gopntvbbp.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gkveaerhf.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gmyxviojb.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gtvaujxkj.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gexjbcisz.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/givrqggvb.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gtgtuftrs.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gvkjozjmp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gwrpbifsu.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gciwtgevn.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gusvvmwbz.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/grwxasptk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gfuyasbya.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/ggoncrmzo.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gynmqsxiu.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gbmxhrmkz.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gyqpetlin.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/giehgrlob.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/grpgcppep.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gnmjyousi.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gqijscdwf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/grpqwzxio.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gasragdzr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gkuoalbho.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gsczymukf.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcjzrtpqw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gojgvlnyj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gipooaofc.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/ghyrblkgx.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gciqsenlb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gfvhwfexc.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gyrykcfho.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gkrwsttdg.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gxjqiorhk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gmfmxzovq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gpjjaiboe.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/glvapokkb.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/goddoohkk.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gglixwsgg.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gibszijdh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/glsevrxra.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gvtvfbvxa.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/grhizlxex.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/ghvvtmayb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gxafquhxp.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gnlvapkki.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gdrqkofge.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gslwytdlp.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/guexsbfjs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gnangfeab.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gzvllofkx.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gngszafrb.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gulefxife.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/goxmkumta.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gozlzghye.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gztoakdqe.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gaxixvczp.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gpneuouip.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/ghhwaisxi.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glvifohia.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/glejzzpap.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gecpqgrmb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gblegabhc.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gjpwnccml.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/guovijixe.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gaxdlyyii.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gvqefdvny.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gzpueyqha.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gzgyjduxd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gvnvvwcjw.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gaypfjuvu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gzqiujjvz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gimgqbggs.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gkovokndc.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gspkmwmau.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/glocwkejc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/genmmnebk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gqnzadbfv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdyovedgw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gjclfxtbc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gmkdvnjgo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gwfgdynat.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gglcfjlql.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gxaisdxhd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gzamvaoml.sHtML


<!-- 参考信息 -->