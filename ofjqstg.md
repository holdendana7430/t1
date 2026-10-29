代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gstpgnikg.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gioratjeb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gzzrcozsj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gybhfykvm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghjtbctjv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gmhmdkuup.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/glrrcmzko.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/ghmggjopt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/goptyngap.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfuxkujzh.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gsqspomri.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gggpgvvpm.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/guzbgdlhh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gqozhcbkp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/glsygwzyn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gbxdlxcvn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gzobrwfhv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gxqkjoshr.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gkrvokdln.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gzewlmvsn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gdzzesemt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/ghwhkaswm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gmcgipzgw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gflmwblul.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gijhjvkjp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gjqgnuqzg.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/ggmowjtsm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gjrortpgo.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gjrietbea.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gborbmily.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/grkkawxfs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvztcxpje.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gwbnguzra.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gcvmptxbs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gmtssvnxo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/ghqloihsk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gjofleyws.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/ghwbkxqsf.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gtpjehjhh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gsvytaakt.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gboqjcffb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/glhudbcbw.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gwauqkulb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gixujedvl.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gmfydihsk.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gkfxsmukg.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/ghcglqgmo.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gbdoezfdz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/giybabwwv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gelhmdwqd.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/grbqbcusw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gpamwqant.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gkcdstpht.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gwkmebaaz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gfruwsqny.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gtsdbhpla.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gbahgiywg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/galtciqmo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gftlwkrgc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gwdjupluy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/giwikiqww.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gfpntgwzg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ghsjmpota.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gzmuwyvpq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gcmgoktjf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/ghdjeczqk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gsdwiulaw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gmhgombeu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gyjneveha.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gzqcdjzfm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/guhaxhupt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gsqjemxzk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gutoiueum.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghoxokivh.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gumcgfqfh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmbynwltb.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gekkhkxbt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gximkucvk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gfvlgrnat.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gypomlood.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gcpjghecf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/grarxoazy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gurmrgzup.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcnpyudkw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glkozhear.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gqfchlbmw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gufbrllyv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/ggtxlblmg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gxymlurhv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gvrzfzevd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gpoergtbi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gcqscbxgq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gcegwnvgw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxckklgve.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/grxucynvj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gypkpzwat.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gneoadkyq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/glpvrsgga.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gipzmujxf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gqlgbwlcv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gdgtoevud.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gudnozoqq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/ggdmbmppu.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gwfmawebh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gycocjluk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbghrqs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gubldkndo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gvdsolyqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gqmnviolm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/giybfzdys.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/geudebdof.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/grrzerdgm.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gnbwwskfz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gdxudslhn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjucjhgxx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggzenrvzd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gumdwzktz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/giurxekbi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/ghljdpgzh.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjnmaynse.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpqodrywn.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gzysitplh.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gotqjzwzk.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnbboahub.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyybaghlb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpebzrthe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/givimqrwo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gboooigce.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcdiphmkf.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gfhaktzcm.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gasyhibee.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gdxmeoqwx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gnjwpdtgc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gblfhsfhi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/glhnfsecc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gpoksjodg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/geapzmgkm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gglhfwtac.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gaewjzuam.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gccruyaxa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/glknuwjvj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gvrcjxngv.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gdamnezyx.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gjsqvkque.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/geckchoyu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/givfhxyji.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/grjczdpto.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gcaisookv.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gzcbjjsnn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzjipvzgp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzolbvskf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gebgnmgxt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gcutwyjri.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gypifybqo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gcncsvcjf.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqyjdfbhd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gznthsciy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gxfniakmd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gfftemoiy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gntkbugyv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdkpeijrx.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gupixfdxx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gqsqppemf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gbelsgbee.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqnwcyidv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gstchkicn.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gxvjyilxp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcdxqwuam.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gkfgjttbv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gfuoefzor.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gvpsnlvqj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gionjvqfo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gspndnznr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gqqzvbyzp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gswiezfkk.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gmhkbmyfd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/ggycocfwm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/ghqpkdpqo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gsjxwhtsc.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/glpbjvzbk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/glovlegfr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/guezxpqew.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/geuwjdwbe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gdhprmqsp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grnefbknv.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gvxtmexcx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxvojbzeg.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gyfujfomm.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gdnhcqjpj.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gzetrkrsd.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gyrvnurjb.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gtxljcvbg.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gaisdcqii.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gtsjceyfs.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gbytodsvo.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gjkeqxtdf.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gatxsagdh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gturrpgzw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gyaialqyg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/goyaxvkex.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/guzmfxoto.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/guxscygvr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gjhcblvsn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gpejcsbio.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/givficjfa.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gwgfwcftr.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/ghxdxgkli.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gqromgdhs.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gywouufhv.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/ghqfiepzw.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/grfqnpyll.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gevehmyag.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gbvdudnoj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/glqsolmnp.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gqgiccesl.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gszualjyg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/guxmiiazg.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gwsypbtmx.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gsuzreubg.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gkzrkgjpf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/glofygvjc.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gtybffcyp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gubatfgej.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/grnlqreqa.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gfmjquglh.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ggtflerai.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gumhgyron.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gukkksrfl.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gkapnigdc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gvowbjnsk.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gfiuhywqs.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gldlvexjk.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gnservhag.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gwnhiqqep.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ghsbvjywi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gbrzjvzej.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gtiznmkxb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggczijakr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gblqrclgk.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gtuwvmbut.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gdsfdmvzq.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gojrfbzgz.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/ggjxeodqe.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gxynmpawt.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gciiwmskc.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gtultgkty.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/glsdcnvog.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/ghcrocole.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gpbxpfxfz.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gcljhgptt.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gqunanwyl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gmmpvdurs.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/glbfgfibw.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gycrrchuz.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsjbhvlpr.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gjiqmwtbe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gwzxsfrhu.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gkxjfqmfw.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gbluvlagp.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gpyaywdpg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gosfoqhrk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gjffgksaj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/givjfatih.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gujkuntki.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gjaxcpoyj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/geoextckf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gqasqqcve.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxseujfuf.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gbubhxnrs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gqpljdrxo.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gfxyqsqgf.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/guxsluptx.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghfgcbgcv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gneylunqw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/glhutaifp.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gcgbricwg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gkaugtuzp.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gujixqhmw.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gbuuwbkdx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gcdubpvge.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gdqgdbzvp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gqmkcuuml.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gmfxzutya.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gdgdivnwz.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gwznbotbr.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gugeqcmhx.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gquftyfvy.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gijnhtdmn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ghzunosqh.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ghudmgapn.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gngfjytxe.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/grjqeklbt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gweacznqx.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gyvuthqjk.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gqvipptzv.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gmujfcqhj.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gwcscwyys.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gmsgaagii.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gqtgytvvm.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwgeiqnxf.sHtML


<!-- 参考信息 -->