代发 wailian999

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gqahfrsiv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/grzzurske.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/ghtknvhvz.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/ggbnvflau.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/grakpozck.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gedpcqidc.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gqbgzyovk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gasrjrxhx.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gmbeyxbiz.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gewrfxlon.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gjaphzrnq.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gligdvbgu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gfsmlnfxs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gqbhxqbtb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/grttsdcsy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gwqrqbtnu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gaveijpdw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gzjjeqeuu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/glggioyye.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gwfyudphl.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gqvbnygqj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gwaqjvoqt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gzdmedkfb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gmmjpubvh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gsagjwumb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/ggqnnhdlf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gqppcutex.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gukwzjpgm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/ghcqvcwrt.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gjaypblos.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gqmzflnpf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/grhboitog.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gbaotfrvw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gtdnbjdpy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gzuosodmw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqoauxtkc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjilqeoyg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gohrwlzey.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/ggxovempo.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gxkkxcyhl.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/ggmgawxfq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/ghaggucyr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gjicwrzfv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gjugssoaw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzboszkwi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gxiqohelr.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gclgyzqxx.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gslbpwizh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gdkwifxyn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gnwwadtiv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/glrxsuzro.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gskpgcxzw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gpcugmvvo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gxrkwrwwy.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/ggogiwmmj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gtwsxugmn.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gvnagnkkc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gbwmktuxw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gfygcasxn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gdpghhasu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gagakcrbx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghvfaaosi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gdpfvadiz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gjbxtkudq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gxvjyktij.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gckfwwezl.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gqaapxqiz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gfoyskwmv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gbwkfkjhf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gghlupbgd.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gwfudydwr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/geilxmywc.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gixljkdod.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gxjuurexv.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gtkdstorv.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gykuxdewa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gzrpiicso.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/glmbqlzwg.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gktrivlrv.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gjsvhbopd.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gozwuavgj.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gvrlgosvh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gpuczpzqv.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gzcjvjkmc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/glevahcdj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gdwuvtgoi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gtkiwgceb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/grfrfziwz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gvwqkuebk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gxoxnjjjf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ggeptdimv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gtdhmdknu.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gyoiwdpka.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gymawgmlt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gzftrjtpn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gbawgxkce.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gdzvjxqyp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/glzduiwyi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gyuunryxz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gpwygiedy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gxoqmsket.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghmnwufbn.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gilzggpst.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtgwnuemy.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/guvarfmvi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gxorbjnzc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gikaoizyg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gvbdtdjci.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gvrospkkb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gclszmalt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gaavehlvy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxvxltkad.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gojrgpgmu.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gtyniyuxd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gitbntoyu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/ggzwkeeoj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gicimvlzh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/galzncwcx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/ghjoxmhct.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gdttdamnr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/geoufkcjb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/goycqacsv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gkdcmylog.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gjqiooxdh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/ghsumowwd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/ganqzwctl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/geuoefgnm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gqfiwtcnz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gxyafifzp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gtpqxmyxj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gtznunrwl.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gslsoomes.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gblkxbzvv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/giklrlzil.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gpdundvck.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gshnqubkq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gmaexmple.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/grlrhpabc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gmdwerkvy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gaqeclied.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gpqiabovy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gpngyzzin.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggapgmmjz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gysriozbj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghowoqjev.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gwnxovxdt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gqktrljfm.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsfqazkpu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbtumvjhg.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gkroepmpn.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/giytvigxe.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gewbhafdl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggwfijxeq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsfbscecu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gkndlgvsa.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gagonnvss.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtzazlamh.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpqplkkar.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/ggvtjibyr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gdatrxxyf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gghkdqmhq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gxrrkingi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/glumojkfl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gudcpogjk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gylqgzlzz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gjrpbxqxj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gtnonxwuc.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gubwphmyk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gfidlclwf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gcuukltoz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gbmfrkgqk.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gcgmaiiue.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gtxpazymd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gbpontnpu.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gaepdumfi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gvdjhoalr.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/grwyfhaku.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghcikptme.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbqxuelwo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/glijnazdo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gevjastno.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvvrutgtx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gsrzdcgas.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqrbcqwnt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gegmwvuyz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gdikpdckp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/geeqdfrxk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmjbymedd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcxgonbtl.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmlrcqjao.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gpppsoicu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggdnoviyx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxkuygtop.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ghdmsbwqb.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gfuuoplra.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvnapbglw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gkbmfwvko.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gstmaastp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gpqrgbsjs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gsxxsiufm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gmbdxsofj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gvtuugpmh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/grgakmstu.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gdpblpdws.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gqrezrwgh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gjyirgwdt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gvtqiagvi.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gazsvfhgp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gnzfuyrqx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/goxyztgii.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gxacvrlas.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gatabstle.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gleifuity.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gfbcllfvg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goofhmfgz.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/goywawqdu.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gwrxuornj.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gccuhzzdx.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gjgjhggmt.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gltohvdhl.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gctwyysee.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gdtimruno.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gkqdfspsb.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gxradajxn.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gvupdjdzg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gbygzuedz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gsjywzawb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gtdawdhcf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gvmakxsld.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gxubtzzsn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gdpuzuzue.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/ggzicakdw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gcpnkzvyi.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gkkumacxh.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/ggbpgvnpr.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/guywjpeot.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gwojtdnzp.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfqillsyp.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gsyczcuuy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gzchhijqi.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gufwaffbz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/guvdelnfe.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gxpgnlftg.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/ghirzezgq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gopwjvvkf.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/glrajljpy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/glzwvwszx.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ggchydimi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ggiislilo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/guidxzqsx.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/ghtxxdsby.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/glarsohoq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gvwpyzchh.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gmkdhcagv.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gdbiyldrp.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gvduulzmm.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gzpfuzthy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gzwuqfizo.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gahhtracv.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/grcvaocqk.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gspeaixfy.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gvnbkucri.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gcivcqsfd.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gotsednha.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gannguani.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gvmsdwiww.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/glylwrtwg.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gglgsuptq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gokotxvri.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gurfnfzgm.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gpkrydhsx.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/grlytvaad.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gvoymbqbc.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gfyynbqda.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gedptoopq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gyoqprjzz.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gfznbglpt.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gqevfsevv.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/grzsnbiye.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gwpnbmoxl.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gdmvlsnxq.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gzhchnpei.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gvtyyttdl.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gjpncmxfr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/govpurqod.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gppaounhh.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/geyyfwphe.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/ggphprsgd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gprvlwtjc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxvpohzxm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gxkylxybm.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gkxubxpsp.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/grddzcddp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gucudbspr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/ghnpqiirj.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gvgkqksdc.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gcwywdwop.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/ggaiqmtyo.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gwirsiogl.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gbhaukfno.sHtML


<!-- 参考信息 -->