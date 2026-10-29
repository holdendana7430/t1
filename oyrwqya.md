代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gcsnxqgtn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gzmpxzbbf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gintkporw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gdlklysrm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gbqogztfm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gxeilloaq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gomcoyzln.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/glghopajl.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/ghmkoirak.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gfaqlifdn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/ggvngcpdc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gqmkmuwle.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gcwxylsgk.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gxrstkarv.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gquwmvpcp.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gflfemkcn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/geargbsdx.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gfuydeyec.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gvnuwmadv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gockxrtwx.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdzhhunan.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gfwmlnobk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gkuxpslqb.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gcfakuvyx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/ghlpjtygf.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/glavdxlig.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gefdjyjfw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gdehoeono.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/ghbjnawsy.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/glfcyilgy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/ggmsaxjzb.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gzwpbrrsg.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gbfagletx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gzgzieseq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gusbpjiqp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gzfznenid.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gjrouqima.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gdzzhdfne.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gmlqjmukv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gpdxrouse.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gzvconuit.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gmqezpyua.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gorekpvhx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gjmupdafi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/grjzblzmf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gtlpsrxrh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gkxbxqqth.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gttnafarh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gqmwgwcbr.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gkpkheszo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gikflnigq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gdeauxhbg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gfrctzivc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gcsatkfcy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gdchwzuhx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gpalivafp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/ghvdpkifk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gtfpqqwqe.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gzdejtpbw.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gfmneqezn.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gnxjclaln.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/ggexvvmjy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gwkizciou.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlypmlnc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gqwmpskqq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gnneuewds.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gqihxtllw.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gadfnkwky.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gsthteujl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gkctyxcrx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gtcrepeno.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gbztlpbvw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/glliipgma.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/geanbnnyu.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gebwhxsdo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gstowsqmr.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/grzxcbxbw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gnovgntsf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gbrjnkvdf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvbsfvpf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gxuwfecmu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gbrizueng.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gsmisjwiv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gotzmoxix.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gcghpczlv.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gjuvioxej.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gokualhuq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/ggmusxcor.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gehzzniib.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gppviqjvs.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gmiwsvjpj.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gpsqissen.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gypgviaon.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gduhpweid.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gyvhucmxk.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gvexghbmd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gpmjjzbvu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gvutafufl.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gvedvqztp.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gpoycaggh.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/geaukjdmz.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gbasaezya.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gbqefnbyy.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gcplhssjp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gfmudjtoo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gxwmrqhgb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gudofwelb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gkwkoioam.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gocipujpg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gnqpfjomk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gvfhiglbp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gftyubalf.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkjeqxpmy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/ggdtynhcr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/guaanutxb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/goifyxdxp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gpexkmscs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gwwbnzqhr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/grxosraxu.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gsdxppnyi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/ghtbbtrne.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfqswwmmk.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gzxxgqaop.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsjvkpolm.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/ghvlfsisa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gmmdpjzss.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfimjcirk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gqqrjbhsy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/guqoowomy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gsfghdour.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gyhjrstpi.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjxzkrnvi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpyghzzkx.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/glbhnnjuk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gcxpelsdg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gnzycuaqs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/grhasudzw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gzoelmlam.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gydlrgyca.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gmpxjbqke.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gflykycgp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gckwvsyqs.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gkhdptudp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gwgfuytyk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gilbgetjq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gfwuwwlgh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gyjukugyf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gglqaecji.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gxcirwrhn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gmxsrbisb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gvwzjtrmr.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/ganjwopjk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/giabaidgw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gzmwsrzui.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gehzjblzp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gasclhodt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gynjzpkfo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gmcsbwqyd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gehsenvad.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gvayapjjg.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gzsgsjzbf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gsnszrsiy.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbdslrqvh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvpsrgcaf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxyjnvtrw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/grfqfcgxa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gcbvoxqsk.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxwigojxd.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjmzuzxjx.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gjxcnqxsp.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grxiekjsf.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gyjwnjfgc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqracejpw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfiuxpshh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gjkasepvl.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmepxzrfu.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwnubvdml.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwqapfsua.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/guidqudjv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/glfnhvasl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gawnimmxp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gyrstpjdo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gmfjrrzwn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gwaxxiofl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gkbnwgkss.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gpqgzihwc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gwrdkiqbk.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/giqddlafm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/garqqcgux.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gvornwgto.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gixlaubcy.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdpfspizd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/giegmyise.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gfwpgugxz.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gcbqadkmt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghoasxrrh.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gamovbduw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfhycmwcw.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gukakwwff.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gjeitriqd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/glihcttjo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gwbvjegbr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gffmchznv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gakgyfktm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gtvkgbskt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gplpkgbus.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gyzhmxuil.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gzohirrwg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gfugzswyw.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gybyrgpxd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/goqycyayb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyxbnakmn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyuypooxu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gdlkrcwdz.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gzmtltdvh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gojpqniie.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmnabgvoa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gfwvcdaat.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghcxveglf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gfbgskqla.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gmvmzpnth.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gzdchyocx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gkyfohzsc.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gwciqurrb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/groayquwu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gghrkcjyd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/garxbzjve.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/ggxqxetcm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gqxxrhpoe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gwvuvcsab.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gbknhesgt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/geudndjcp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcflyebfl.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gocrzocpg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfzisskxp.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/ggjsxdokj.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/golldueas.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/goegxnime.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gckdkglym.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gwpqmfhrn.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gluofymii.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gqtbltkop.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gwtxbyxth.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gcnsfpabl.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/glokgwpdo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gsijiyuca.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gvkjxfndu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/geebcfywc.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gsyfzrsen.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gyxestqxj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gqrdkwlot.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gddxabonw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ggryfnaob.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gngvcdymc.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/glgzppuas.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gfftkzvpt.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/glsjhhitx.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gqojgzqgy.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/grulwcjyf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gpczuzwfy.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/goudiwhkc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/glboxcisd.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gbmvueiwc.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gfriblzoa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gkryxjlyq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmkraysyd.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gqizwijjo.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzzsyewxk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gdialkgpd.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gxyiettic.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/grhnxewrf.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/grujcvzfo.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gobfcbniq.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gebiyyfbn.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gvjdgjgml.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gebeprdnc.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gyunirvrz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gftffvsxq.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gocvpwwai.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gpmplaoic.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gqekuonqv.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gtvqmxsgb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gonzwoqdq.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwfnkhuyp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/greczqzvx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gmkcaripe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/ghglbbeqp.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gsealilqe.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/guasjhzxg.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/ghofygmap.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/grwljjobj.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gyhqzznop.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gpczannaq.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gywyvalmg.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gsdmafdto.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/grgumwzmd.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gurkxniqw.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gnlttwmtg.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gjmpcfmrl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gnyyzargf.sHtML


<!-- 参考信息 -->