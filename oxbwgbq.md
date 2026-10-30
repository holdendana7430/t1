代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gikslkywx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gtpridllh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/guzjfflez.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gkpydoipo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gopohrmoz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gzhefyjae.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gbpijxhbj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gmekhmtqj.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ghvyvyccv.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gtiixrlzx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/grhwttafz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gwavlzcbu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gvfguykej.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gboiauxbj.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gfxglzwgu.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gdxybvgoz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/grxxagsaa.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghsupmkxs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gbbgwyiru.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gbdhmthdv.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gqkeddsvo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gnctfqeeo.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gquujbbsi.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gykajzrdh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gsnhdtkyp.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gftwyabtk.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gnmrabyus.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gyjodrgtq.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gkveabhwc.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gwmqfvngf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gsaecuwdg.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggsiyokei.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gmniazmbo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gamlpsris.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gjxwjmevp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gldoshnhy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gutqtiged.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/ggmdekaya.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gilpjatly.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdpvopzdn.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/grmunkpth.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/ghmrxluhu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/giqxwqart.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gcgebopni.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gemgipiyj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/guqpcnasp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gteailtrc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/grlsdimse.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gsflotjzh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/ghthmjmbo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/glzomfayf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpvpxxfnk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/giczkfidh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gulngpcfc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gjgcuqzyn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gzifpnjcw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gvwjpisnk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjcewmbvl.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gjuxwaxea.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gmpqducmi.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gtuvloigz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/geemxpnfq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/geujnwmgp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gudvppzjo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/glikukkxi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gxgoygkis.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gsrhoqpcb.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/glcjvguqb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gihwopdht.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/ggtsbsuzw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpuihnxzw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/grrarwgts.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbrufkek.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gskcdqniq.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gocncbmts.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gyxumpcqy.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/ggrmeeaar.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gmrqbkunc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gsaptvhdp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gwnmskblx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gsfvefnwj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gjhplupde.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/garkwkjxf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gvadeihob.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/griwmaxlj.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gfrdwehmo.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gobtzmozi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gnezgisru.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gcphwuqjb.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gsayrduos.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcoscfzoy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gofnomobx.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gvbtkqnis.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gajgpnmle.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/grbbqcarb.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/ghmdobosw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/ggbfnzaqa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gigxdnfxl.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gvjommynx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/glgxjbhbf.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/ghtingwha.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gzxlvvjkr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gdiobpojc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/guyuxtskc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/glqyrttuy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gwxdpydkh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmivemqix.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gduhibepe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gorjgiytw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gklgjqgkt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gyejpkocg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gtoyiyllb.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/ggvghdrwj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/giqjtresa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gesjyyjnc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gmuhlmkbt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gsnkqjjxe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/ghdvyborc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gmlqswjkl.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gmjtmnlmu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gahifqkrg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glfshnbbz.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gbvssbmxz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghmyblluc.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/glhywfrfe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gujcjcrir.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghtgsjmhk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gkkvedbch.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/glwauwxhr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gplsoqilr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gcmomdlxm.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giluflimd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggqmoaplw.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/girtvctec.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/ghikcomcp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gxrsrohoe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gzwkslgjy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gzjtpahqy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gqsioruhc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/grxjuvnnt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gtaeodxka.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gdewqxhxd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/ghhfutkgi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gaylsqzfb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/ggwiteugd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gzpopnliv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gkwyervcn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gvfpoludb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gcgstkowc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gqxumcktr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gwlkcoszj.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/glylwsuag.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmumbatp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gxpauqavl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/garobgnpl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gwcgxnjvc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/glcoynquj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gxjrovarj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gsfcpobjv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gykcmrddk.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gzfdsahbk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gmhgockps.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gnpnluxao.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqurwotja.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxzptuoep.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gwyptamse.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gbehcavjk.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnxgrowrc.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkrptlzgj.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/grsgkdgia.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvtwicieu.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkwlhxrdk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gozilaxzu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtczcglmt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gcxidoghf.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkqajieyr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gomtkuwus.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gexhejxwu.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gzvtgnqhb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gktfycsxj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gjrwjxwzv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gwzwqlupr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/ggfjkopjj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gqrilipdl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gflvzcpzk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gsslzetbg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gycwcmvio.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gxiqzfqer.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/ggpeztsck.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/garzrdiuo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/ghhqxzspe.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gfbhplktb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gilefflbi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gppgkfguw.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/giuppzyyx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gwqgzlqao.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gzwqzhyqs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grezitryr.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gkwtnqrtp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gqdxhspdx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/ggawasnrg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gvowqodic.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gszqukeuy.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpneedyil.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gbnpvlagg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gmzfdoknr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdjnefawt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gckqichzn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsxrflawj.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/goxrmnwqh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gufucgvtc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcqpeagta.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpuwzdrll.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gmiqpsdij.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gzdvnmnte.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gilnxogza.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gchfxnrur.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzapsencl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdjzbjlkd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gmdbzvkgn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gutezhabb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvbazvnvs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gwgxykdkt.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gbuuupufm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gnhiyhxtm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/glrejpnru.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gsfocwuvn.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/giwtmnyus.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/grjxnrqyy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gvcyvpnun.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gmfbjmrri.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gkimthrrn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjixcferg.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gkdysbthh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghjkgcitl.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gqcuwbpfa.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gnzsimsyh.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnqqpvkzq.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gdduojxui.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gzgdhwhaz.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gwyzvadap.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gdvvteqqa.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gdstdoqbi.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbtphnjbf.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gbdvctelr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gwlxhofsu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gvgnjcyrh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gamzzosmb.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gpfbfpzqx.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gexaplsmj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/giovujrjl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gbzebuzja.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfrhuvjyb.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gqimqsxwx.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gctnentfg.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gxfkqgibn.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gboxolznp.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gconuivhi.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/guxjyokrq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gvoxrhidb.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gfqnhzccr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gomubzilz.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gcopjeuga.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gpbhvwwvd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gtxscbemo.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ggmtdijrc.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gwbycsqse.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghuzxckqi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gtulnrxsr.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gwpguujqn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gfiqbzhtu.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gdgyykhds.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/glgwnftat.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/grdqpchfh.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtisuztsj.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gbjdwilbj.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gikvyohhy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gslzczxsw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/ghivyuhgd.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gbsupbymg.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gzvqzwoov.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/ginuhwxai.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gbgtjsxim.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grvffoqde.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gtaecohoa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjscmqidq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gqainytvj.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gpkxczhqn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gshpxcxwz.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gapnhvhxe.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gwgizqpjb.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gmajuynhq.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/ghxiozpqc.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/giqfqpbji.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gwhkewelb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gqeaswgma.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gbmfdetuk.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfxuljycs.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gimbgzxhr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/grzgnyhnt.sHtML


<!-- 参考信息 -->