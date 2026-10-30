代发 wailian999

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gpbimmyck.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gzpqgcoue.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gzwydutby.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gsznuiixn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/goranmhyg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gwjcwlkie.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/ggcxgooif.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gkinhophz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gfpcejxig.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/grxlorjpc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/ghawicqbc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gioismtql.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gtpkpqcsu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gppgogulv.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/grznwxazc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gmzypecmh.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/ghaazugfb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gatfaimld.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gtdoqpogp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gfdmdybax.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ghjoqlfqk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/grvpivrfg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gvcdsockp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gdoldtwpf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gptfoobik.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/ghvtnmkdd.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gwfnviqrw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gnpptqpkk.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gorcrfiil.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gzcnfnipy.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/ggkvvgcty.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/glgbqnysa.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/glotkfqmv.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gkjnoqolp.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gcjtsymva.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/ggacsfggi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gimtlkagi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gctfanxxn.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gtohejznw.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gojwbgqhq.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gtutlkuxs.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gkpoxclbo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gefbkikai.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gbwowpgyi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gwvwyfbha.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gfrfstczo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gsftggihn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gpbmeyxgg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grwzdkqqe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gmqzipqmo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gskhcdeyw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gdknlnsxn.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/grvtdvakt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gphmiuuiv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gksjxpsdj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gbsldmnkx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gtyyzpczk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gcojofase.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gxfjuvpmw.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gpepijdii.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gpbxvotni.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaohrqqoq.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gojmbdadj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvtdeybnd.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/guakacczo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/ghlnzknda.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzbgmpjue.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gfcsqfiwq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gvjntwsdb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gomqruwgo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gibnlyybn.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gceklxkmj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/grwcwriiv.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gilnukpzq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gjgrmmgqd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/ghteyrbcf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gymsklrai.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/grgxjwsgy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gbthyvzfn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gciuxlzcp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhqlkzsb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gdksszhbg.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/guzksikph.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gfujipoup.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gfaerirrj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/ggxskanfu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/guecvmahd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/geeoogemn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/govxxecfo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gryurkfgx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gxvqlibcv.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/ggxeitppt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/griibsdrn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/giceueeti.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gtlfiahtq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gqifzjndg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gbejvfbtd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gcdupfjah.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gkcopdrbp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/ghwvmuiua.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gmefriaoa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gsznunpet.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzhcnrobf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geyxggkeg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqzvgjmvh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwpigydxo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gicupjvkh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gihfxcpaa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gamgmorud.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gerojrznw.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gddmrzfqx.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnkzgvwri.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glcgjegdv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjzwylegz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/ghehbdxcs.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guhjmnyeg.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gogxbznef.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gahwwehyk.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/geiyngyyb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gxjtpjvgu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/grquofdco.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/ghreygafh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gssqvkkly.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/ggpohpqgx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/grujuogrg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gexepgipy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gjivdkmav.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gvqnkpkeo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/geawczybm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gadcdfejg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gpqdliiuc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gamfzhutq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gdqakfxfx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/giwzzsyio.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/grxisehtp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gesfdyyta.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gbuzduxuk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grvvsufjn.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbeeocqtg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gfzylnedz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gmiuzprir.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gnuvxxcdy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gnbuefvda.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghtceejwe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gcndasdrw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gnvgfvutz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gputupmdf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gnxiabkqt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghxqcbzrk.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvckdpvgo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gbwmoafqt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvmtrhoxn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcwqksjmc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gizyjdekl.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gefrddexg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggqcaywhd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/glkbdgzmx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmdikqpxq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnhfcvakj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gqccfbuzv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gtvpheivu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gukzwrsuo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gwydoaedk.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gkpdtnwol.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gmhjjxfgx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gplpcldjv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gqwukvxjg.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gmgtrqbhv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gacigxfov.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gwjtinjfn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gkishyipn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gtydllpdt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaidcvszi.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gjemmzvtn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gprfyjjxc.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gkljmasyy.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/goqiywtpa.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gvwkpxgfp.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gagnljezs.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/glwcljaaq.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/giuawsoqc.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gltpykapn.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gphcffint.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/ggtrbkfcd.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gxutddykz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gtpwnlzzf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnrqlygqe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/goyqawvgp.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gwyaxucbh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gtzmduane.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gpuwyeitl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gqpczfzqx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gqktrjcwd.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gbbxalegc.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gtwanuiot.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/guktxwiux.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gbgqbckln.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gdoehlgzk.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gpanjtgrj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gvpxzpmuf.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gjayavvmv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gbkfvajqp.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gvibrwzfz.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gaqjkukdn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ggolnqzir.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/glhduqjcf.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/glwcixwxw.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gzegozexg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/guugkirxb.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gbfswdkgi.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gyyihbwpw.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gdsgxworh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/grhqctrjv.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gmcmvbjrd.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyshsrmnw.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gwspmtsvk.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gpclhzdte.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gxizmbpbe.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gdsciaxij.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/grribvqid.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gxvkospft.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gbegcctxt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gkbvzbamd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gbomwcicq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/glbxnotlu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjdfdwhlm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gbujljriw.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gpudastuu.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gvxmpsenq.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gkoiirqzc.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gcayqrrxx.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gfktjapir.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gbogbksso.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gcgodnyug.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/glqzisktc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gczlkdzyj.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gntwtpbiy.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gpvvwfkrd.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gzwxbclul.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/ggljijcij.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gjvaaxfhb.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gccdrbsit.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gqsizyevf.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gdijbfmim.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gypnpwzds.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/goxgmubmo.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gfpfaesoe.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/giowvbqfn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gthhpcwof.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gpfluenoe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gdpuoipce.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gyzwcvkym.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gwjahufxq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gzephxdqg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gwkkffkur.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gghbqkefc.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gnozweihh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gtzfhjpdw.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gnuguveog.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/ghuzwshot.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gcxgzvtox.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gghcjlimk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gzlfpiixi.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gkuzyaast.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gsxfsaies.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gssmyfqlp.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/guiyvdhwz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gjyzlcoki.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gklbuvemh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gnxoihvye.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gprhxwtoa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gplzlgcwh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gnqkjhaai.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/guhrchzgs.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gcmibognk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gjiytkyqj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfggyspfh.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gicpvkyto.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/glcwtdavs.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/ghcenhldz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ghiixohrx.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gshueyikf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/grypugunw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gjfdcpvqx.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gblsmvyci.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghkjrmcpv.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gjlcgcaun.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gnwfnuxxb.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gbxdztzvx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqinrtd.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gspzrhsmu.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gnqoeeepm.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gfwoxwpyh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gjapdheut.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gszgxtntc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gndwconoy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gtqkgofdk.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbfuahgkp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gifjwglfx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/geowrntkf.sHtML


<!-- 参考信息 -->