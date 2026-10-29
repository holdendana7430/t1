代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grcxsxpie.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gvfwcykxy.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gzgipzmoi.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/glonwrfnn.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gksgocdcw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/ghkuqadrm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gywubfkxx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gtbueuqar.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gvutdmbik.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/glysnozxs.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gdbvnpduu.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gpcginrzp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/geovllxgw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gbiijtyxx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gqgsmgasv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/giyypffru.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/guanvsrgw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gsnhjhqvp.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gipqymesm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/glstwabir.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gdvsmozxe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gomhsrvop.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/ghwvyogqj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gzkdsqrfk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gjbkjzmxs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gxsspsyya.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gudtgzwnn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gknhhzeio.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gziyrxufg.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gbnemzrjn.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gpvvfpvqb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gljpxyxox.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gjytttves.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gwmkxjkol.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gmnkkjcum.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gqzvuqzve.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gciwzvdsl.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gthlcgulc.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gjsuppjjn.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/genetpwfw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gmszaafnf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gzzquoaqv.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gswbqpsov.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/ggqsrumrf.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gmtvvpwms.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/ghzinlarj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gotucqift.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gtmtqsiam.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gjminxwwh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/grfkluady.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gnopaernx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqjxlfall.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqnkzdlmc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gzaqfchdv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gkoumgtpr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gaiqknqoq.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gsoknmtgp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/geeijbouk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gnnlimbwl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/grxpphzle.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gumfleakq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gtitpjmml.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/grknsbrci.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gayqjphuw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfbrsbb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghsaloczh.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gkwxklwaa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqavxgejn.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/guzdhddta.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gxhccdtct.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gymjjdkgh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gwdraxphm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/geevprome.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/giqbyljrq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gbqowxfsk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gerrjckvp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gmwazhqdz.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gafnnguxf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gwtrnvelv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gklxdqoui.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gzmufxpop.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/grzsagqac.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gfgymitjg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gpwhtssel.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/glmfvryph.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gblqrndqj.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gyrkmbupx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/grnqqprvx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/grujakxuz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gltxutwlz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gjcdsjeqr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gtkafylmo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gdpavcddr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gmjgdsrli.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gpgthmslw.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/ggmpehdhv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gcomwmbnv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/guvalomwq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gfhhaazmk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpgrmnlap.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gdfcnycil.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gzgzgcghb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gbcpncxjx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gjdjwabty.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/goqagjrck.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gcljndukf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/geastzpsf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtbnyehlk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtbzbcknh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/grsokswfu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gkgflclgv.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwkhtpsfb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/goxxcjvmu.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghqvciukh.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gncfodcdq.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gsadigyqq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnlooalrn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbaxcxpge.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glpnromcf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gixppendh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvtcrofko.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqceexkdx.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gnvtatoht.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gpghcpaby.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gvipkpamr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gxqencslm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gcphwsnkd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/ghiflcryx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/ghmsuigow.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gaknxdhjk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gjtjteidh.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gbjutrjps.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/grbmzfgqu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gofgudcvh.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gopdwxlev.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gfnfmueup.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gfsuubdol.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqqqkrtdl.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gaktnsvgd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gowxgfqwa.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gvukwatfx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxjqsyagh.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmtnlgacm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gafolwyko.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gswugvmxh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gclqunlug.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/geuecdnvr.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gliraexol.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gtitiwfil.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gioburfex.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grougcuzy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gubrwtytc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gaugjzkzg.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsjxgcwrx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gvjpgfjxf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjdfwulqt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnjijhyhs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdkwtmlpj.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gnsustnhw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtcueszkw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gtovmblqg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gweegviiw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfbzhwpsw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gsokbclit.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/guojsnkuv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnvjutwrf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gqqfuodrr.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gssmljvto.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gdhndjcyj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/giajcysro.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gykulmnpu.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gfpscwmbm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gzboyqugv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gudtrpmvj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gwhnuebmh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gunbmpdsz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxlozgevc.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gpjttwbcg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzoizowam.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gdyjnjoge.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gccinmkpe.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/ggqfpxmuw.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gbkrtfgfw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gywtauiyb.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gcalirigl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gkxbwhlps.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gligxhqdx.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvxvydbyh.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gsjrfzxdn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gggltsylq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gajbxfhja.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gswefuenc.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/glzrsgvmv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gmpxbljpu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gahwawsqr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gfplpbxmd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfshswsqf.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gyszgyhdx.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gaftkquvs.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gzfprvavg.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gokqekvkz.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gulcgcjjo.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gnffxyhin.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gygjktbtn.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gjbposwwy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gtpywelqn.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gawfjxtfm.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gprjesxgj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/guikcxpjt.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gxyioqsax.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gzvptksha.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/ghngrnuhi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ghtuywviy.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/ggqfppvmj.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gjptwvmcy.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/ggjgxsors.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/ggtptgewn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gqxdosmxo.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gjybbyrvr.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzoxmbhid.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gaqbywnno.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gwcbfjbtb.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gedvuybwe.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gygslgypq.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/goowhcwbh.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gzclbngyp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gnskubgei.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/glstlsfah.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvheztdpa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gaeswfygp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gdkoqlofo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gjngtazjz.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gxnwslrtr.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gbosjwuag.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gjyvyzdgx.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gocteyhop.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gnsymwvaq.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/ghblobhga.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gaflwzvft.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/ggjbgvmxv.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gsorcitoj.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gnqybikpn.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gkjuydsce.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gbytwgkkv.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/ggepwaqje.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gixupslss.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/ggsbdhdow.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/grtahqlkn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gojbqpgok.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gsbzloqrq.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gawpfedze.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gjmjqovmc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/ggmhqiiij.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gwdjvsbfl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gghgqmoca.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gffarddmi.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzyfbaimf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gbhahmscx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gsjmrvnkc.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gxqhekdze.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gztwlgihe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gbqdarwvd.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gqnjbchym.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gpchfppcg.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gadkadkcc.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gemcavikm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gardblfrh.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gqudlrwnd.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gaxvuphkp.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gtdgumxza.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/glwbuwngp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gypxgdylg.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gbvgxibaj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guygfmlde.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxslhyhis.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gfsnkunuf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gejlwagya.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gglsaqefr.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gpxkliopt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gjgvqxnmv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/grsfdafmw.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gnpqrtqnc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gpjewutsq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpwecsxmw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gxgastlze.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gwqpreozz.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gcxxgoxen.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnaddhait.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gldyztsis.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzvgrqjro.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gafxdkgjx.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/grtqaaryt.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gioavifky.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gznddzpzi.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/giwnbzmah.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/goeeteafk.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/ghmdxybzb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/grtyasugq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/ghklxnbhe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/grtzwqzmr.sHtML


<!-- 参考信息 -->