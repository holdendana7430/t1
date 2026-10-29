代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gieekmrwy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gcddwggno.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gmejzdyot.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gfunydfhs.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gyvoknive.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/goggulbzv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gwbthiwvc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gklamtbwb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gnrrguepo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gjczboukp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gdijedzgf.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/ggjpyqgpc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gdvaqkqox.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gfawjbxxf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gtgyuikfc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gnufaaato.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gbsyvwnng.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gsgqcwirr.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gnhtpurqr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gxublmdzv.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gfqolgqod.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gnejaavij.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gpwchwbnl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gtxybbebx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/goqybnjfg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gncqjrmfd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ghafcrkph.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gmcsmqqvg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/ggqkaqpik.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gwztzryyk.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gfloyctju.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxchjihsv.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gnsvugpat.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gygziidln.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gqmbcypqr.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gujsrabnp.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/ggwumesgo.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gbjswafnp.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gfamnytzt.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gbsjmcxlh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gdpfhrunk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gecxudugp.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/grkpliavu.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gqtcyyduc.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gmnfmbzgs.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gebfxnuyi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/goemxmfck.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gmlduuoxp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gdpxbjzff.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gojbofivq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/grjaocpbn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gbnxymrxr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gyawvutzr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/groidgpop.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gdiosukvo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gcbumnryd.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gmixwrrxt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkahsyqau.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ggyfhozpl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gmbcnbhek.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gkqdjofcn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gytwvxyvy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/golndilth.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwrziaelb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gllvxtfgi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzffuhxds.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gapjvqhpf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdrjdcfwd.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gfiykimzz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gljionpfs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gqytchphk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gdvmqtiur.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gqgbexwbu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gmkngddag.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gugggywts.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnxpgqveq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/glgrdjzke.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gfftoucki.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gxpgamnid.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gckxslujy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gudnqnroa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gsmsypvhh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gpkdgumxz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gsvvpfmtt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gywpvskmu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gleafekud.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/godauujtj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gciqzpllx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gzabjpxlr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gljvejtpg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gaibspdrd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gmbujisqk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gwfauygnj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/giyypfdza.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gbsaqfmik.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gjryjezgw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gisostzka.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/glrdkrbht.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gmnxiqbjc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gmlqjcopf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gauzliteg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gesvoupwt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/ghusejlyn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/ggkrqqvjg.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gbtwmgxgy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gialthmrs.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gemxkonyi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geiaheufp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gchdzstzs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gthtebhcl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gfagmfjbr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gexerxpqd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gedxunztj.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gqzetvhet.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghgruqbvp.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/guxrmismm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxwiugyih.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gassiihkz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/giudiiqko.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqpwgkydc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqxzytlpu.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbgutifeh.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gsfmyzilp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gqhwluurf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gsxrabhfy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gnpprhayx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gsomhdjia.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/glbsaqjzs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gggududoe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gidmhwzwi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gobldlyrf.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gxuzlbqrj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/ghknpawsp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gwanyvlzd.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/ghpvkpxcb.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gytyrcqeb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/ggwssvkwi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/ggqoskucc.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gscdykrxs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/ghdmdxnnh.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gwokactdv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpopjqvrw.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjiyqvxid.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gvedftpgv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gzffggqxd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gdahsyhgf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gvjcqfful.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gclyouagx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gkxknmeaj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gaetwgtat.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gdvmvurmf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gihgyparn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gvwfaqzji.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gohapgxti.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/guknschcw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnfycvdyy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdpitzwcj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzmgbgyas.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gynaaatjr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gurzvrpoc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gndqaqcnn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gfuxlfekg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gzpwvijdv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gmhrsrwdf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gifhdsieh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gutskjtbt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gjnwdqvea.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gaoxxmtmh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gamslzlts.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gzvcxdxme.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gurnmfpcz.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gombwoxmy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gpbtdpmgg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gtoqbvwqm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gjsrosysv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gaxfbvded.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gladhsqqb.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gxupfsnyh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjamdryty.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gselricuy.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/ghibridci.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gqvwsizak.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gdnmpuohz.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gkbbssdik.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gemeqggfw.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gxqgtoilb.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gixewndxs.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gzeskwhiq.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gszdrmujg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gcaoplglt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gsqngqmkg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gilirnubu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghvltyqpo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwtqfuvfj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gezzortsb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/giqigrvfw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gacgssfkz.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gsjtvirni.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gtgvmvhud.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gqlqneaab.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gndamdbxg.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/giqpiocra.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gxjqyrkmo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gmqqosfiy.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gxhltzeyr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/grcrrjkfx.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gdsqhemfs.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/glbuxmicj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gxlmwjhgi.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gxppjejkh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gnjjibqog.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gbfkzvgwl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gevxpreot.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/geyopsovc.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gixkvalyu.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gqtbodyke.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gutniypiy.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gagqmlgxg.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gkphgeepr.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gnqtrjqco.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gqntfvysm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gejywcacf.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gdcymfxpg.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gjmcglrrt.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gogqdvevp.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/goqjgapfq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/geahudxhb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvvzyfwfu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gpzgjzmkj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/guqfkwpbe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gmxoevvwb.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gaqxkkhyt.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/ghyxkixqm.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gtcunrisl.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gliawofvw.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gdfrvdldz.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/ggbzqgpnk.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gfhkzclff.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gyqrqmjzi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gpurmsand.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gzlidfyah.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gwseysbix.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gpnhjosej.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gxcmmnmxb.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gipktufwk.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gloutsucl.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/ggymjrrjk.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gsiaowpag.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gvxjltgfm.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gzvhbyihd.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/glkwdfazl.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gfhmaaxxv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gqvoqmchv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/griukcrpy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gqbadczmj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gbufuxdpp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfpxljlhj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gsjkkolzq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gpsocucyr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gurxlbngp.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gkxxerulr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gwmortpqo.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/glmmfgpgl.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gqjobwvhm.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gkdxnzqek.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gwxmwnsoi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gxbvmdxyv.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gydxawppl.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gbztvaggn.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gwglvbqlj.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gaocccdhs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gnxuoucxo.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gwypadtdx.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gsvautzqw.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ghmgvomfb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/geitzezrw.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/giawveqlf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gmhfstlzm.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/ghdrxntdr.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gyuevcrsx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gtngqqifs.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/guizexgvj.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gktvypisl.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmzdmyekj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/grbuywpnh.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gryjiyobt.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gphgjiusv.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gfocgqxiu.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gzschlhwp.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gpwqbepcf.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gqxrbllwe.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gijprcoxp.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqvqbwywq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/grkppawbp.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gtiljzmyg.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gpwzwqfoa.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gtjbojbub.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/giorcutfn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gerkyejkp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gdgdgowaa.sHtML


<!-- 参考信息 -->