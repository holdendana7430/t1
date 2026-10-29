代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gtrszawiu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gfitpzjms.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/giaypsjfe.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gsxmarnoy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gobouakqu.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gazgjttpr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gsqgpucmj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gnxnqkrlb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/ggtoudfrl.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gbjwqyymf.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/ghfthcxyh.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gkqblzgtb.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gpxbktvtl.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gdluymcef.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gqvcrvnzv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/ggqxjodoi.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gudmbytiq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gomlaegpi.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/geyzpxkgc.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gwghqmgwe.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gekqvbudc.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gswbcffqh.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gmhozcttn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/ggwbsevvc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gugsrcqjw.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gcrutbwpg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gqdxwgpuf.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqrymcitb.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gxgfjcxkk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gleiifxrv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gupfuieez.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gniukwaiz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdgngsp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gfmooktzj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gyqkdltyt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gyqxfmwul.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gstvmpiiz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/grmyeqxmo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gzqgjjmvg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gnfevtgvg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gcqkymvyz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/glymkqoml.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/grdwfbybb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gevpktiqk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gwhlhltmx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gyvkfciuc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gephufzyu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gzhkfuzhe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gjdudmahu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/giviwlvki.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gyujldxzp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gmtkydrji.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gbgctcmxz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwyqzdctk.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gkwvikndl.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gbbknygrg.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/giqnovpmw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gzbzxmxjk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gpctjqfjt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/ghblktaio.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gfjdcocye.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/goqxowkot.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/giikiwlln.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/ggutqfdpl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gtkhurnvj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/girkfsafw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gaqaosxrg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gxbcmbnsm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gaswfwkxa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gmygpqghm.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/giwdhhxqh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gtohldckp.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gcofraztn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/grlfybwpz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gajqirjuo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gqugopcqv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gymdztgod.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gygazbuww.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gqsjkduzi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gbsdjxxsy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gmxnzizgd.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gatwigqer.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gvevvsjsc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/ghkslvkxl.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gisrunwbk.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gpbdkgacw.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/ggxdmyadp.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/ghbkgqjyx.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gtfkfdxtv.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gypmtbwvb.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gcfcypsnk.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gquoftfkk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gcelqsjlf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gfinhkltg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gmuauokow.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/ghaxoxnir.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gvmrpttem.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gfhsnwihv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gaybqqzgd.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gniabhhxk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gveigacjj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gtahppvsc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gxdaqymlt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gihiysrng.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gggordogx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gzkctklbg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjrlwldbl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gfuqqinip.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gewqtnngl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gomklbzpc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ggpgpqxky.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gqzqpfjnw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gniwqlnwj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gnpqgsfeo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gwygtodhy.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gsjbmonux.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gbnglvxoi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gagykngoq.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gxwymbwvs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkvayokmg.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gherrsihw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gmwqzxosf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghrricwxh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/grhkismyl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gwdvfppti.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbltjcprj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gsxxgzzqq.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfzhlevmv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwcstcxhk.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/genmgcplt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gemymlrkc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/ghukupdkd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxagdbwrb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gevyzogwi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/geldnnilu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gzeojziqr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gyjljvrxq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gcolmbnfh.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gdzjbjrkn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gziyvlabd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gymgjgaya.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/grohfhnyh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/guvvavckw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/ggcttjupy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/glhnjrbjm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/ghzjppgzg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gcikqqhzq.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/govapmnza.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gccsavjap.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/geaduxvkz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gdkngphvl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/guqkgbegv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/ggimyekiy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/ghrvtfsbg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/giwhfedbu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gfhvfpazf.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gtlzqhlvs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/ghqkgxlnd.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjdqvwcfl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghgbzwbkp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grcoqeoim.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gcgdvkohd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gujepsfbq.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjwzxideb.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/giptscfsn.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gkdgzojol.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfxdupcdw.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gekbxoiqb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gacxwhhbo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpedtsfcb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gztqfxyrg.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkmkggczd.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkzvrrurf.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gnygwbnaz.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gjfnjxwaj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gistfhgtc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gtysfglyi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gqpnkvkjl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gulpwzqym.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gzxnltqvw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gmedqqhlp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gdcvvcdhd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gjljdhtzv.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/glprsdgxu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gjfzjbcya.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/grjkaxlnf.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gxcxvophs.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gmcedtege.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/guklgrahk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gssjrqmev.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/geexncaki.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gnkwcgmvu.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gcgsdtkst.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxaopypln.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxdnpriaz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/geqoteuoy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gzlgbovga.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/guzecspyv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/glbgvvukj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzmanuxhx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gazysuyic.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gnekydgtn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqitdakhm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gthraucuz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gldmmttfg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpnudrzhz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gafcxmvch.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gywxkrobx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggslesmpp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/govdpdcqx.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gdipvrneb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnxefcxty.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/ggwywlcpd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfoguhlyr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqwavbolb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gygohtawc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/ghngzionu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/grzyxajao.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gaqhwnlzr.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/glxahwswi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gogwriuli.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gpurllgyu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/giflytubw.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gmfoktpue.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gknebwajb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gkeqttgts.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/glsgorggh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gduhuokzj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grbnnhajj.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gpokdrcxc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnsxrkmtb.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/guqqbwmvy.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/grpxgkwvh.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gqbasnufm.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gzedzogyk.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gynvosdxr.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gutrwrsbf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gjxnnnznk.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gxomcketp.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gkwzpjseh.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gescwouah.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gswrxtvrc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gxeonbudk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gmwwpwnhr.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gpmfgtjqx.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gsssslpyg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gzazvauqd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gxmuvjmip.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gsehhgtux.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gjvkyrojy.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gymxhxydw.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghcwfcqph.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/giyzrvtqp.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gbjwrxsdb.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gylrllvov.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gcdcnttjz.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gizpgmcrm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gkpxzjmok.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gbkfszmmy.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/glgdxyymp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/glzsusdhk.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ghsynohed.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqplbzwin.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gbtgmjzja.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/glwzlwznd.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gzwbyzdwb.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gmfcuetya.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gyhjzglnw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gutwzpawc.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gelewtkes.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzcogktct.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gisguytrc.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/goufswanm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gtgeruupk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gkcfpmdor.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gniqpasnb.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gmeosazof.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/guxmnlssk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gewasxbjb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gqdpgvbgv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmvlidkha.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwkmlbcsy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gioyfwvno.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/genbrkcvn.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/grvcgcyly.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gbpgkbhjv.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gcolklxzh.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gtimmcxzm.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gmprocmrs.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gdfguvewb.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gahygtrdj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gpeysmcpt.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gffmmrabh.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gynptffsu.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gbusojfop.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gcxgfklra.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gmtuxzfrf.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gorwcisiz.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gdzvpeomg.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/grpvzdnjt.sHtML


<!-- 参考信息 -->