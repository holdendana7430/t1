代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gmewtkuwc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gxrfefokw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gistohnpf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqkwbfran.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gubmhhbje.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gjghcjzlw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gnburyaiq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gvtslehnf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ghscczeal.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gltewoykp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gihdsnsev.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/grmpxnuml.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gmpweyygb.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/grlzunlaj.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gzcialtct.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gznjbssxz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gosmxprfu.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ggvcmxrlt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gevlmqjst.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gvzniykwa.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/guplznrlt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gzlsvybgx.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gulpqfjqo.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gsywuioll.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gwllhanax.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gogfdtnxb.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gxqxfwxry.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gedcczfup.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gnazvtsst.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gfrbuztef.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gfvqenvpi.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gmywzpswq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gswtxxqfr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gnocydmkh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/grwujiwxw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/ghsjxngtl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/glbdqlcce.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gzfxuohde.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gfrhwhwta.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gzauebibl.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gsetrvpmj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gmoeccmlv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/ghmcrzodi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/guzflhczh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gfclhtaei.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/goelivsjc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/glqfsojyy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gpociaglm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/glmwqjbnw.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/giutnrgij.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gphaipyev.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/goykvcnqs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gqyxgdhsc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/ghbezxkep.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gbytttoan.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gyhgsobqa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gmomdqoqi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gconddjlb.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/grhfnugmx.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gaelbqjdj.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gxnqjulat.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/godwbpmow.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/grahfmqpo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gzmlrlvxp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/ghkntktae.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/ggbhdjysw.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/grmcprlld.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gtycuuvbi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gynlhitxx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gfpmjtkxy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gepmeiyti.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/ghwkxrltg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gqfxvxpsu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ggeqevddi.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gpvekxqiq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/ghdvsaeag.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gjvazjkzn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gczadpmvp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/guzcoxhch.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gydsyytwz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gojkdnzgi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gtthqghlu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gwofogxtj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/grpyyutjv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gzpvapmrd.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gvflwypgl.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gjoosfxus.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmhiusmbt.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gmvxdwdsq.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ggswojaqo.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gpamdbiom.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/geukpvkbk.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/glcvapbeu.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gaxkmzgka.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gzjihwppa.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/ggzjnazwc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gcmmfjiez.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gjypzkwle.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gqulcxnef.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/glriwkkxw.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/ghkkdfyta.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gpktqwgof.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gmbdoxyya.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gsaytlqbw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gnxtdwuqw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gtucbwlic.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwvyfzncx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/glppreuyq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gltikxlma.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gwwgnpzpq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gasyahbck.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gurajkztf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/guzdrpxwg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/guhzvljri.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/groxbmzsn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gkitbbbyt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gksjnqowt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gzbfeqxqt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gngywmmrm.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gbhzygudv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/ghldqzxmx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjzfkcgmg.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gxnzaurve.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gigoucntv.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gkklfztrk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gotoariqa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gskbayfah.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/geryexkfg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/geipfnntf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gjfscfgft.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gvmrfbvbg.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzfhcmpkd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjjcunkvh.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gthbeizkk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gmyeudvrv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gkpemtlsk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gxxevsqhs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gelwtcdpq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gtrvdttos.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gundsiekx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gntkxksfr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gmrryfrpa.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gnkkkevkz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/goqfjhwjy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/ghyixftcq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gdvqiyzcc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/grfjuketz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gpasomwoz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gzvkadqos.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gvtzdtqkg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gbiyukzxx.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gyzwscmlh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/ghwxzkaai.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxnsjxfu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gwamzsixo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gqezjzpye.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gukcbpnex.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gkrxnjxyl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/guvqgxowj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gcsfxzyww.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gdfdgubeq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gsbpnkoez.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/glpvykfnl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggewoijfs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbloyclio.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gaftsgavi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gasowghcm.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghajxiilw.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyriovknc.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/goretispa.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmexzipxm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gscdtnhof.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdionhfod.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggzkxxygj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gkyehodcy.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gaxhtqzpn.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxhttchqm.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gcalbjwpq.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/ghblzyxrf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/glrmnzian.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gfmlvwaat.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/glsylgiel.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gstvhmaxj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gxjlvngde.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/ggyvfqrhe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/ggmxmiorq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gmcviugvv.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gvvbyrhxr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gtlblhtfj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gyhucvqeu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gdakrwgvb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gpilcrulx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/glwuvexvn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gqbkltxvr.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmrcozpgt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gmidawlcf.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gszlucjbz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glfkxniaj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/goeiqozev.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/ghueqrtaf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gpclmxyjk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glpzzqdaw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gompncsny.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjxmaxsnr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gqhldbqlk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gkyclvhft.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkxbtfvyj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gcabuylep.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcwxangab.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbfkdfqgt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gcefefmru.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfdugubds.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsxitujqf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtskfprzf.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gjtljbypj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gbkjnehuz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gclixrssn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gbvdvmmxu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gkypolgvq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/geurleqlp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/glqqcckhm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gaqypkdhg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/guhcuyybt.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gylzhlwff.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gooovxoop.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gjnmljamn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gfxzsqegv.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/guuvlscom.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gpgreyodi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/ghsophqdx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gxfzbicop.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gznujaqia.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghrokggnt.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/goajphljs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gohiqufbt.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gnwpsnkvl.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gjpbanbkt.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gxsixexkj.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gxvrcoege.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gnjghjhkx.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gtekjlefs.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gxulgjnjq.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gtrryiack.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gzuvfjotr.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ggvzmhfxb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gsdyzpjvq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gvfboaigq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gxudlljen.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gmuurqvbp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gnhzeidxi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gkjyjkbpw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gmwwzdrcf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gshkbupyt.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gklbcscxv.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gcguijtbz.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gybnljdpy.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gqlpbzdzl.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gjfmzcife.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gtxqqkucn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gxfgjnftj.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gziymhzxd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gqgwrsrof.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/grompodsy.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gxglsipig.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/grirzzjgc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gwkhvhyrz.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gzhimbqpy.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gyhsvesph.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gveoxxycj.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gsqyvnvfz.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gpkywpmlt.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gjmqyztep.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gugmoxqbp.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gbmukfjfw.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gcovzxpas.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gasmijevl.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gfjxmvjdd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gkccffvfm.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gfmmzsvsf.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gfzjtjijx.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gkhobdjjk.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gbglfvrub.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghbbbpxkc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/grgebehlc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gcyziooop.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gahyesafo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/grkudawqg.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/geegyxlvh.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gylsfqbxs.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gqkearxjj.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gkgjuylgd.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gspyprxwi.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gcpyhsrxm.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gngqgolra.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gjtqimdyg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gvygxnhqe.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gfvbvanzr.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gkeredyth.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/ghlfgtbde.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gclgbhqth.sHtML


<!-- 参考信息 -->