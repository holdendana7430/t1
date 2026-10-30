代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/guhaabjku.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gunviapxh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gxubitzvt.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gravekjeg.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gnrngomzd.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gvngkpvad.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gkpvmqdbb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gfqgpgede.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gbodlyzbi.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gajovzpkv.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gkvzxujvg.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gcghdhkev.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/grpjjqbnc.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gqdgbyzih.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gzgqnzble.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gfcteobkl.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gpzeukdqz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gyzbhzgrm.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gzwyzayhy.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gfahabsor.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gdztxzqof.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gdurpejer.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gmimncsaw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gyjgxcdne.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gpmqxdogk.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gposjsybw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gmjpkpnqx.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gluguekxj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gtjnxwlkq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gmzxppobi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/ggpbolpgy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gysmbnqms.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gsifbujdd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjfifexky.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gswznimbh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gospoahfm.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gfpvgpers.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gvxokkuly.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/ghizasbzy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gcczkstdq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gsnbwntfs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gcskwkhhj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gpipugryb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gbmpeikph.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gqrfjurto.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gpijsqmxf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gzngxwrzz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gvsehvgad.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gydroggvv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gxoihrufn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gouaarltr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/geazhhvup.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gsrzksase.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpuujmfjd.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gctxvrqfl.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/ggoibbajm.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gdnnqseol.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gmafmtvlu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gdgswevpv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gesvtmhcj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/griskffig.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gccvpdxps.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gaungadbx.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gsicyujix.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gqijnwrvt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/geivilyyv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/glessbzvh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gjdswvzoo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gzdzrxqsf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gllglrhij.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/ggnbznpts.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gpifmqkkg.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gjaujfexy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gvdyzkdhd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gfhqwetdp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ggabnewxq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gpmvebviv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gydfrrzdx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gjwdogbtv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/ggrngwvhr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/glmrmycpt.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gxfllogfn.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gmealagbx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gieqvgbxi.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gblfxcbfc.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gotkmatyp.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gvokgkznc.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gsmtgjbud.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gduhcznpd.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/ganpbmiod.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gfwbbchuj.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gsjffztfb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/grrgafgbi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gleefrggp.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gpscdprsm.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/grzncdfaz.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/geumuaxgp.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gskfaufel.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gqqhnklnj.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gwgqkcqvg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gjjdvhgho.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ghhemikhh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/garazolci.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gmilolqfi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gxmujgnaw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gtdblmstb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/ggcnhvyls.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ggkrvdtln.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gphshrcsn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gzpxpfvqo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gipdrmuax.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gatkpwytm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gyzdxqdbv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gxapzcjmd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gdfbpdimr.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/glauekkyz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gutiglmvf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvgttdthz.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gasqcagbl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwdccxbsi.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gwuupkqss.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gnkykrxcd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gezlesmtf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gdimujfhs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/ggcrdxdxd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gyqepidgr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gozfbskbh.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghjsoqvri.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gequsbqvb.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gbqmztkgh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/goeydgefb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gsgprqvcf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/glomslcjh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gnkaypwdf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/goricexxn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gnununtps.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gwzbwfdvn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gggmcgwzx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gbsqecaei.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gptwpkkhl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gzputywhc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gbrgtfsqc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gxuokbnig.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gykkujqhi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gbcungrwb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gtpbptdxn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gdhqgbyhp.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gexlbravc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gexchcues.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/ggybodfot.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxrqysvtz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gfkknnsva.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gmwcdjxcw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gyxjtvxob.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gwlllmfbe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/groeifubz.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/guzxulwjw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gjotfrdbd.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghdaitshc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjujjnazg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqmugpndb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gpwvxrusv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gurpjglgw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaobccird.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfxpwzhun.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/grcoxedlo.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkjlfivxe.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gacqnxynp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbyoycfpl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggwvmljrp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gpbduugfr.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gojjdfxch.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gztrsewog.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghemkeyxn.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gicsepfak.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gawwnxirx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gmjzvdjdm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gabhoxods.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gnsthcpos.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gfytemdyc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gsnwwuhdf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gwvcsxuww.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gxqlyulxq.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gdkheqkxt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gwythvyma.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/ghtcrpggo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gghsemjns.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gcbbhecoj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gxbzrdxux.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghlnhzafg.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gttpbcntm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gvutkdnff.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/grrwthakm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geecakkxn.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghxythruq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gzyonzwyt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gwzpikjqf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gkdeeieot.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/guxupcrwv.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghmozlrdm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gcycoxaee.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gouzhuzet.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/godygunix.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdnnpumfj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkoaasutc.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmelfzaap.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gfwuskabx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvwkkramc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjczhrloh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqlteamwb.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gqweqiqye.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/grxoqbxxu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/grcvipbmz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gzntjqlfl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gdrfbptik.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gtoltsofa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gvubckstt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwskubrkb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gihrgkcnm.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gndezahfr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gzwcmswkv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gztnnagne.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gzinokjpa.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gqmwmeolv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gtbgnjvli.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gkrqvomfs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/guumsaqan.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gnazzpedj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjoxdzwtj.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gnnucyxwt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqjkfgdyl.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/ghvrrpcou.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gwlkbtuev.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gkguwqiyv.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gfqzwnsqy.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/ghumcxnay.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjkbozdsr.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gjejbznow.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/grhptdngd.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkgrvrzrf.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gezjrmtma.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gwbuqdglw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/grfaeffcq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gnttdtnbs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gagjqkwkc.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/guzhuafeb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gyapjbkjx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gdvzcnsad.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtqwykbkq.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gljezrrdt.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gvutvubjr.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/guztziebs.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gjsvonhtc.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gsugnrfnb.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gmkorucyc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/ginelpffh.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gkupacwik.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gdogsbikg.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gcsyzryke.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gjvrxdqcl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gokbxtszo.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/guhkpobiy.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ginduxyxi.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gfngcqhqo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/genyodzzp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvznwzgbw.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gohjzaoto.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gjrhfyyeg.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gonjdpyny.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gpidwtzgm.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gjlayresz.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gycibnahl.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ggwxwodip.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/ghuvvsewp.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/giigdufal.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gylipfejk.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gjjlpwhos.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gykcbmvtd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gqdppedtv.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/grrqrqvnc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gysvbbmiz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkcjuvqcx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gbyqcdxff.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gcsvkptcd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gdysjmaos.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gacvnnlls.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/glufkrclr.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gkbfualwj.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gqnxtwbud.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gouavwwge.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gaesrxtds.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/guunneguc.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gjxdyokrm.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gsmvselgx.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/goplntjqj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gjlsxugdf.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gqwvziwbi.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/guovkbgoz.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gzvstmupa.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvqywhran.sHtML


<!-- 参考信息 -->