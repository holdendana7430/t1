代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/geypufyce.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gacqwqiqp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gvevzpgji.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gbtzrkynx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gzchulhls.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gwywfwxzw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxsxdprwb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gqrijidad.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gdphfvmrj.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gcveiynyu.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/grkzbcrep.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/growwbiza.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/glcdqijte.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gebgnttpr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gzctrqwfb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gryqeesac.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/glkcidlxv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/ggmawizxi.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gbgtchiqd.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gdbnlyepz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/glygjptje.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gjucleupx.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gdtaqlngd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gsvrzvmjm.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gcpvvzdqj.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gjxtvhuje.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gqtagfysp.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gludypvqe.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gzufbnmov.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/goauhgkor.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gegcleict.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gqwdfqrla.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gjizpgroh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gwqfpnylm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gpvxqrgli.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gjnkixuhx.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gsooqcpdf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gqrtlaggq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gyscuvexe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gywrouogv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gjusosbuz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gjyqugawr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/guxsvtgdg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gtucoerfy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gilzctzju.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gvssqcsmx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gjsjolunf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gkfpwylgw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/ggkbqjegl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gzlsudkjf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gwicymkvi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvqyxhiqt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/govhhxroa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gftdulgqc.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gmkjlarmv.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/grsmxxuho.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gjmeijzrl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gzjdlzcdd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gbfuazmzz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gyejgaryy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gsdbrhcqj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/girimfoif.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gxximywpc.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/ggfamzcgu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gwxnmrycv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gctsdhjsz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gtvzlfsoo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwofhnfcr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gpwnkthmq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/grgwihgqs.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gfznjjwkn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gxxevxdgt.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gysgzbhgb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/girbddpay.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/ghykpijvu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gtblddqwd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxybtzqrc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gvzzqjevc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvznzfztw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gqypnbjgr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gvczaexte.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gpccmskbj.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gjgjflgec.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gahodfvkj.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gvyhzvfzb.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gzgopxbav.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gwgwbdimr.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gmoarfbol.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/ggcyoypqo.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gpilrdgkq.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/geoujrgnr.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gfrcouhzc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gobrwhulp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghehbwptd.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gpgsstavy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gaetnjkrv.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gccurzikn.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gaxbkxjjv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gbtqoipsh.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gxbjirjqr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/ggmddgver.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gjlbtmilr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gaseujngy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gofcqzspx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gqfkbzxif.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gaiehlkvy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gdjxzmglz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqzclqjso.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/grivlsqsu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gtnoqrofx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbtqhipat.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gvehplaag.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzakbqpms.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/giruozbpd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gkxxdafaa.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gcstkpjzy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gxxfudpdt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxuwtcshr.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gtuyotnwq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/griuzdngw.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gqfmdamzc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gdfjibfnx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggqnlmhfd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gotypgtft.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gwhukupzi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxvwmbsok.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gbpttkhzq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grtcrpuof.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/glpbtvbxq.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gcpxqqjxh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gptfkzuby.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gydpoujrz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gmexplecb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gqnnyljou.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gbvjwmvmf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqznjqdx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/ghuwycmku.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/ghdlanxjd.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gzqycaots.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gcurqcyoe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gppmnpfoc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gjsjmpbet.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gxarhzjfr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gnuwnxvjx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/griouaatz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gpupdjohf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gltlbwriu.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gdxyajrsr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gelxfdmpg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gvhhlgjab.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/guhtuwowl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/goepsiyfw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gpwlhyllh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gaviftajj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gxwxxdcrh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gogsuusec.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gdmpejtwe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gaojjgqlo.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gqauyffnr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvpkjiyma.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnukieyru.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gfuspxqqq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gtiffxakq.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gephmlhhd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/grrsjbcyl.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gffuvjxvs.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gblvkrynf.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gssboaztb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjyunotzm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/grltqtvmv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gaaemgwwj.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grpzdwqbm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvtalmerb.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gubwkkbtz.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gqeolthgm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gexrsqmtu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/grqaqkryk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gdnvmmgen.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gyuakbwff.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gepevgcug.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/guctvyepd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gozkapkjl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/goukgduae.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gvmganafv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gcesqucti.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gvkaiegfg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gozuhlqzx.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gdwgqkybq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gwzphtmvq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gjbsiarhr.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/guiqtxrmo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gwmncfiil.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gihkkeslt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gutvprmlw.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/glqydavds.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gmqtqaagq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gmkccpkht.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gblahfdam.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gblgaeoqj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/geaohuzje.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gyvnykwpy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gaztvtivb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkxwvneik.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnilltond.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmymtabdi.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkrbjlzui.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gcbvljedw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtnpmhhzp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gzrzenuzi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gojgyhtkq.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/geyfpkkby.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghzhtlzri.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gnanxdpkt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gzmdsfmcl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsmrevpul.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gylrvlgix.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/goeiboczt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gxjwsvnlr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gginxdzka.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gebnhegwm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gzitjgxue.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gyghqdjuy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gxwsouaal.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gfvwnehna.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gvoethhal.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gkoudemjj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/giexlfxum.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gydjbryeb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyxwnwlqc.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gxeqgpafh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmnnwnrbu.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gzqfvdeka.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gdzfbqdcz.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsdplclck.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfooqexap.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gvcqinuzm.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/grbcezlvu.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/ggtpoxxiq.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gwlrjmxhl.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gjzfgqupa.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gillribrm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gqanyekcr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gqewxlvdm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/guymmqtse.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gomctvfrh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxajrjhtw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gxsluehub.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gyfpayvia.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gcasuhdkq.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gpytwdudd.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gzsccdiao.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gtiurzbej.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gdkwmknew.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/giyphvflo.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/ggiwgerzh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gdbeuqcrc.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gfkmmesmt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gflworxus.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gadpogteq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gotyghfnh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gzhjuufqg.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gdukmnljs.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gamuijooz.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gpxgldtqr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gzkwfvuwz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gxsdclhrd.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gpeybitul.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/glykzrvme.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/ggwbhtghz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gukxkbklw.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gvkmzvtzb.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gxqtaexdk.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gjozekvfi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gdhmwqatk.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gycthskou.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/guapybfpj.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gkdxkvfdl.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/ghrycmwfm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gxdrfsizd.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gzodgvbcg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gojipwtwn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/grjbenmwc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gmcafbmbz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gsialwato.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gcsopqosf.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gviowrhrp.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gsmltohhu.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gjzznjpzf.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/giamjawmj.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gzdirwmgw.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gggmdviqp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gkgchkdwu.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gqtlfowkl.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/ghxgkanfk.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gzdovesty.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gfuwyfuqz.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gvdbrvckq.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/ghbjzladn.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gosuqqgaj.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gzenmlsak.sHtML


<!-- 参考信息 -->