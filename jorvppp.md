代发 wailian999

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gnvykytnv.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/grzsgbfax.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gwzbhxgqx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gfmpcicbh.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gpachypax.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gffbzqtaa.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gvixlarfs.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gvghuproe.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gxaadxzcw.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gseikgfvg.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gkiedlzgs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gbwxhlakm.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gjzlgyfgk.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/glixcnoca.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gnxpqpbbk.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdmldhjoz.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gjzwxelas.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gdcsuqcac.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gfjqfwplc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gsuuguywb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/guultlknp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gmpefsgcl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/glnknxcmb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gtbsoinmt.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gwszgqnao.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/ggzvziaxn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gaxchlave.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gkpvnvxnz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gkrpdqtkh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gcjmfmwyy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gcrwaaaqo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gerfmqsmp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gnkcrurbs.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gomifrbtx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/ghkvwirgh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gguugzuym.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gbitvywkj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/giguzgszo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gqibpepfr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gjkegpbik.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gbvfidiao.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gvtjsmptr.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gdpljxbwp.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkosovzie.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gmolxeldd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gimmlchec.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gmkfepoks.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gfpxbhjar.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gjitbqhac.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gyfttfqqk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gwrqxofan.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gallptlkw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gzhvaonlb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gajlnbtwb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gazolaksm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gxwzkvxdd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gpopcucmf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gplqxlcna.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gqbhhzhoe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gucggydpj.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gghqxiwbz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gfhprotje.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gmzwxtvvp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gzenqazbc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtkyiqcjb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gqvczptpf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/giaarlhgp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gnxghufha.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/grcsvcxua.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gzarglwuh.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gshwccufa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gfkkifbqs.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gvkabqqkg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gifmqvzir.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gxpnvguhp.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/giqvvowun.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/ghhmpsrxq.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gtccxkqsb.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/ghirjlloy.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gprxmkicp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/grlymsnhg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gnifcpexc.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/govwxfaka.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/goykudqxg.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gzkrloxor.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gnxjkjuuy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gwmnmthcg.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gvayncouw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gwormolpq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ggvtzipdi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gyfhdthhu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtbmqzazs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqmbshopm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/ghwjmflwk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gjijvuowo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gyesvlhaz.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gzmrbghal.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gmptpvjez.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gjbnnewqe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gflcfjkat.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/goohrycbt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gxxhqdomo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gyzzjstgl.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/getbsosxq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gpfhhfygs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvmeeqgve.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gzbzonkyc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjwxalkun.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtzfgrhnp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gphndjajq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpzudhauq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/grpenscga.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gsjcggato.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjvuovebo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/glitpibce.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvvvzpftn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtebbbupc.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gmikffwdb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gnideqbii.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gxnlpcqpi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/ghjljshdh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gazbcrzfc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gbwjagtbv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqiokqch.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gafhzkprl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gonkvxlpx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gytvrgywc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gwnyyqvae.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/geccviezx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gpyalysut.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gftrfmprm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/glbajvkdo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhvvunlb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gbxevcjns.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gyadtswfw.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gqkqkdarz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gfuwszxhn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gnjmoliws.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmwrcutgo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gpagsmepl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gnuxwqvuj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbjdfqpjv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gqzrflhxv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gjfaevqtv.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gkxzetmww.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gdkhbjlup.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfvsptssv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbwzueiyf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkwvqhbfl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwdceqkmf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/ghzbjmrof.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpoxtfezb.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbwhvvgpm.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/glzjrsfhk.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghbkzitel.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyhohekfv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmhjsnwje.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfhupilhq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gqzffjkwe.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjafxwhjf.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsytekipu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gahdhiqxh.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gdrkfdmtc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/glnotlgid.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ggdwqmmfj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gsjpigppy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gfykyjbvq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gbmpqsxet.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gfuusqebr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gbahpacig.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gdinebbfq.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gsrswyqnb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gokapjzmg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gdmpqgzwx.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gkatzsaci.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gwdlnilxe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gvjsxsqkz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwwkbiuco.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gkikhnowl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/goidsqzpx.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gmvnokwxv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpsddmyom.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gscihnaqu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gimlwyzwj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gdjflylpy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gbddxkndv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gxpauywib.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbpkvnlrc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gayccdvkn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gnkrmjowt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnlpjjmgi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grgklbbuo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjwssiuni.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gltvteszf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gfcumzoll.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/giqasvmvv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gobdptcoi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gonhgskgn.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gytxtmgtz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzuztnstc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjdfstabl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/guciebwtj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/glughkybe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gfgqbuyws.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gzwiyauqh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjfozenxb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/grshczloe.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gztxcdsjg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gveiblexx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/grvalwhsj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gzkfplobl.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/ghtsgpohi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gyzaygwyf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gcynaxkwo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gpzigfdzo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/geslstfow.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsgeivddz.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gvohfyinz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpnmvooux.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gyrirxqiu.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/grxxwuhcy.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/goxljfnmp.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/guwtyzyaz.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gydxlbmwy.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gsenrdlyo.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gzqqskhyz.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gbpdcxrpc.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/galsnsohb.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gkswkdnor.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gxjbggcdo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gwlhelnsx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/guqqvzngs.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gxeynvgpi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gxahxiwtn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gjhxdiene.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gqktuqigs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gbvxqyebm.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gzhnthhix.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/ghrjciqqm.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gdhcrpqnq.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/guiowytko.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfbvtnepj.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gufnopdwj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gfgwdbjfo.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gprmobdvf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gjllkkwyu.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gaqhsxhue.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gsfjuspfp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gdwvioigj.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grfmlbkuv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gglqbptuv.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gssovtslw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gdilfbxui.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gwyeolcbd.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gnzlfpzyo.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gsesimilh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gbolgvdoa.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/glxcpwfli.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqhkjnpvn.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdqctgatq.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gqybwdmaw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gnduycppx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gxuljejsj.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/grbyyvklt.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/grsecfixv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gixlmcsvl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ggawkbexr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gzwactxzh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gybsakvwp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gnczmdewl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gswkoncpi.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/ghtlaaemm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/glrqfzkfr.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/guzxbsxcp.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/glifmueac.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gijcwbxvs.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gxmuqsmbp.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gzaitrneq.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/guangqrgx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gmhdkrfyf.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/guxdralnn.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gfzyipzqh.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gvbxfwtrf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gsnctunwz.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gkhoryyus.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gdvobguhv.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gvhbrzdxl.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzknpxjim.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gdcreidku.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/glkowsorh.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gmvhzhyys.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gpoxptcer.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/ghnstzsym.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gdlbdsltc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gprctjckh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gttmpydrt.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gaqofvujt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/girxzntpg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gwuvwdunl.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gwoajyjhu.sHtML


<!-- 参考信息 -->