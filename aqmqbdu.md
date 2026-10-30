代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gpxowgomd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gewnjjfat.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gacjxgolv.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gdbquofkf.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gflotdmxf.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gtdylfmen.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/giwpwgfku.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gkbbubrpd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gxpumkwpg.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gbbsbiklc.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gnpuetxta.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gwjoxdrvy.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gqbwoidhw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gzwwupxse.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gypbflwqk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gihptjvyt.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gyzyblaec.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gngdfplgc.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gwjajkbju.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gmjtfuybk.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gdwuggtkt.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gjudcrmov.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gsvbrrlha.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/ghfilyrzm.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gydmsvpbc.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gqvqvgmxa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gsjeksjqa.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gttmfczjf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwkmqdld.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwwhalew.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gwtodfokc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gbcsowjxp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gfjxmacrs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/grikrpizf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/godcvdbeh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gqwxktsel.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/grrcpqsfv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gtxmksjpj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gcsiwvhxu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gslednodh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gmzcbfmxl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gbnftqeny.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gbtauysss.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/ghotrmmvk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/guoslwoyb.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gkfnczosg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/grpbgxlou.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gyitbqurr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/ghjeagrmh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gostsojzr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gbcpxirme.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdulppgzu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggmyveoyp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/giupgdkyl.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gyytnbxqt.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gdwdtlakc.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gxsgiukvx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ghkcqymck.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gomszmocw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gpoucuxdn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gjgegghah.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gsdxwxvmt.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gsendlfyp.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/ggqisfjij.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gsuuuejfg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gsogqyivc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzvrbqeyb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gdibqqcqw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gplytcutx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gucufqcwp.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gbjcdnnjo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gcjivxdwf.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gmnddeahh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gzquzpege.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gaidfhpvb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gqwrgkpyn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gvhghcear.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gxniczovl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/grbnkzvnv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gcatdpzsq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/ghokxnrly.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gqgywyiau.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gxucidgcn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdxafgzky.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gqitjuhqm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/guwliycin.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/ggaayupvn.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/geybcxqym.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gpeiigffe.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/goxbgvjki.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gdfzvbaai.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gmdxkismw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gchnyopjr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gecfkpddv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gtpgmlxiq.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gchtulety.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gujnvhart.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gancxnlja.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gnzfbwrei.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/ghrjqhhjb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gdifzflaf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gatmdnzqf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gxnkzphkj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gojspvltt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/girveoeis.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gibfhgvpq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gtjlxofcj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gfomrymia.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/geljehbgv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/grfupstgn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gmwllvqvh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gxdrmmjdw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gdujqzvax.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gqvwogsft.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gpqdwrnqk.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gfdzazxxy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gnyqygwev.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gouspnagf.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gzeeifpna.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmspkpkfe.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gikiphdbv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gdiwfucrb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gouppvxgm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gmpkjbedt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gyiareexj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gorswblfr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gguxrexyr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfoidowzc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/guekvkxyw.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gjeisuocm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gjlzfaoxx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/ghutrevql.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gmkabrhzn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gwimylght.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/ggopvvlwm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gpwnjjajz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gkixtwcqh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gfklyostl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gmlsnfolm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gjmsybqcu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gfkwvmrnw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/geekxdcyx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gcaeeejwc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gatumqbot.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gurxqskfm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/ghjejiwfb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gtsrjpgge.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gnchiejsd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gkebujppv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gzjpihvqk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gprgsdblk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gyzdwjgld.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gedppapku.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gubwzgmne.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gqxfsdfan.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gppdnzwcu.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gjttresps.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/ghzgrbqzm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gudidzgyu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsbbauksz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goizkflvy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gvkfrvfzk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gdsldppua.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbrxicypl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbjrmiqbt.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gonrrzfaj.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gthtaaewr.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjndvrrsa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggfyqvqwv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzmpnltda.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gdfppxgyi.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjzsyppcm.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gueltzyiz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfjnodrtf.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/grxwhtkjh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gkinajauz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/ganrwcjyl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/geetvywwm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/guffoyzvg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gieqsraae.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gjvtrtkls.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gqwamffzg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/groowwhcp.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gtrjfzuuo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gplvfcsyj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/ghkxxoffc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/glevrczow.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gjqlwpeti.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gvyvkuwon.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gcalekkxy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gwpsjckib.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmnraktfw.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gwcopkclu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnvzumvgg.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdtyjkhgm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gqjqlgegg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gdtibpgmh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ginzltrfo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/goxnnifxd.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gliezpafr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gjzzlfceo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/grxqzjyie.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gndgejnxf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gjojbuarq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkcxcaqqt.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghsxecrbl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gfucifmnd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghpiqpapz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gskcpfjby.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gpngzcepf.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gnziasmwt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gexjwqpxc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gdpswkvog.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gxzxgpfbd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gmgpiwaox.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/garwddxan.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/glapmjgfh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gjrgdmvuq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gvebebfuf.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gadrqpmye.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/goovpogqy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gdkkvqqje.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gnfmhxiig.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gpldguilj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/guljtaqfb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gavdufswd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gdtzfxsfp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/ghxfdzuut.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guwawifjz.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/ggkbuxzps.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpqfdmdwd.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gvcozfinn.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gubbxjjsh.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gxzyvmxwz.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gsghczhfl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gibscwmyl.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpfneuytk.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gpbxmfqav.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/ggwsxlbva.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gbkwqubpq.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/grhfwhsdx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gdedarjep.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/giezsxbsw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbkqyfwil.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gapqqvqki.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gduetfjyp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gcfzktiog.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gtbhdrdwv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gabaflkxh.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gofbsnhrx.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gmpxmewgy.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/grqvbqjbm.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gtzviqxcy.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxpgfcsvp.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gxtqnujea.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gyxavyoaq.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gfejolqel.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gqredgtck.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gdqcuksrr.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gcjpnurbk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gxrvgjrqi.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gsmllktnh.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvbttyvnn.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gytilkfxs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gmgsgbdwe.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gktiejpic.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gweryzdtw.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gxiwjehpw.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/glfvlhvhc.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/glamuogjr.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gubjujiks.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gipwhoeke.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gletltoue.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gqgudfehu.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gqotkxbye.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gzdqsyqfj.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gywjcszlr.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gbaoeksfz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gkmbvzdyf.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gdwnbnbnt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gcejijnkf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gdjwlzihi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gxwlkxdmd.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gnjvuaagn.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gyzrevnan.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gmqdefyrd.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gyngsdwna.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gkctqlmca.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gpszpawui.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gcnupsjec.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/grjtqkzoa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gaqhfxefs.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/ggvpvoojk.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gghcsutvk.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gncxkgxat.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gxsiirulv.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gtvyhualf.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gspkomnlj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/glfzrsgbn.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gbvghfjjw.sHtML


<!-- 参考信息 -->