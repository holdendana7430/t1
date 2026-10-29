代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gjfqbwstq.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gouruxzuk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gnkfctkwo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gfbgzxpnl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/goesivnjc.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gfumpcftp.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/ghicvxbjm.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gchzwfplp.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gpysypmum.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gpvvrbdpy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gkpfysupz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/guebhnlbm.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gaiwuuiap.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gvwcckiez.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/glmzdngcj.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/geyjoqzcv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/ghvxzexmi.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gdigsbrcy.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gcwtrwgpd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gkzwsfeph.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gdbjcthoa.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gcoauxiil.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gphvyegms.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gyzqiqdif.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gctnyoltt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gbxfmknjq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gpbzxdijq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/guarmsigk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gddkunnnv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/grkhvbgsy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gveooqlwg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gezxntrza.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gonvimznp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/giwrbrdoz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gwmtsatze.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gglhykvgh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/glytsnapg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gcdkkvfns.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gjtwtyyql.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/ggtzxnuag.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gsatyscif.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gfjskaixw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/geglgykwb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gcmqqnqys.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/glrolhoht.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gelgugspu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gnmpqhxtq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gefimfqer.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gfovnsogb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gfckdzfjy.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gfedxulga.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gwclhdgme.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gprlustwq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/glscgfyrt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gcwnrnrpk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gcjsstxhi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gkewxjwdv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gjrxdymzq.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gtgpgngov.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gxwpoolgm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gdlkyoyww.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ghkadvuhi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gugemvpvs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/glbexgext.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/glnavaqej.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gkarcfagg.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/glxlbdmdk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gugqpoosq.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/ggzbtyflf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gduswaafi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gqtelqnqf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gkireplfs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gneujxmpf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gabvtuqbn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/glkqxiyzx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gmecwwdyr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gbuoomayj.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gmzkutwqo.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gjifsjhma.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gbhpqzbdg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gqiyzcphc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gltnvxmvu.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gjufreljj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gdvbordls.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/ggapcmbam.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/garomlfjs.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gwwihanyw.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gyheejoda.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/ghugtstri.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gctfduwph.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gdtokkuvl.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gchympyda.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gekivabix.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gqxxggbiq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/ggongmigv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gqjdlavvm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gfdawluey.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gyrhhfpna.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gtihidsut.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbgevruiv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/goqcczhfg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gektmazci.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gqrzgeiml.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gaeqnnktc.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gpterpygw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gvprauctq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/getgitlhu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gaizksikw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gknfmbbif.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/geqyanlds.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gselopqzd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gydbsvhih.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gradlapdj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdpihabpg.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gjmrdcifw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpdxykivn.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/ghyueywpp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gsabkfyfz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzwrwyzpo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gmkjipxkh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/ggubdhahy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gncxgsneo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/geubcawdl.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grcrlxhsh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmecswdme.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gzuzlvigh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gmesopiyh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/geuhtxzrx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gfqwnthrj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gkroraxng.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gccsjhdtl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gilqivnop.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/grugcijsn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gqtkwrrlc.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/glyaqpucp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/ghvyburiw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gvhohrhqf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/glxwvoauy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gqztdmnkh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gpvhofcml.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gamsjfqir.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gxnwjbcay.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gqsdrrimx.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gnursnmur.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gqwrtqvzk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gtsvalkuf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gnjmtoltv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gpnzpdohj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/ggwsuhfyg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/giqydkkwi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gamugvmra.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/ghvorlvqc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/grgugkoex.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gtqehegsc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gyuywtpdv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glwcpjttm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxajrurwl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gftjongxh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gdwcdsssi.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzomkwiqz.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gddhtzltx.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gkkdehjno.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/guxoiquht.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwnhqoxyd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwthtzgfy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/geoiyapqu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ghvwpjchr.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbsfwyxlu.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/geyizouja.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gufkwplyl.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gbupzuxou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gizfbxpbo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gbtqjidec.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gtnrnwelb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gujkmpsiq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/giavuteki.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/grvbpfqim.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gzfserwvk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/glvkgmszt.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gdkgeynzk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gqcakemyk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gvaicwmcm.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gzsktbmms.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/giiqjaqhy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/grwlfdjui.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gezbtzswo.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpxfkhove.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gmxpviwhx.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gfoemwgvq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxiikzmrn.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnksfegkk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gdvnxzdfk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/ghvcvtgmq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/guyekebqr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gznvpenro.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjalhurth.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gpytppswp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/giccdlacj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggjditrfa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzohhgbxz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwwoudsmh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwwphftnn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gwuogysst.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/glzwijhjt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gnfofhmfa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwtzccfkp.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gdekoknzm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gqndhtszr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gqaoocfgz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gtlaacwsh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gzovixdzu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gepxwtcvg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/glzbpbrsi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzvbfgtdz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gmpalvtrw.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gwxjqimjj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gzqdetzlu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/ggvcejxfn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gixzmoddy.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gxmowxxsg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gozwvieyu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gmqtnovix.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/guoffxwyv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gjezpqzsa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grxoxzsjx.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gmkgxkyjm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtucfcxpn.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gcdovpvtd.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gdacutdxm.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gfvalbahm.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gmikwnxze.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gxnzdwcub.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gvlwqvqjt.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gzkuoxsyc.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gsajtrtfz.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gkkdtwnry.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gpmkqqcxw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/glfplyepa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gkskmvggc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/geedxaluv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghwitzdlp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gfngvdsif.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gzscllpju.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gerrirafk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gkqkdswov.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gcinbabpy.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gmzvqllda.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gicwyuhyp.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gffnovzrn.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gqqumsibz.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gquistwvp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gwdxcnrzw.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gmwylaxuf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/ggoiheett.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/ggrihpknk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/ghcpfypqi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gbwipzbcd.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gqoadqpdl.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gvkvkaykm.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gcrrjzgnr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gujvxwjtb.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gstszgjdf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gqiemgcyf.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gdijeahiq.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gvmrehteo.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmyphkrsv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbylvdfdw.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/glmxcbvmk.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gflqgisjx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/ggtqdoidx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/glzvthpka.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gdobccrcf.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/guxsiiyuj.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/ghymmxwac.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gnhgzobwf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvzaieger.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gfxowfwaj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/griytxzmq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gsrnifggn.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gjgoptiyf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gisoskeuq.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gypkjflqi.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gcekqbnxa.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/grpvufecx.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gvalwojep.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gnozzaovc.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gcasnqkay.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gsbxjbfth.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gazwbejef.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gxobighfl.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gxvrrcdzq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gelauqwro.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gddacrdrp.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gpcpimdmb.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gnpmnlxqw.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gndvvgfhp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gfpxfxblq.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/ghezztytl.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gpdcajzmc.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/goghwiout.sHtML


<!-- 参考信息 -->