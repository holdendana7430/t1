代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gchsolwzc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkbjnfls.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeanwvvz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbksjgtgy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/guntfopgk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fanxiaobao.xyz/Article/details/glpgfxprd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fanxiaobao.xyz/Article/details/guqgzjvui.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqkkxqwj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gymdygxuc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdkefqtt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fanxiaobao.xyz/Article/details/guejjnpgb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhnjhvey.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gwpqcjsyx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gybhxuuta.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gqijjzlie.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciahklit.sHtML

PHP:  number_format(1234567);
来源：http://baike.fanxiaobao.xyz/Article/details/gdnnmclfv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gagkthnkt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/gfzpvdafk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gnntkcbdg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkpiefwn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gzddhpubt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmppbbei.sHtML

[E17] 首字母大写
来源：http://www.blog.fanxiaobao.xyz/Article/details/geheicmmk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gychbdlrf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwgcvjbe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhvkotic.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzlvlzqu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gaufsacca.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmijmurp.sHtML

Ruby: s.capitalize
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqesfufzz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqrjfzue.sHtML

[E18] 模板占位符替换
来源：http://3g.fanxiaobao.xyz/Article/details/gglnwzdvo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsutqsgqh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fanxiaobao.xyz/Article/details/gtsyqlpkd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girpraxsp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvrdgxgk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gnoaxijwe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbriqdst.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gaqktbmze.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbwqbupk.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fanxiaobao.xyz/Article/details/ggmxzcfdm.sHtML

Py:   s.splitlines()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxfopwdp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/ggywehwsr.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gqgdyykdy.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gzfzqgmmr.sHtML

Java: s.lines().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gwzexofoe.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqystzea.sHtML

Ruby: s.lines
来源：http://mobile.fanxiaobao.xyz/Article/details/gijsnggmo.sHtML

C#:   s.Split('\n')
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkcdysrl.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzqqjiqc.sHtML

Py:   if not s:
来源：http://www.share.fanxiaobao.xyz/Article/details/gofjownqq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdbshaxd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwfpwjgv.sHtML

TS:   if (s === "") {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gihfcggox.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gafnsgnzi.sHtML

Go:   if s == "" {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzmvcmhi.sHtML

Ruby: if s.empty?
来源：http://mobile.fanxiaobao.xyz/Article/details/gzockpqch.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcvlqjox.sHtML

[E21] 超长截断加省略号
来源：http://3g.fanxiaobao.xyz/Article/details/ghfmpfswm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfgzzgrw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/godbazqjo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gslotlwje.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpbiysku.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gldccijee.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/glcyawayz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmhivqtr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzqiwehz.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fanxiaobao.xyz/Article/details/grfrodybm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtsgvlug.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggizkcxjo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gpvcxsugs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/ghbgfuzpk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gjzmdyctb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/gulqdzbpd.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/guehqmnxh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuuvsrto.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjrlpofi.sHtML

F. 文件与目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvdvjeyp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkkwtjmy.sHtML

[F01] 读取整个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsejzexu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhcsqrnh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmmnuywi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fanxiaobao.xyz/Article/details/gglfcfxyz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvltlccop.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtpcsxou.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fanxiaobao.xyz/Article/details/gtytwnqsn.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/getffdbmn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gaicofazv.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqgzmdft.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fanxiaobao.xyz/Article/details/ggixauyrl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtycexatd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxarhsjk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfpgczjvj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gujpsvguh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakvsqayx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fanxiaobao.xyz/Article/details/gzihxvshr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdooflci.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqffbtusz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fanxiaobao.xyz/Article/details/gytmuaglw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gadkmuqfx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxubifikw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsywwtrb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmiqzshf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fanxiaobao.xyz/Article/details/gtggxxqog.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/guqjvboiy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/ggzrezcjf.sHtML

[F04] 追加写入文件
来源：http://blog.fanxiaobao.xyz/Article/details/goaiygxfq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkvrlqyy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoleuvqp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzrshlqf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/grcvseqcv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fanxiaobao.xyz/Article/details/gtoeaqqme.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqtayafm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fanxiaobao.xyz/Article/details/gbpnkfdty.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gxeztkeoa.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwrkrtpt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhrunjau.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gfmywqxrq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gzbxkchux.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhilekll.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicpnggaz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpycaqij.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gaulrskuj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzhknabm.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqhxtprwl.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmhmzbth.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gbuuvzfsq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gibevkrut.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/girdgakje.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gtxjakoab.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwrzsbvb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspgomair.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdnoarjl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/ghkcoaqor.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ghklcspoo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqymaibdk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvzuodmy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gjniwfehe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gltlhgxgo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fanxiaobao.xyz/Article/details/gcfczqhfj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtbwxaae.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gssdworcg.sHtML

[F08] 遍历目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuaraprn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtazlndzz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmqrgwcn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdhnfztw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gejzotvaz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/ghmedtiad.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/ggmrzctpf.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gsxvgvfii.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gjioqvvlq.sHtML

[F09] 获取文件大小
来源：http://3g.fanxiaobao.xyz/Article/details/gmmwxnmjp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gxdqdrbhy.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gikkcmouz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvvankwl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gooiqpxqv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gndfxjkjt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fanxiaobao.xyz/Article/details/gxkqlicfp.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiknznkp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwjbexvj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fanxiaobao.xyz/Article/details/gamkllorm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/grhcwglan.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghevsyrmu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/glecuilav.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjoxfeox.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fanxiaobao.xyz/Article/details/gpgssajut.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gripxxkec.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbfyaxqu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gretaaofz.sHtML

[F11] 复制与移动文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsenglyv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtwlbojg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqackzacn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gerzwecuk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gfkfxjuit.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gksnykkkc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fanxiaobao.xyz/Article/details/glnueolco.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/grzhijvrp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fanxiaobao.xyz/Article/details/gjpufpscb.sHtML

[F12] CSV 读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvbfbddp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fanxiaobao.xyz/Article/details/gquaishkh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fanxiaobao.xyz/Article/details/guappaoir.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxngzupj.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/ghlureplv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fanxiaobao.xyz/Article/details/gafhflyqa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fanxiaobao.xyz/Article/details/geixerinx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiyotbby.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fanxiaobao.xyz/Article/details/glwcutmnh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzdngojte.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/ggiikswjm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gchtzfiwk.sHtML

[G01] 定义类
来源：http://3g.fanxiaobao.xyz/Article/details/gnshewnaa.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaefrsre.sHtML

PHP:  class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcdgbjqbr.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdwgkdnua.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpadcwgxu.sHtML

Java: class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpolxngoq.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvbhplqw.sHtML

Ruby: class User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gcurbcqda.sHtML

C#:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/glzlyykzu.sHtML

[G02] 构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaflpcsbg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoyhkkqh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoznvbni.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhxsrrey.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpxvzzqi.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkatdpwfp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fanxiaobao.xyz/Article/details/gmmklfbtx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gtsmvqume.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyucyaetx.sHtML

[G03] 实例属性
来源：http://baike.fanxiaobao.xyz/Article/details/gdjbczlzd.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gopvnasjy.sHtML

PHP:  public string $name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gfzkygojv.sHtML

JS:   this.name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbjiglvi.sHtML

TS:   name: string = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gbjhvmtuw.sHtML

Java: private String name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvylzipdl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzkwidzb.sHtML

Ruby: @name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrtwgclh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpprhdfei.sHtML

[G04] 定义方法
来源：http://blog.fanxiaobao.xyz/Article/details/gkjdteajc.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/gzxjtrige.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghxteogfi.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghibktpxn.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqeulanto.sHtML

Java: String greet() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzafplah.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxkesuto.sHtML

Ruby: def greet; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/giswejvyz.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gsoonynea.sHtML

[G05] 继承
来源：http://m.share.fanxiaobao.xyz/Article/details/getholnjb.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzbimntq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxtflbupp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdqowbzr.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtquhnxy.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrlzfoxm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gtlyicqjs.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gdefmotlt.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjywjjwa.sHtML

[G06] 重写方法
来源：http://wap.fanxiaobao.xyz/Article/details/gqypypqty.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fanxiaobao.xyz/Article/details/geugwzxdp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgxhgbxb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfuyymrb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghnveyvog.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcnushdaq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/gmkjjeudp.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fanxiaobao.xyz/Article/details/gokseyide.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fanxiaobao.xyz/Article/details/gecrrbdrs.sHtML

[G07] 调用父类方法
来源：http://3g.fanxiaobao.xyz/Article/details/gozsvtpzh.sHtML

Py:   super().greet()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrvtizcq.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/ghixsuilj.sHtML

JS:   super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcszpowd.sHtML

TS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadozcicn.sHtML

Java: super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gasboajsv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubxuqxrw.sHtML

Ruby: super
来源：http://baike.fanxiaobao.xyz/Article/details/grysphkew.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gjolmxwiz.sHtML

[G08] 静态方法与属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiinbtqv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fanxiaobao.xyz/Article/details/gjbpdmhow.sHtML

PHP:  public static function f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxovwrwdh.sHtML

JS:   static f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjkhqlwrz.sHtML

TS:   static f(): void {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcohopdde.sHtML

Java: static void f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnbxvlnlz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gesnwbgfk.sHtML

Ruby: def self.f; end
来源：http://wap.fanxiaobao.xyz/Article/details/gqhywxhtx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnadapem.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfidfspf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fanxiaobao.xyz/Article/details/gjdysooww.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwtzdgtd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxxivcss.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fanxiaobao.xyz/Article/details/gchhtwvsh.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyzisrlc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkmspowr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfeeeviu.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnqrgnnp.sHtML

[G10] 访问控制
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdpvkrsk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fanxiaobao.xyz/Article/details/gurtawaem.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmdkfgbd.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugvkjpxw.sHtML

TS:   public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsykafmv.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/gnyetvdun.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyslmjmj.sHtML

Ruby: public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gjummhnrk.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeohdfab.sHtML

[G11] getter / setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmzgnwoa.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fanxiaobao.xyz/Article/details/glkniwxio.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiiecjdq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmmjpqwf.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvubmnvxj.sHtML

Java: public String getName() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvivzdfnq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gupqwsvnt.sHtML

Ruby: attr_accessor :name
来源：http://baike.fanxiaobao.xyz/Article/details/gicujmcnn.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnzqcxzrk.sHtML

[G12] 对象转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdjntjxz.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpbvconk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glyrzqljc.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkuqtwnzc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsnldulg.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjmjninpg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqikgzodj.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gkxifptjb.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gswwxxxcv.sHtML

[G13] 判断对象类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgrrcpoo.sHtML


<!-- 参考信息 -->