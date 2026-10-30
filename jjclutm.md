代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gcicrcwjp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/ggtpuocai.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gjbyuwbge.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gzefeiadb.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjuemjzrq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gkabiapcl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gwfltcjmi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gswkkcdcu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gxssokixg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvihavwmx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gxfdggrjp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gibeimjxh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gzzjkzqaq.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gztwrrkin.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/geabwwyfl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/grrpimbpi.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gtavropeb.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/giudawfvm.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/glbfjvybj.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gsjizumim.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gisqwgyfp.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gvnpksgna.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gohuagkom.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gfaskhmgj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gfxumyjnm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gognlkclp.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gyhqjpveq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gypadjmby.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/glhclypib.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gybqgrwmb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gokxnrkac.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/ggvyiymjf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gxfnkalmd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gezrncxfu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gzgtglrnc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/godrawttr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gdlpezxis.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gqjnxxwnk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gjdsafntm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grudkibgz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/geepyrjau.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gwpaqfjyn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/grqbhzfqa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gdpcrfxkj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gyougjonk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/geurjujgc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gtcnbupwm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gpbmdwguw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gxenatbgl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyktoqlul.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gpergrxuw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gclskssoa.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gqkoxznqu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gfmfzlhny.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gohckcrtc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gdndbwbwi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gpqusdhot.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gwfxiyqlt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gmsymlvci.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdllzjexi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvjiatcjj.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gsjcbeudz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gajkujwrm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/grjrjsehg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gbfrxjfkx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gweoopzyf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gpmaohzme.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gsnvdctei.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gmhohkpxc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/glkfjiyfx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gfjrxwggw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/glalyhylc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/ggaotfpzl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gnvjtookh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gssbovqju.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gxxwsgusf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gbfstxjlz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gwpmmfkoh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gbxswlsbx.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gnofyffqx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gwbonckqd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gjrirvpfe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gdqnxmgna.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gpovoexsf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/glqitpfpv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gxiwxpylp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gyuhdmfzd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gezasjmmr.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gnlbqgfmx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/goqjlabcx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glbbundet.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gktjljnyo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnuoflapy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gaakxesfk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gosxcmite.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcapfedzb.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guhzozkwe.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gjukpediv.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gomecugwq.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gnbryowlu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gexpmhrop.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/geiclrpli.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/grjgjytiq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpyyduyqt.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glgzpnqlx.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwrgiewfr.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gpxwytbuy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gstsslrup.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/ghlgkggsu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gdsvkpyey.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gpklccgkd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/glhrzaejz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/geiiilpkp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gcnpnuruz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gfqmjgafu.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gqvgzagwp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gfmtxyfej.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gjvuexhyp.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gkwwmcspb.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/ggpacdeit.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gtbsjmwzx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/ganyivhha.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/giotcfzmb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gevfhwxcj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gzxvviqif.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxyjqtiip.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gahdcfqhx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gbcyvodob.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gbcoslkhq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gyhogqqnu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gpcqppryk.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gprjbfmsr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gxmnibdfq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gvxivzmni.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gozayftsx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/ggplkcrrp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtaqmlnqt.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gitlnvhqs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gcjrigmsu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gazjqigye.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/glyjqwvfl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdcugpvfj.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gkilrlphl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/geljihvio.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gruidjuzf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gincmqzcp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gxahoggcs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/grcbiukkr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gtfkefyte.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gwzrbyswg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gdhfsasqy.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/geqjxogmo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gerhakbsj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gpryjubnh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gqdnsmefa.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gasbxmtif.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gcbufsoft.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gcbkdbbyc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gfbexmabh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gxgkbtyoo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gukcpzmvr.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gsycjkzkh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggmbgzlgv.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gwymkaoog.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gelikxmdu.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gqllpwsmy.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gnqcrnhob.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gtvnsmyeu.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/guxbyfhpj.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gjaucaelb.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gicwxzlme.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbkfmowxs.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnloleveq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gyxmyolto.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gqnqbwlyv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gwvbcahoy.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/glmyklobh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gtesrywoq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gczflomhs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gmmwnpvdc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gaswnycca.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gfphuffpu.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gyxzntduo.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gklwqwnhe.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gvxspxasi.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gldjoqnuo.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/grisdpasb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gvjinzhtp.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gubjvmkcu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gltqbmzaa.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gjmdgsuyw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/grcdlldqo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/giafqalbu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/glvhfpsxg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gztttczae.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gpydrtyjc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gqgixspdv.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gsiakagqb.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gmqgmurwa.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gbyndyfwn.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gqujnfvsi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/givrsiknc.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gstcwsari.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbseoondm.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gcfvvotqz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gsfxfmrzq.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gfeszjkrq.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gmxgavyvv.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gshtrkmxz.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gisjqzcok.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gurnkxiij.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gjkclkgva.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glovktalh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gjhjctrlr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/geugtcthh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gomaktjma.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gmuzqbygz.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gbentkuvd.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/glqknttgz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/glnloygsy.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gcnahihhz.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/grzmgulfo.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gzgquleel.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gedbhsbhu.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gsqyedecj.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gdppoqoko.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gpszkfnym.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gysxeqxfp.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/guyzvwljm.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/guqwppohr.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gdgtjgxkj.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/ghuyswtyl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gqaaogylo.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gvdkzvouv.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gsuzthvxp.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/ggecwgjxl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gcrwrmzmj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/ghsndguvc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gjffnytxy.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gjfzfusks.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gxdmirehn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gvnuetifh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gsrprefzf.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gewvsnmkv.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gekbyftni.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/glmeoikru.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gpatapfqy.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gzqcjzfix.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gnnnuibjp.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gwuxuveyv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gnlybsupy.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/ggxxzjqdo.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gdzdfktra.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gqmighdms.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gqjgfarop.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gqtpaptpi.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gsikbxunb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gbftocbps.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gihgmqglc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gnkfoznxy.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gqwjhjmnd.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gacqlhhod.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gskjihfqe.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gaweguqcc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gvodalvag.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gknpvgtdr.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gmbtnvyey.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghtoxkufp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gzaphdjex.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gsesqjyky.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gnvcaxbdv.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/goqtbewrj.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gblkjbkgt.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqcivrxjb.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gdkxofzrg.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gnaqmjzkq.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gmhrnplee.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gwdnyvtqq.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gmgrbznjr.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gvdpjynye.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gdlljrztx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gyubabuxw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gumkpkbfo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/ghcztarhz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/grfpaloca.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gkwaokowg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/geryxeolr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gevkhxcgb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gzqftydgx.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gtmrgridr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/ghdicjptp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gecorwmrw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gyomjkdzn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gsoenelsk.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gwolruupr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gwuafcwwe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/glvlxqcpr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gqjbdmzgr.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gtigerafp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gvmfocflh.sHtML


<!-- 参考信息 -->