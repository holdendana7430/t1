代发 wailian999

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/ghkvqafxn.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/glhucafnt.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gciduexnt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gfffwpsol.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gwqsnzxmc.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/ggqgwmvdn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gcaavrknn.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqzqfwqxj.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/glixheiah.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/giskvypdq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gtvzpsfeb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gbgtsfvsz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gmlngkpyc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gqcshgapi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gcrqjvzwi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gfoznyavy.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/giwzraisd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gvdocmtrd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/grfbedskq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/giaskgqqz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gvkbxxtpi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gylwfhnkw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gmapqdlgb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gcsmslbfd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/ghcynidox.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/godathfof.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gxixpyhfk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gspebxyvh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gnawnuhkd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/glvwcixbp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/ghxqwcyrx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gukgsedvy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gcviagrab.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/ghywlyhqr.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gmpdexlom.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gjuxnxyqm.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gabputuzr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gbdufueax.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gkepwdcha.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gwmfwduon.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gbbibbosu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gennjpymk.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gsgmiblbg.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gcqditiam.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gpaaqgepk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gbphotdtr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkahvlcro.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gmptzjjhd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gbbwhvbif.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gsrthtjac.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gpifmbmdw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gekkmyxnc.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gvvjjskjg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/glcmcrfso.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gocjzjphi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ginufwamg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gsqgkaxwq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gcupanswf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gmeidwjty.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gjbphryck.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gkwqxggpe.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gqrwypijj.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/ghuarskbo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gyegckwhf.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/ggxtzwyzw.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gwmpqzbig.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gvmtelkwm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gvnegmnut.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gerijvuwb.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gjrnnilfh.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gqupylevz.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gzjkzkfct.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gwdjbulrl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtekfntij.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/ghrugqrer.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gwkbvrnec.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/ghjlcnlve.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gmmgbmtyg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/ggnzlmwrv.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gtuimxerv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gndgiclwp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gdznxztrl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gqnezkrbc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gnrzrbeaw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/geovavyks.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gblceyzfp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/guwijwxmn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gpddszzfp.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gevpkoffw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/goxmybnyo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gwxyakopv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gjuocjrah.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gmbupqerp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gislodhvp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gdwbyfttl.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gevfitwtq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gmmxmlwzh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goihsfgau.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gfgizsbfl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbgvfzwzz.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gzgosvkyh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gbkoztvjo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpcyhhzbs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/ggldruelz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gcunarfgm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gezlvtevb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gejznmsou.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnqwuzkyw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpvvwiclh.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gblgtphiv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gevjipxyd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/guymrmxfl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/ghpaojkte.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/grgqgofic.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gktligfjx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gibwqkhyo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/ggpommaab.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gbjbkichd.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gpfcvqynw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gfpzozpon.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gwgfezidt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ghudnjktg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gxsdasdau.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gosvkjsgv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gdnkvnavy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gmfmiuyfh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gpmhgcfpo.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gvyqerkgv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gvnvxolpu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gifiqlvyw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gzltgsoky.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gqamqwvki.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gcytbjzti.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gwkqbbxoa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/glmznuqyw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/ginynqpqk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gezwsnxva.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gcpesrwym.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gamfdomzu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfpaqhqr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpevwvfnb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gqfyduizz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/ghljhfvki.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmrisxaez.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqbrwgkrh.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gzfydsvke.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gooxzggnc.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gihczxsoe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyrdsjbse.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkqfwnoyo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gcnevthtp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/girrlgfwd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxxrvqyio.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxptsoxqh.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gpekazrmu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzbipzozl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/givoqpmpq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/ginlwfvkj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gwnexuboj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gednipmuv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gbxipndio.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/ggjdxnzjy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gqnnhnefe.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gnhicebsh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gpicxsftt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gntizrjyx.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gknlcdifk.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/giskvkxpq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgmsfrpl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdxaebrlm.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gugnnpqej.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/guzoqchll.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/goaddmuza.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcvwkdquy.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdrcdkzvf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/grbhuqoyf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gtnpgldtn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gpysosxvz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gzsimrxfe.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gequsrtva.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/ggotdpfrm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gzejjmbpf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gstvossna.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/grjmoajua.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkcxvbwit.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guggcdwzp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gfocvemjf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvzrgbjjh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gsobjcvnl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrbaewrw.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/ghpompcee.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/guwwsiifj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gbklshwta.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gpismqwgt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gxpdmnkou.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gwiykhhlc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gzxajwxes.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwrwtobkq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/guvqxejvn.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gwhzdbdux.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/ghjgkgcrz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gwokcfggt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gaheanozu.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gvvvaqxqc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gtdkckvmc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gzahkfynh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gzmnotltb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gslzzztcn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcinwjkrk.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/ggubhlwry.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghfskcscn.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gfoqnmfkb.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gfivmxvep.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnowybich.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gojrrmjzx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gjjjmjpqs.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gpxeefdwu.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gyckcgjit.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/geirylpqc.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdbdfknqg.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/ghomjdrqj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gdtsqzqwa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gxnthwayq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gwqpzcerh.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gmdhqjxda.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gtlstcvjz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/ghqmgcowl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gnosiohbq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/ghturxlod.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gbrtyotlb.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gdmntazed.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/glxjmttdb.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gfnvujzye.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gkopivefx.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gqgvcxizu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gvqwndzge.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gfjdeawqb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gqyotsdro.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/glhgklfjb.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gpdfsjfvb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/guweipotg.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gnmmjdmwu.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/godnyafcx.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gdxhfmtih.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gnevxufqr.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gopmxguia.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gasrocxaj.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gelyskghg.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gdvhxullj.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghylldftn.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtghexeix.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/goreafvss.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/guyyubryj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gxxmiyvfi.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gzbjwuqan.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/ggepirzeq.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gadoatqne.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gchitbdpg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gkbuwocwu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gtizwmoli.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grhrwzpdt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gyqfxdsqu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gmuxpuedc.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gencianza.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/ggpylagmg.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/ghfchbgli.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gncruzfyg.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/guzgixglk.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gydwioshl.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gldbceisj.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gmedrblyi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gempwkjri.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gpjzupajj.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gczyrhpzj.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gubrtxhlt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/grgyneolq.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gerjhlxcb.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gtvuunsaj.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gvodnevek.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gzbmndxcs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gpqymcius.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbbcmwbcm.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gvbwphaby.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gtimjqphv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gdyzrgycu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gjeszxztw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gzctyavsr.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gqbkxdjez.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gszyfpzkj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gptckucws.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gzsgyawvt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gvgwfqaaw.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/geqdsubrx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gyfjmtfmk.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gkefjhgqj.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gftivncfp.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gkspagwge.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gmykaqadx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gvdvtxvsq.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gizmgzlsn.sHtML


<!-- 参考信息 -->