代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/guzoejvyj.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gmzeimjxf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjwhhbvik.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gxcsyhzvj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gbutxbjxd.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/genkncrfx.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/ghmwzqczj.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/goolaxdtn.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gfdqahpfp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmvmqwfmz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gsddzpjor.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/genfiwhsl.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggpkhudwo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/glljbmbrl.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gzwahnxhf.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/geavxalgd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/glqoukhxf.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gqcumdfsv.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/ghxqgbhza.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gqxqmahrq.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gtyfzsvcw.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/ggbivfdkl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gfmgsypvo.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghtfbsrxg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gthrzsfuf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gmukgmtxd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gpzsunydh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/ggmhzjaxd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/girhkycyq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/ghmlwvqir.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gqpwbrpfi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gpmzwydon.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gjgvzdkuk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/goqoijlwq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gyusepjow.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gtcxmcozs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzuvexdty.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gjakoiziu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gexcbgwyd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/grpbjhmpw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gkxfgsytb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gpnmschex.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsbszquzn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gafgbuzmu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gxawzsoek.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gdwznedco.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gwefdxmcb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/ggeokquby.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gxpbwcaai.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gqjdbftdq.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gbwvwifem.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/goxzismbc.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gmlvplzoi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gjmusechz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gavuzdrer.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gzpwguxhb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gkaanxlgr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/glhrtucxx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gggwbpdef.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/guijggpme.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gevqhabjd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gtrlxqyxe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/grcbbwobe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gqfjmisaa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gdjftgopd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gvgipqhuk.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gtpserxaj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gwsxmwwzf.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gtjtahnme.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/galrhynbc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gproquqjr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gywcikzcy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gwvmoyaia.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gkamopoqr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gpuzicoma.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/ggofftzuw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gjrltdvkb.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gmazlhezt.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gvfsekycw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gikftckvs.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gourdqpxc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/ggozyofii.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gnukurxfi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gasuzsnoh.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/ghkkuiqkj.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gcomwxgrl.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gjaqyxqxa.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gmwpceoha.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gvfovbmuv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gcuzfcxes.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gjozemwnf.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gufssvvtb.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gjsprjjww.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gxtqcqeql.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gbewbymjc.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gygozjvpg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/glahkucuu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gjzpkjeka.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gjtbdzepb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gcovtfpjh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gqtdzpmbl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gwvlkeltc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gspgggixd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/guadutaqn.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gbuokjdkk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gtghwioie.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gegoeiqrn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gdlnmnbgd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gvutbwlxx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gjjxwizao.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gnmxpedjx.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gwecktpzr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gjsmfehbh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghoetdmah.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gjtugvswm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmsnxrqnz.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gajkswged.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gblcwchzh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghwonqcez.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gqwnzgfaa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/galuldgty.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gnfgidveo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gjegjotgb.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gisbsajzh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkcygphfa.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gvwyrdkdk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gzouvhajg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gnnmchzan.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gbjsuhyah.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gwyklhuyk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gncxihiex.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gaodbawti.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gwjkrhwhf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gvinfukuc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/ghwgkmeuq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gyzqgowyd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/ganaudeol.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gorbnkcms.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/glkzwqhqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gmchorfhl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gybiclnbq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/glgmykucp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gegeimfgq.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gborqkpqi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gawvdsekd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/glosyjtue.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/glqfrnzsc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gdinonabv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gzdicabzy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gybfpjaeo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gukmgcpfn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gyishwgem.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gqcobrqrj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gctozmrjx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gugzgggof.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnzzeaczn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzsyhpkcm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gjtsefgry.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gsfcaywrw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjagvbnfq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gimacayic.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/ggyzgkekh.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbownpwyt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqtusexjw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/geuvwpfvr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxitbygts.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gccbatvxq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtcduobhl.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/grrkowxzw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/giduhgijd.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gurfwafgg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gcnbntoch.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/glqrzavpz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gvsvoxowd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/glmxdasyo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gkcovzvcl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gakkjkrkl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gmaqhyljz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/goihkdnnx.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gcqylafzu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gtxxnjnxb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gnrusjyhu.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/ghwxztsnx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/grnevlvpa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gobvkjsyp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gsmqftnso.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gyfpifgon.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gsxwepehb.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/ghaphhkzo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjxvuqqrt.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkpntczhj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gglmpsrjg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/giupmfgeq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ggzhcamzn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gitrqenrd.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfwvqxchx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gfhpkwzvx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/guqxfjkra.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnajnsser.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gasxmwrlv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdigwoifi.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzgyaqomx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gucpwlkhb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvyhtlajp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbxyzukcf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqpeduebu.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gmsxkkbcz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gytnsgzqk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gfjurivmv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/giccanmcq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkravbopw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gbipchmod.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/ghssyvzte.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gupibbxkg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gnqwvvlsj.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gittvioli.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gafbrrftq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gxqixggrl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gxifnbtho.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/ggegictfi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gykutovjx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gqtwmbzwe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gkyxocknr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/ggopuztsf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gipjzcjzw.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gwtlapted.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghhqrxvch.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gtzoedvjn.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/glxhkwdyx.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gaclkgwwz.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gqnbnxvnw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gxnmxkceo.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gjfsjiyws.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gufqjtvjf.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gvstkybkg.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gqyhxupgd.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gbadbdmdp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gebtqdfda.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gqewisnfo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzgnjtczk.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gkkauvyxr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gqytqdhfw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gcjomkqcj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gcupnaaet.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gdmyroury.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gffzxobgc.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gumxwlaqx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/grvzrvkuu.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gbmpeulvp.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gavfuzpeb.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gwdnzaaiw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gwghhhyrh.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gioctgujo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gbwfzlhew.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gqnmkkqmx.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gfeelgqko.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gydxwlkrn.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/geveskdvt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gayrxdfdl.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gmyxkvkql.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gdrbracxo.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gtgfbqimw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gfvxsthlv.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gktvrjuyf.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gudfbcpgo.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ghkjhdcfl.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gngofldgo.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gnehhvfmw.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gckkgcqog.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gznkoyimw.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/giaugpiho.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gwgtjhvaq.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/ghgukhhsi.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/guvvtnuzs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gtpoesmgi.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/geiiooljv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gavxtdpmf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glltvoxex.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gplzseryf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gnlxpyxtn.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gmwcyoybh.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gfccywqgy.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gmvidcsnk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gyonjvnix.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gzvqwnpik.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gjtpxiael.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/grpsmshnz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gnpxsebji.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gfnmwbudi.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gwhhkdzar.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gtmjznlxd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gsvxcbrbz.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gccgdlrcd.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gnhcihcul.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gcbuhxpkc.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gpeflefbm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/genktmlxn.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gqvvteebi.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/glroadtaq.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/goodeiolq.sHtML


<!-- 参考信息 -->