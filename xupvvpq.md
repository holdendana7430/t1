代发 wailian999

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gmujmnttp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gqaishskl.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/goqzipquc.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gxelwwaao.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gcugbxolp.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/glirnutjs.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gmcxgspfc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/guicbahku.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/groiofoda.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gzflkqlps.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/ggzmrcgjl.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gikdthxyt.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gamfycwgo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gnxkdczbp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/godndkodq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gybqniwdc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gyaowprhq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzxcoylns.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gmmocfgod.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gphvvnkyr.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gpuqwstyh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gzgplwfrm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gamgambhe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gdgnzjdha.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmildplri.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gnwpkotlq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gdhpczufs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/girdrwrtj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ghmineyza.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gxpiaijiu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gesrhlgfa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gdcehlopo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/grmemusvi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gmayomxdd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gicictdrd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gftuvsaes.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gprktwqwn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gwbkpoidr.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gpwuxrbfd.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gjhsqzybc.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gnhyoaoma.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gzkctrsqr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gxpltqkvo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gknkbgusm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gvcxuprab.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtvleuzwr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gjccequgy.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gxupdzqwl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/goxmvtcei.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gkfymzpie.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gkamxejwu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gyvtzeuec.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gxwnihyra.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gyklksnub.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gsgrrnzsw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gatwpdljh.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gxzrbeqsl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gcojmqpru.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gpdhpxygo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gqtbpdyqf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gywhfcsgi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gvjywwsex.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gaovgjgbj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gdfpphyzu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdrckyfqj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gngxqpbtv.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/grefaodeo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gjbvgvnfo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gsnimahal.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gwrbfjnjt.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gpocxfhak.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gjqqxaute.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gixryeacv.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gcngdiumh.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gyzmynxng.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gxignxhme.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gzwdnlgxg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvjujfctj.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/glrmwkitv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gckrvezap.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gdacqzpml.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gdiypwlmm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gbkmshuag.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gjjqcfeor.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gewgavjin.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/goszpullf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gtdpurrnm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gukyuhcuu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/ghfnqioqp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gcndnppwq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/glhqsnsiu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gwsacgjyl.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/giaycdrmm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gvqythcpk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glnepbjxg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gcqfbkoki.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gsopdnqso.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gajnhndrs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gwsldzvbd.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gubetssjw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gjrzxnyis.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gylfkfqre.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gyktxoskb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaqcirrpb.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/godkzjzcp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gsenbvurw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbeyswvil.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gyrahwzvw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/guaxjynli.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gkzdqexpu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gcczlpsji.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxinkaukv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfpzcoazi.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gewoacweh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gjnukrweh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gwrjlavow.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/glooesvkh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gzrqusfhf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/grvzcetaf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gxywcmfjq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gczhffyty.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gzwlbrnwu.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gzxjfaroa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gjesarubq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gooymlvir.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gohikknmz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/ghughwyqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gqxfhtsvj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gxscvtvjp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gkyoezttr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gkwwfrblq.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gbmjxgrgu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gkzzkrgql.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gwfpmublq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gkhocubub.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/glugqfein.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/geihcpwtm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gaurnepss.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gqmxxssth.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gzjglokqb.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/graeagxoy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/giaojztbo.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gljqjznzz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gamtpbnna.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdkhxhvkk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gihnclvej.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gxppvpwkc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/geryxfsgq.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gviwyuczy.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gbtofqeiy.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdqywmvkf.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmedhhiup.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gizzvyqjf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glpmhcemd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gvtjtjoxg.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpnxntnrt.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gabmeevgn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grufaptzg.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gyeptxswg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/guavxuxux.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gzwtihant.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gunmohvku.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gpwbnxrdz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gppxlnscl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/guyngoevn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gyptgotjk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/ggatcwfsd.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gejvairlg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gczwitdpx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gpxtknjsg.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gvrfskrws.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/ghzuhwypy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gnnwqaqvx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdjrcfhuy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gmmghhqjr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gqjswzkei.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/ggousirtx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvviuckcw.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzayqrlgw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/glpprbcuk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gmblfapsz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/geezpjkgx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gjhxlrprk.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/giffrsjwl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gdwhpsxjr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gxoejqeiv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/giedjrosn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gouvwtiyt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gidihprwm.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqlbvfiut.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gmkvaasrr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkfnaycmx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gtbdeqwvi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gisjfjtwr.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gfkwxqdie.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gckcjusct.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcgaracwx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvavdejpv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/glsvyuiwb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/geqrnrqkc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gwoximaea.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjyivqmqs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gnvcebbbo.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gcsnfephc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gmjdzorcz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gchxookap.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/ghvxipsgo.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gihwklijw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gwfhzbsok.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/ggluwxnns.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gjqrwouom.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/guwlsusku.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvdnccerv.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gvniooppz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvsyokkev.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gdyyofjut.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gokekcbri.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/giqkhsqih.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/glvqckfin.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gygqpbqgu.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gamhyniyc.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gvqspdxar.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gbxfwtzbc.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gaftuyjuk.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcdmskroh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/ggnkacgkn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gqibhbkhm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gfvszfqad.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gddwyugpp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gjhikbnlq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/ggolaysbp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gcniyhojq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gycvbuucs.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gevpdatpm.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gazdiioux.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gmeyozujf.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gncnxfjsp.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/guwtjzxqb.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gmcivkucc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/glntziyhp.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gqvhrukcs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gfzzwccyp.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/glalmvtza.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gjihypqnx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gwoudwxxj.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gjstyyoxb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gbjhltcir.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gcomxmgal.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gkupscqat.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gifbrgzmp.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gqnmdlblb.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gsjuxrbus.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gzbyaahak.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/goumqpcdf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gffpmuihq.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gzhbdtlsq.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gjqzwjvnf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gfgnzetkb.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/guxifnyze.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/glttzflwe.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/grtunuqzl.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/geexxamkw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/glkbjtkou.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ggmamfubm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gknuydevp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gepyyngqe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gcuhsxxiz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/grjcjapbz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gjgpoetwy.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gxvvxxeuo.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gqixcmose.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gvinokimo.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/glapffqxy.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/grgmxhgvt.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gkigzhvlg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gkoysigan.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/ghariztiv.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gukmnulfs.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gtqwbcaxi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gqtoprtmw.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/giqkxbtmo.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gnumeghwf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gwnmvwzdd.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/ggnkhvcds.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/grjatcppc.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gxyvoxzvy.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkmkeprfy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gahqffdqp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gikqqscvj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gstgztjca.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gqxneipkd.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gyvvdsoyc.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gjandedou.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gjenmcpqt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gkqazrxvy.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gxiabhfhq.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gmgdxhrsp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/geilohpma.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gbnqjqdis.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gtwmdubbq.sHtML


<!-- 参考信息 -->