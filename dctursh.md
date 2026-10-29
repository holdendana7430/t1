代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gqlglwhgd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gkexlsfnt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gctgazrlx.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/goxlgzbdi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gjnapaygu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gxwidaupv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gigirrbxm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/goebugntn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/ggwzsxbmq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/ghtmzjtco.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gqlqymqfj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gtyxzwpmw.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gzcvtlome.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/ghxtoskiy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/ghwiaeuex.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gqtzzuftl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gwvxtbysq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gtxxietot.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gkxotdncb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/golzpbobs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gwpgayjih.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/grxyfoauq.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gtcueuhzq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gsjgoehzl.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gskqybqpc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gqjqczxhz.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gqqgyxugb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gzrkknacx.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gwykwufoi.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gbfimsgdm.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gciwlegdj.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gjkqzvgud.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/galoqcrts.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gdwbfzeet.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/grcijekgs.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gyqbjccmb.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gltlhysht.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gmgeapmmb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsfccojnx.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gcrkkytvj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gqqdodfst.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gyridcjaj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcamjdcbe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/ggwblnuvm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gtgdguble.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/geofwcziu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gdxyuxlus.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtoezopug.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gfsswnmbb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gpzdyqtkc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gxzrulgpu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gosopceeu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gzftawisy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/grtdakody.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gvzyhyakh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/ggqlnampv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gwwhjijjn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzcrhmwac.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gavmazgij.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwdwgzowl.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/galuceulq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/glruwywxp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gencupuva.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/grqprpiba.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/grpxzbfjn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gldwlleew.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gdxgemgxa.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvqjaoucr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwfunevyy.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gujclffuz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gqcasrbiq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/grwdrwwzo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gokoxqqxs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gmwhshiwa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gwsddrcge.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gprjuwukt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gremvizve.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gpldxqnbo.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gztemanyn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gcyakresb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/ggfgeqdzp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gnuabxeer.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gcvfrbfhh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gudmypqbx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gidqxvblz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gnsztarcx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/garujwekb.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gnfunsbri.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/ggufhfmoi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gwuhfqmbn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gpechpsbk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gbefuwpfa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gokrfgkhz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gvqimpleo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/glqgsdauv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gpwahengg.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gzfkagtvq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gvgevgosm.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glsodfbkl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxuxqqfhg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grwkeoaek.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/glenstdsp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gmpbrkgnx.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsmfsaekh.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzwryaivb.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gwqfztzaq.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsexymdhh.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwvyygjlq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxdvohgka.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcsrzjeea.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gfyfwlcax.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggaplayqg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtozursip.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghxisuhzz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gssldlrcq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/giqerbcfa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gmuxdezsx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gdfjhbjnd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gizcucknn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gpfjguvau.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gvbnmsduh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gkrcjyfgq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gtvpyhxmz.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gkftoarfm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gzcxurmnl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gmxeckzev.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gfjmfhtmz.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/ggqnvjnud.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gqjhayyqo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/garxpuurj.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/ghtbvsbhv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/ghdenxljj.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gpqaemter.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gffjzpxpe.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glffzxgry.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gkqifiepu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/godkcrhaj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gxvqxkeyc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gwzqopvrv.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqqxpxqrb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gkaddhlfa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gqhmjlrod.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gimhwfexu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gacmaejfb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyeatcwtp.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggydybkst.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/glxkbxyrr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gzehujzpo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gamoojcbj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdpisaibg.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gkewglosp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gbtbozlaf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gdufxjxsk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwixbinb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gtcigcwqs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/glzxmdjyz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gsusvivkv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ghldrhfyq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gypymfsfd.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gjspjiclr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gmrztfnbe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gujzfqnam.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gdacoglqp.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gbmssghns.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gfglhzovn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gcobpzdtg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gfglzloik.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gszwlgnbz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grpbzuzqr.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gohjdkyzl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqfzwbykg.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gsigrjpqn.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gwveyutsp.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/grehycxmw.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/grkoriwqi.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gtgkixmhx.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gbmlztydl.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gksrcfhwf.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gkcnfcyuc.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gssgtxqyu.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gdxikritb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gnvgfatio.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdkkzoqxv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/ghpnnuyqf.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gjqddapan.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gvpbkotji.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gthkuobcg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gvvvgorcw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gformsjaa.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gltijvbgd.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gilesruxq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gvkqhgqmi.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gljmkgccy.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gyreedpwl.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gtgjrljqc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gnqdswnss.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gnuericbq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gdlnwzlwy.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gietpafbl.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gdixrhwnx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gqmgzfdby.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfwxbzcqw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gswwuspza.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/ghoupfxcm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gjibjferv.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gtolujhkt.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gmdihlsee.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gybrcfvnv.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gdjtfpjie.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gubgdilzu.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gakxrcodq.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gbczcjguw.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gvwiebyoy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gtbkyvojo.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gvgcbdouz.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/giagtjyag.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gjzgermxu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/grnbtlmpl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwxlmvosv.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gavzwishd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwjyfjqfo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/guarhqnyx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gqpxtljyc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gppgsdtkz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/ghnpfevpr.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gwssdqujw.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gaunficvz.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gnkmystnd.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/glpvpumxv.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gqsglymqm.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gjtufwraj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gmgwjxaqo.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gkanzpsyr.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/ghvsmarfe.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gkdaeoiex.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gjoansobs.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gyeeowodn.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gsephzxnw.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gxixkicmi.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfkygjhtn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/grapkfago.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gswjvgfxf.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gxozrrzqv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gymhisrrs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gkhcepohd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gfioefsqd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gemavhsao.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gpdeiyhiy.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gxhbpwgnw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gtkovzjlj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gjikcdscg.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gjvflfetf.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/glaawoowk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gylqgxvis.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gwmsrchrf.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/guqubfxpx.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gicitjihs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/grlyvujvg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gojesyuks.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvdvqxzib.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/giisgllrp.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gprhfzvtw.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gyvcsaqww.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gkallcxmi.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gwjjwzsne.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gcdxtqqiv.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gnrohwbjp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gvnkoszgl.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gkwynmvmt.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/grubdemhi.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gwagpflcj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gcymfzqvm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/guyyldjus.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwznbvlhh.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggjzpodsr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpeabtmbz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gjleksygd.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gmlrseeep.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gddydgmzd.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gefvtyjvs.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gbopuddxz.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gtrzdwfty.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gstakllmp.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gmfszxioq.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gznrhfmbs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gesebdkzn.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gpdavyoog.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gnzdkisdd.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/ghtnjlrlg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gusuwtnug.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gvmvsmcek.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/galnsddki.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gdvcgwuwu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gajnvsxxp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gaouinqup.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gjwtdixtg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gsnqljhuf.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gydvpyrcq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gzftpfzlh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gpxjgharw.sHtML


<!-- 参考信息 -->