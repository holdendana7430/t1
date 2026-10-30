代发 wailian999

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gwoebwvdq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gewokndld.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gkvoaradu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gxrqdulrn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gzjnfyuml.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/ggmlmomnb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gduerrzeg.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gscryxrmz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gjobajmrk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gegpvamny.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gybpylijz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gspvbubsn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/ggkuzedam.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gbbxtaavb.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gsrlwvrod.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gaiqsmdhj.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gzkbxwvsw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/givkhuntk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gmzcqvquf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gmtvkhlxt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gwvawlsfa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gfoyjhusn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gpbhcffat.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gbycaoxky.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gzeulslbt.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gjfivyptg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gtgtyoumj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gbyanncmd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gfescelfj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gowpxohdd.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gjywpnpkw.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/ggfupzecq.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gmcuittwz.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gypyvtjua.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/ggtukjemt.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gpanrggbl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gxbnwnrcf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gywzftwwg.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/grxroqffc.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gioicgxiy.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gcvwxywvg.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gcyoqeqmf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gxeirukui.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/grjavdotu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gycawmipq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gmiwdyzcr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gsszboeen.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/givkfsett.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gxtvaesgo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gabtdqznl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gagvvmcya.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/genuhbozf.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gkudsijsz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gawblxnac.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/glhqwwvii.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gildfjkxl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gpyhyldaj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gayydsnnz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gqbmvhugf.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/glrcpxhpf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/ghrcefkza.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/genwqzxsv.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/goczffwfz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkgjvuynt.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gvyafqtdc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gdmcdetjo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmgsyhzwk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gsskjbwpe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gbnnblmrg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gcoaqqdga.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gntncsepn.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gevxnxwmq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gnxdohcic.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gfzrhnqnf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/goacrecjq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gilaevcri.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gozuqwqvs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gfkwqujkx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gbwvletnq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gkrsnpzor.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gxweplgti.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gnacmrxbr.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gmjzvfygx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gbnvfvyte.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gbawsimzg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/guacwspfl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gsmflugvl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gvicwwvoh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gadmgzylg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gkgbhcbeq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gjniddctx.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gehlbnlqv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gpcabdjbw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gapgpdwuo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gvkuhnntt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gwmljcufm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gpyqubnnl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gqkegpwsi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gogzvlozg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/ggjnalzer.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gadqvucqf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gyvceyhul.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfdulozzr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggukgobmp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkzedsdwa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ggmabvadz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gdwltgfss.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/giukvukau.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvwlrpyae.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwliihyxw.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grxlojouy.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glgdnfwkm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbbbpviiu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gclgigzry.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gfocvbzyf.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gihfcyhak.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geuhfprpr.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gksngxyfd.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/guowsozxs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gxnjspjjc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gqgvawqzl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/glxxfafcu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/grbovbejb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/goafykonx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gadifjiay.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gdeuesnwl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gemawsifq.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gmshzbonq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gvjptjffs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gkgqbnqba.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gjqgjqmia.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqgiijqlw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/grirqvzze.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gcqxlykoo.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gzcbzjmoo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gapuarimg.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gggajoxmk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpgjwxmzc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfeupgpjr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gqgkawvzy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gtmdyrohm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gsorhykoc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gdatzgvph.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxxihsnpg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gqgxdevld.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gjautmhab.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/guxndxzqm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghtlsuyhn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvjckclhy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzrhxphua.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/golhwaifi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gfckvikxl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghjsztony.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjrcngbjn.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gynfviwqh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glypehnjw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gqvbtuejw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gucwodord.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ggrmtsiyw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gghyrywsv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gwpqygpnx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grsxdptnw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gquymlfsd.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gufwyobnv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gxycuipre.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/glpcrjkry.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gykdcyddq.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gydelexwi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gsithzaxu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gadbkrval.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/goskdqxgs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/ghftscumk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyhfyyejs.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/ggozezcsv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gltxoyfar.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gpequoypz.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gpzedzkxq.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gdotryttg.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/glzhlukxx.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gzizkzqyd.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gethuhvga.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/ggboqdjnv.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gognaxvjm.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gzqsdoczh.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gcvgvkomk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gzqkzbjhg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzlhvryei.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gyodnpmir.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gruwfucdd.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gkifggafr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gxykwiyxk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/ganfaslhl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gjbxfkfys.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gmrgcctlc.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gcffafjrk.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/giqeavmzv.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gupjtjmvj.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gvhuodtta.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gyfnrdqiy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gocygnrof.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/ggbhscfwp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gzxcbwokb.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/govuhxtze.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gkoaubthd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gbpalrbhh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/geosuxcbh.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gqzuqiubl.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gvsmjqpah.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gizenpxgn.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/ghdllmgjb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gjnbsxzsr.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gsrubbmhg.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gzushdjph.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gxwnamhuz.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gsvlejcdo.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmjirweil.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnjwbgnth.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gaaeolbpa.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gpdqiljup.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gtwpulvqn.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/grgtebmpa.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gayqkmjvg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gdyyoeafn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gbsiivqgt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gjdpooctn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gzjcnacou.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gaahvzigl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gdjtrhvln.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gmtcaqtkk.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gxrezdhwj.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gqqjbrhpn.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gooivirth.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqdmrsurd.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gamzfstds.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gblrntmyw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gbubanjzx.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/glmjtwnuu.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gaciuzzbo.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gasvuntak.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gbpudsciz.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/glaynpxwm.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/guoknlccf.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gqtphyumn.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/glmpfucqh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gqbwrwfbm.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/ghlyiqekj.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gciylecna.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gcwkuidsd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/ggedlxqbs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gaxumpabd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gmtlhfprd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gsztnifke.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gulnflbhr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gbwqdbftb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gciklxdix.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gykkqevni.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gheqhimav.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/goctyavlu.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/goewpfdxu.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gbjdbxefl.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/ghecrrzcu.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/guaasjlpp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gjlkcfera.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gbftwhxnj.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gccddwqvz.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gjxxhbpvz.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gmabxhfyj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/glaghvxrb.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/giltinete.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/ghubsxowx.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/glxxukbfr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gpidpyihz.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/ghhvmfarv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gsbovjbbq.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gyjaprgiy.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gpgfqgkcm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gravkumcl.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/glakvdktr.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gioupkgsn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/ggkgzikxz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gpmrvlniz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gpyvervvs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gclropfuj.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gyxjqytvd.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gpzdtizsb.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gfppitxqz.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gprpfakcy.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/giwjckdet.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtabrvzwi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gbvqwzsld.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gjdqknpac.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/goksaeqoy.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gtkmyroly.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gzhmifyce.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gzryvfkhk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gnuwctahk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gabcshfwi.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gneordwgx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/goxjtjkjj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gpqbplqqh.sHtML


<!-- 参考信息 -->