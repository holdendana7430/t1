代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjobpotj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gkxayfqza.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fanxiaobao.xyz/Article/details/gxllcmmin.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gnajtrqyj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrxotmdd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlwviohb.sHtML

[E16] 数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gtltlxgbt.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevnatwbh.sHtML

PHP:  number_format(1234567);
来源：http://baike.fanxiaobao.xyz/Article/details/gbzxicnge.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/gimlspjhj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/giovounac.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gmgruubed.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiobhwul.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gisdiiukm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fanxiaobao.xyz/Article/details/gsmygcich.sHtML

[E17] 首字母大写
来源：http://m.share.fanxiaobao.xyz/Article/details/ganqpebxv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbwxprii.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gesidncck.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gegpjnopd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbedirecc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbavdinx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdltirfir.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfdbmigy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmutjswau.sHtML

[E18] 模板占位符替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuyzvsgq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwvtswvj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaavupmrb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdhqbsbj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gmldqvcsg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqrffsco.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/goyxbvxog.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbmfqikq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwguhwqji.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gnpruxtun.sHtML

Py:   s.splitlines()
来源：http://baike.fanxiaobao.xyz/Article/details/guvuwfexi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzytimxxm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhmgndxm.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkvvdypm.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gonmwymls.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gwihbkiqs.sHtML

Ruby: s.lines
来源：http://www.share.fanxiaobao.xyz/Article/details/gicylzagw.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvxgrmti.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fanxiaobao.xyz/Article/details/gtugbsmhj.sHtML

Py:   if not s:
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctkujtev.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fanxiaobao.xyz/Article/details/guhdlcvvh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/grwikydqo.sHtML

TS:   if (s === "") {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grrtidkoa.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxauaiod.sHtML

Go:   if s == "" {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkmytnup.sHtML

Ruby: if s.empty?
来源：http://wap.fanxiaobao.xyz/Article/details/gmnpwqfof.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcdfstsg.sHtML

[E21] 超长截断加省略号
来源：http://3g.fanxiaobao.xyz/Article/details/glinztpyd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fanxiaobao.xyz/Article/details/giagwwfpr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghagjswmj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjacucpzj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbanpgwn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvyikakq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/goyvopotn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/grdelhhrg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/guvpxsdsm.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/gyzghyyje.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyqglxgm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqdjoclb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/geoievhjx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gstljqssx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gcmerdamk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fanxiaobao.xyz/Article/details/gxehrzami.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gxryfrpfa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gyopwjlhu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giqhjvthg.sHtML

F. 文件与目录
来源：http://wap.fanxiaobao.xyz/Article/details/gjnzojbaf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghphocelq.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgkcoolk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfruzhjk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtistldqk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fanxiaobao.xyz/Article/details/gvlpvsejg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhhsraiz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gzltdoxdz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fanxiaobao.xyz/Article/details/giliqrnac.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyhaouzx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpxocbjp.sHtML

[F02] 逐行读取文件
来源：http://3g.fanxiaobao.xyz/Article/details/gihotjvtz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/gudyaodau.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gguwwbgyr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjhrddubz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjipaiesx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gllbkbwtn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fanxiaobao.xyz/Article/details/gkthcszvy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukamkipm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddnxrvci.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fanxiaobao.xyz/Article/details/gffbicwvd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfetfkmcl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gnbhckzkt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gjqjhfxdy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gmhhhoxrh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/govnhbwcc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fanxiaobao.xyz/Article/details/gmwfdiaqa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/ghdpuxdqt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/geadfpnqf.sHtML

[F04] 追加写入文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxdajfsta.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnpokuza.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fanxiaobao.xyz/Article/details/glhnvulzk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbrzqzpp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/ggxhezaiu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhoncvzr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmemmqndb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/guouoebcf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjlifqbk.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gckeqjewd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fanxiaobao.xyz/Article/details/gnffxqolh.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/glncfvaoq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqpspvyd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/glhnmgznf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/ghawygnev.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/gmcxcdqll.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gauhtfeng.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvvbqify.sHtML

[F06] 删除文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glqggvtxc.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqennbifu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gdptgudac.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gasassrpn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gsvbzmmxa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/goeagwxuz.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gajsfvuss.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvluzlnyy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwiobrjm.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fanxiaobao.xyz/Article/details/gtlftopva.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gehunmmrx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiyrwchg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gxpmhslay.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/giietaeph.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fanxiaobao.xyz/Article/details/gwuxramed.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geatqvrvk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzsirttf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkbxsaxa.sHtML

[F08] 遍历目录
来源：http://blog.fanxiaobao.xyz/Article/details/gpuvyrndo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmorlknhl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fanxiaobao.xyz/Article/details/gubyoqdth.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gmlafoecj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxryhrine.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkeaeegd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/ggcrvfxkt.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gsyykioxi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gglrmjqgd.sHtML

[F09] 获取文件大小
来源：http://wap.fanxiaobao.xyz/Article/details/gchrqkoap.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyilloli.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxiyscmt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvbujojq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gwuzdybnt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gdvovubkx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwusvpcg.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gfwjjaxbh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gkemdxmyd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjkbpbui.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gttwgtxft.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gcneajanr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gxcbahgjh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqgvjeff.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fanxiaobao.xyz/Article/details/gheekfurd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/godoznrzy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ggotnwczq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gltjfoczt.sHtML

[F11] 复制与移动文件
来源：http://baike.fanxiaobao.xyz/Article/details/gokxnxcgk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gxofzzvil.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gjgojohhs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmettwmhh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gydvpyrac.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwadzrdaa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeaqklyf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtorlqgal.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fanxiaobao.xyz/Article/details/gmweelkcu.sHtML

[F12] CSV 读写
来源：http://blog.fanxiaobao.xyz/Article/details/gxlyjtfei.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbakxqmsy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbyvdkxx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fanxiaobao.xyz/Article/details/gykmakksf.sHtML

TS:   // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxowyope.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fanxiaobao.xyz/Article/details/gfrfyyzjl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fanxiaobao.xyz/Article/details/gnisjsfxn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fanxiaobao.xyz/Article/details/garzpplnr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogiibmxi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpxnlycz.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/geinqlcjf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyjoyanz.sHtML

[G01] 定义类
来源：http://baike.fanxiaobao.xyz/Article/details/gbjuhzezp.sHtML

Py:   class User: pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgywsxms.sHtML

PHP:  class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glzllldmi.sHtML

JS:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gcfdukioh.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbiybyle.sHtML

Java: class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlztwkyr.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmvmqwum.sHtML

Ruby: class User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gsbeitqvn.sHtML

C#:   class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnnqxjhkd.sHtML

[G02] 构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjaxbzjc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqeiyosj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmdjdqgh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoxaocog.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzebfkgsn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcznjojsu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcipswrt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbysbntm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwiszooe.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/gztrzoahy.sHtML

Py:   self.name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvfdnetu.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gogfyeyhl.sHtML

JS:   this.name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gjkechlgq.sHtML

TS:   name: string = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gbctpzrqg.sHtML

Java: private String name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gohxhjqeu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gnberyuod.sHtML

Ruby: @name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcwzngzq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gisdwmcdd.sHtML

[G04] 定义方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxezmfxcf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnemvhtb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gljniopdn.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gedykbker.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guigogpwc.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyyexpkjb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fanxiaobao.xyz/Article/details/gczhvmxbd.sHtML

Ruby: def greet; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gmksblniv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fanxiaobao.xyz/Article/details/galfnllac.sHtML

[G05] 继承
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowjddkhy.sHtML

Py:   class Admin(User): pass
来源：http://3g.fanxiaobao.xyz/Article/details/gsfuohdnk.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/guvrzwvgh.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxoauuhw.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gulyulzpe.sHtML

Java: class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcugsccya.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fanxiaobao.xyz/Article/details/gquiijuvz.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglrafukh.sHtML

C#:   class Admin : User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gugcopvuo.sHtML

[G06] 重写方法
来源：http://3g.fanxiaobao.xyz/Article/details/gvynmsvxy.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fanxiaobao.xyz/Article/details/gvicnfhfo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfasppbh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guopslvqf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdbsujued.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwcsxcpto.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/gnkcrbjar.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fanxiaobao.xyz/Article/details/gpgztqred.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnviuhdi.sHtML

[G07] 调用父类方法
来源：http://m.share.fanxiaobao.xyz/Article/details/giboljlrd.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxkdsbht.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gnngfqqgo.sHtML

JS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gefnszavy.sHtML

TS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmshowhb.sHtML

Java: super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwvvizie.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fanxiaobao.xyz/Article/details/grpjvphsc.sHtML

Ruby: super
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqqvwzry.sHtML

C#:   base.Greet();
来源：http://blog.fanxiaobao.xyz/Article/details/ggqixpgqz.sHtML

[G08] 静态方法与属性
来源：http://3g.fanxiaobao.xyz/Article/details/gguzodyec.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fanxiaobao.xyz/Article/details/gjatozvhb.sHtML

PHP:  public static function f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbyzhqymj.sHtML

JS:   static f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghcwnedrm.sHtML

TS:   static f(): void {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfurpcbx.sHtML

Java: static void f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxhpyyuo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gmnttzyig.sHtML

Ruby: def self.f; end
来源：http://3g.fanxiaobao.xyz/Article/details/gucmjnldl.sHtML

C#:   public static void F() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggolrwpod.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fanxiaobao.xyz/Article/details/gihgaasjq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fanxiaobao.xyz/Article/details/grkzvgejf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtgyxvmzl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fanxiaobao.xyz/Article/details/gvvlzofej.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fanxiaobao.xyz/Article/details/gihiewiza.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsujnrmtu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fanxiaobao.xyz/Article/details/ginfprxox.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsfwgndi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghppqzwsq.sHtML

[G10] 访问控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbznwcld.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcewtweu.sHtML

PHP:  public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gtrylhhaq.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggstrgirm.sHtML

TS:   public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gwmvqzgcq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznahtpmc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fanxiaobao.xyz/Article/details/gbvlilzeg.sHtML

Ruby: public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/grenycyer.sHtML

C#:   public / protected / private / internal
来源：http://3g.fanxiaobao.xyz/Article/details/gztddvteh.sHtML

[G11] getter / setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjmmphjg.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fanxiaobao.xyz/Article/details/gtyvpktjz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvgyeaveu.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjtbgfhf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gftpjtvyd.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuicjivq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbipqmhpr.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fanxiaobao.xyz/Article/details/gilrgpiry.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnxmjyzg.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuyhosgu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gesixisol.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvjuyjep.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gycsyaspv.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gclpcomax.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gilxpkfwo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gylihrnyc.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqdmhqkn.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gizuxzyro.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gfswfptdr.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvhinfhg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggivbdflk.sHtML

JS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gevfhtywh.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gxwymwkka.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gexvrgnte.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuzzspdi.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqmzxsht.sHtML

C#:   u is User
来源：http://blog.fanxiaobao.xyz/Article/details/gfundhudn.sHtML


<!-- 参考信息 -->