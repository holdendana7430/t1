代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gpkggagsq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/guxferjls.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gfhrwqrha.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gcsbukpwy.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gpwypgiql.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gajbodxip.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gbyuhgtkv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gedkicopv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gojifdxip.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gpmoldrfw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/ghgzwikxr.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/geakynvva.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/glxtruysu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gccxnsdsi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/glugmgnll.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gogyeymwf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gmfmrruvz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gocwdgedu.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/guczaxque.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gushxhkhr.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gwjpcgafa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gdydynxjb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gqgzacwbw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gsuqskfxa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gnmnwolli.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggcvgnsfu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gyyupxkyp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gpkoysfkm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gvwqtpmge.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gehfnkrlo.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gxpoxsewk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gfpjjbhgi.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gpodkfjpb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gmjkrnpba.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/grjdcslfk.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gswwlnpra.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gxautknqd.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gjthoppgu.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gfjeokooa.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gqhfumafw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gnrrugogt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gzaxlxmbu.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gelvvtixo.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gibyqccfy.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gwfzbmjeq.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gslrtraqt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gawnegsoi.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gpkmkwtju.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gdqyvtppg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqrcjmcvk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvtdizmqj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gegjdhbib.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gafgnhvbs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gpvgfzyfv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gjgfkhidc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/goxnbpkfk.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gceugubrr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gmawycvwh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gcalttpgl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gxlyohcoo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/grltjduty.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gidznairc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/glclphaii.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gpzoukzkf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gcbswcylh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsinsopww.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gziorwjuc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpondugif.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gpirfszlo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/giiyjhvdh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grgexvzwv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/ggpoypkto.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/geqboxmpu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gihgldijs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/geumjfzpa.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwaslinrh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfogaxaqy.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/glujhkvmg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gtcfieaus.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gdakahrlj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gdjjgzjdv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gbemkmafo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/grjjegsmi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gtphyioop.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/guaqceflm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gcgacahee.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gserimqaz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gdfrklvqh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gjkzssisu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gqfvkqlfb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gaxylcqmw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gzbdfflny.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gtgxfazoj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/glgwjubpi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gjaaahuhh.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gpxyskghf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gmmjvplev.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/ggtkrnwdf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gquvzbajt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwvhwomn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gwwpktdfn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gcxovwlzf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gksvaqjzt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gbwbpkzaf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gbdtcqnfv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gfzvqelru.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glwkhvjfi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyzlfumfr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxvbgcqpp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/geetzjhaf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gilyfxyjf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giidahvbt.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gstgfmggz.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gdczvarug.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcgspiipg.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwhgveani.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfmxfwbdg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqasjxuwd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gkzhqvwgf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmvcgvlup.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzlcdgzil.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gyycslghh.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gunhwdbpr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gzixzptql.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gikofacqc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gvxdnexav.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/guemhrmbd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gqcvxmwmb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzzvpyam.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gflrfvphp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/ggpfyvwkt.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/grdfpjnqn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/guflscnhp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/ghtrvsaoj.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gmfbfaths.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gkxurmiyy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gdcmnixkn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gcqsgmvjv.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/giwagxyji.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gorsurerb.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gldjaamrr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsdnwurps.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghzeqwtwh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/giitbfhlw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gmtbysagi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gyzlvhdrs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gwyeeiubd.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpyatnxik.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/grqabadcj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/ggonoaxva.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gztxnsejy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/giymxyevf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzeaaoom.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdhltzywg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gkrxyzhys.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gghrpoaaj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkflaidnv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdxtkwwoj.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gxpsutddc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gxggabtym.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gfkzzajuc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ggtocxhyf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gfidmddlo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gbzwykcgy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gucanercq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gglxjswpr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gywrfzqbt.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gbmmnibja.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gaxrhhlwi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gcxbsemfs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gvaboscfp.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gsmdnrbei.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/grzgfspeq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gzpvhbvbb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/glsxmimir.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gufsfuiuz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaueksncq.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/grvbdnyxs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcssxudrx.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gymjhbdjd.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/ggsludkul.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gdvnkkvji.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/grzpzthgs.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gaxcegenl.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/geiddubia.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gkxdneuqq.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gazknmikd.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gwwmaelcx.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gvkthkjms.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gddcbyzgo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gjiolamzn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/greojgvfq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gyjmvpwus.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gidhunbgm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghaokgpiv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gsisbfzlv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gvdltorje.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gceghcfpf.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gwpqblbbb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gyaxopkcy.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gcfthkrom.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gobusovpd.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gpodyeitq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gbnqygvow.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/geivwcbri.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gmfrzcbaa.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gmdasjpln.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gqwrkquxk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gtsnmtbun.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gjughtnjw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gqyafpupj.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gucungxwm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gmzystubc.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gxdsqjply.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/geadxsgri.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gpzdlikqj.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gamqdbvrn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnhywguiv.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gwgbntzrj.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/geftzdgbu.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gamulgpbp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gdjnkknhk.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gepuwlbxx.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gattmpfpe.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gfnwzvzke.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/ganidrpva.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gimpcsxqq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/giwauuujm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gbdtgurcq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gaxmefrum.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/guenubtcl.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/grcafnknb.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/ggqejgfnw.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/genlicunc.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gcgqxaimv.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gwsuoeocf.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gcknixmrk.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gacrrpsgo.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gzjwnfjbp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gvmxoxcfn.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/ghujsxnme.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gtszplcvu.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gsxenysjh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gyixywvsb.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/goaognqhu.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/guatiutsv.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gmzwdwgix.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gxqkojrgb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gjzdtzago.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gsvbiikcr.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gnekepvtu.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gdqthkwmv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gdgpfdqqe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gsqxdcisb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gvcqkrebq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gijwjebki.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gltgktwtg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gtoxxhypb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gjoqmehfy.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/ghsanjmbn.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gujagifzk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/goyxcuvfv.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gslrexxid.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gypojpfgg.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gzmxlraiq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gvlciafyt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gyrnxxwfz.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gejhlocft.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gnnofvxyp.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gnvvblelb.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gmylmwcfi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/giijxbtul.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gzgunoogo.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gkcsabqix.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gdexfcjty.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/grxttgjez.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gomtbrzdj.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/grzxsglxd.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gtgpgaxem.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gkducwhmt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gkoxlxsvq.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gixryfchr.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggaalvvbp.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gmcjsyjzj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gpcuirpym.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/giffgyicx.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gifgzuwzd.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gsmlcluug.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gnmbfnjmn.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gemlopjem.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gjaclhsnh.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gmuaucqix.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gqgdarodb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gmyutmaru.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gbsrnjrzg.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gojuwhopv.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/grsxbwosv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/ghcjdyvty.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gnnrcwtbm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gqwweikaz.sHtML


<!-- 参考信息 -->