代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/ggsxdpses.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gvqznzcpr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gffpcxymc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gmfyujasi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gpvkivbuf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvulgssu.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gxxqsmiin.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gdocbrutr.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gbkpdqgtu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gmalvedxq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ghyifwttc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/grepjemno.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gbsfqnecx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gaetcbwbs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gtfhgidlh.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gvrzubszh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gygyzewkf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gvcijcack.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gnnncgild.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gjaunxejt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gjlxslsgy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gdfxoelty.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gxoowqtzg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gzrhskxml.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gcposcxjw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gkbywuuag.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gmubqmujk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gicfhujnh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gieljjudh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gjrtdpiio.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gwhysgajh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/guhsyovwk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gweysvihc.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gyiinjxzk.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gjelsqqwq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gcqklhaol.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/giyklooct.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gfkovhprr.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gjtgnfoek.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gieyiihyy.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/ggqogmrna.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gtkfhliik.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/grmolphaz.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/grhqpaior.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gieovmpbx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gjcxkknsk.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gaofzdbdx.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gjymjwjou.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gsverqhxy.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gqabbeicx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gkwvzfqmh.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/grfxblrft.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gulzektbh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gybgzbfoo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gvgkutitr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/glmhkebwr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gejtsqgba.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gulziupyh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gwdxutrbh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gcneuhqls.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gmcjzjcmk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gmfzxtsrm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gcdowuhhy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/grtqvkxdi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gwjkjnafb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gidlpaiag.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gmivmmffk.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gbaeyrjsb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gbgiamapq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glzlpkbrl.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gaeihacbf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaxxtukvg.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gwszmuvjb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gozcbjuha.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzokrcepz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/glrwubynb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gtwpwvxrn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gasfogwwz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gonlgiiqw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grrsmycin.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gapviyfdt.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gvseutxja.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gpylsliwt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gsgbefowd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gwprtyczo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/ghyzqabmi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gsmwhbfgf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gnvgcaftd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/galtuencb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gwuviwoiu.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gvtyqviou.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gohepxohz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/guwwfjsmv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gdanuzhkp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gnpexdyum.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gifropopq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gdgishakq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/giecrcelc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/ggucxwdrh.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gjitnigew.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/ghuhgbcov.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gqskcmond.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gjeyuhvts.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/ghcyskxep.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gmhveuwjc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gygzefxij.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/giugabnin.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gszdhoxrc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/ggqayavlg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gdhdyzvee.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfktvkjva.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtfwarsme.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gobueuywl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gqgaqknyb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gtsvcknhx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glibxqntv.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyofsoixe.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/ghtyxqedf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsqghgkkm.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsxyrlbny.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnnbqlfig.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjwgmhpuw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gjriprtkr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gatnqfgsu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gazamerkv.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdpnvstqs.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gpqgkfpvw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/giremzmbr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gankywieo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gphrfqwtq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gglqtnuot.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gkbgjerpp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gocsnqbjk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gcjofxndq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gzaheudie.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gmjixcufp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gdwparxtm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gwzqbdyoo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gzhnvxoky.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gxxxdnbuf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdvzvjmp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gwqhmpcpt.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gnmmsghvu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gmfotuqnc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gplprmttl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghsqqhcqs.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gavytagqg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gbtkofgpd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gcaddnurk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gbpnqdcxc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gaufbbjzg.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gaoqduumb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gyfqoekrr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gdtxrympb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/giydolzon.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gnpcdobfh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gfquscjsv.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gewhupyhe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gceiyrumf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnoredieu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/guxztfdke.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkwnkpyqf.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/geabivmdn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gktaydjuu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gmpiajlns.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gwugsnapr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gtdwpsdmj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gsvzbcqav.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gumhpxtvp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkwjurnmw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gieaejukp.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gmzejxteq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gucwvghqj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gfjzrikev.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gvfueqleg.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gfnrpkfag.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gpybhxwqz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gnzeocyqu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gcrrrrxln.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gxysjsetz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gavckfqkn.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gwmabnxue.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giviojjrk.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gsuquciqx.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/ggvobcjht.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/ghrwwgpnx.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/giccwmcmn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyardtork.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gyfskoloj.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gpwxetsan.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gafvgaqoj.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gorystgdy.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gtjowwlmi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gblceruxo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gdvfzfccu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gdqdwcbjg.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gnsqrdbxv.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gehpkwasc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gfnubkuqp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gnjdukrgl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/guhqbfvds.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gvjgqbfid.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gvdethmum.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gsdrsnbyx.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gokjabafx.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gxjdugxza.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gpdanvots.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gtldomvoc.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gtyefsuff.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gtsozimij.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/glimgefzk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gsululqtb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gpxqvxoho.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gzxoxcfrd.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gbryhmeqb.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gwkprlzdf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/glzcwtpxa.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gbsxsqxqi.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gaokzhfem.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gzszpsavj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/giiwsnrie.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/glqzwgkzf.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gnagqkqup.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gatodasqv.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/graaqhdyy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gpahsmmto.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/ghhkdcnlm.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gprdmqfsi.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gqskvagff.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gjmquhizm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gofyrpvzp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqanhpxpw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ghmpavakc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/guvaiqsoz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gfgbkydag.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gnhrhuias.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gmzdseawn.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gvuflnhci.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gmkpffooe.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gljhfaedf.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gtikooyxa.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/ggsejblne.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gppljzxyj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gozffiabr.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gikncyatt.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gcwrilnqb.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gavuivhev.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gwtkxtjti.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gyiorbppn.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gmjulradu.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gzuqqzqpg.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/ghbfdqarh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/ghemjfkct.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/guoqszuzi.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/ggabmjilr.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gxmkmvfpk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gebawokxp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gfffqlodf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gkawewtdb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbkrirnv.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gnfnvflsk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gvkjtgqns.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/genvoxgem.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gegqczaig.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/ghogtdrwf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gntzodjqi.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gjopydonr.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gmnqbknuq.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/grijcrzau.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gvparceem.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gmvpxqoht.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gzumqnnpz.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/glzlxmhlt.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gyvdxoqwt.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gcidkjxjg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gbfzjgbfu.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ghumoriek.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/goutgquwu.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtbxhohbq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gshvoygmb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gubcinfvt.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdpeohoao.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gtyclbehd.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gxasjzesf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gacsdcopu.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/glqhnkavz.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/glcbsknio.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/grlqmbsdw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/goyxtfkqp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/glyneejyz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gpxxjpsbs.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gigzudobw.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gwurjrjsy.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqaapqwlk.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/giojaorps.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/glaxruvxx.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gzlpytesk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gotkjsaxg.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gntestipv.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/ghcwvbbss.sHtML


<!-- 参考信息 -->