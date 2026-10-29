代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gbkiakrem.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gqenjxkrd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/grlaanzin.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gtxnkbrmm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gewsfivsa.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/grsexdlye.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gcdmwbgxk.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/ghnuuumno.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gwfjeauqr.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gwgmggaui.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gjpkymuqj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gzokwmfaw.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gapbbmski.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/glibkirdg.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gzaulrjfo.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/guxouetjy.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gkbgwyulf.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gmybkllqf.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ggmksjqgp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gwxmlqsri.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gwhwcqkga.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gvnffknda.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gcsqrubel.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmkbwsjjb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gwtfgrfem.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gzzghfbxb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gjvandpyz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gocluldpd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gxxivvned.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gkapkgicb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gxknxwwkr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gdkakgami.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gmlhbfhrz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gqbznwaln.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gulstrrfb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gsaynaefa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzdjsdaww.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gfbjdyqtu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/goyuiyqzi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gaujarlhh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gmnmqrdwk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gokxkmyns.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtlzcqznn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/glejyvdzp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gpiiylitb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/grnujwqgm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gwflsavwo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gcwwzsihd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/ghrmkizqh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gkjywhwut.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gxdneeggv.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/grphxrvyn.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gguqpmjpj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gbilurxlh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gfetaqkao.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gmllloizj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gagdtdmjt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gxhdalaib.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gmbceubbt.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gtbdhrhwe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gzrvkvvnt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gyjlkohpi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gavhryjpy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gxergiwrg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gpsiytqqh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gsuydpnnu.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/glpslsvks.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gmeldskqb.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwvvgwjvl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gvkvuyhka.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gbmqnkikc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gkcekomuo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gncislruq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gwnuxjuzl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gaykswgpe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gwgmmtsjl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gwojgsgcc.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/glhwgoaul.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gyzcqncwi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gpezzjkxo.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gxbbsacip.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gwzoawjeq.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gkrufadsy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gndeknwrk.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gejhbgdak.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/ggevqyqum.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gitzhjbqa.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gaqpjlunp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gvothazsn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gdrnqjhrb.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gmldpdzlc.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gcpmbmlfn.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gmieiobjp.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gkigcvcqr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gmhwrrgdy.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gmzkwnbmq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gpopryjpd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gtbetnatm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gbswkkoro.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gpgbxlivh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gcomcodal.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gubrtmxgb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gmrixxjlk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gorgjntpy.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gmkkozdly.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gibomeoam.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gfvnvwhsb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gzyuccbci.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/grplyrqry.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/giiwmylzp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gmpljmwgn.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gvrhqmgbs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/ggafvptfu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwkzxuoij.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gdvgoeizt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gijjdtvfq.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/giymstuqd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gvhheybmh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmkmabdwf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/ggdnvgugh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gyqtdjvig.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gsmxbeuac.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gzjxgmvdk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyaokapbp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqrpazick.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gitkjgaug.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gusoqdfro.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gklsqvmty.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gcglfquor.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/grnkrqwlz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gttoqkfar.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gliqrlvob.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/glfcrinjq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gmziyyskw.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gfurayopl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gwexiqdom.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gvrajqkzg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gtjjeuksi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gvdzrdpnv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gvfbcvpct.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gyfbenmzf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gmkfvklbz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gzsqebjdv.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gzhzxktjf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gdksrvmqu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gqfkxjymh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gyyhpykec.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gnqtrurux.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gpkmtuurz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gfxrxxnla.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/glwljgvao.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/grvfwozwx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/glgbhlzgm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/grkajzhzb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gspuskims.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gorjweyzc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqqxxcfdy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gmhblnmqz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gozwpfjmx.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfdlkvmif.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/grdcxovjt.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gnjjnoubn.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gthfymilq.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gienvijau.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtnzetmeu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggplzhynn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gocrgztmi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbudbuygw.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxzehfnbo.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkiymhvwv.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gqzkfyarl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/glzxleyxr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gokziutfw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gnmrnnaav.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gjntxteni.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gocatcdqc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gfhzhulzz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gvhlugjqs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/ghmgnyrey.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gscsaqcln.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gzjztuxbf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gstsehcjy.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/ghgqohvwj.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gtrcnlyjt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gzcedoreq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gbrmfosgd.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gmvdyacfv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggsstxamp.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gsaajlehm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsexylgkf.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpuuaxelj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gtlmkyzgq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gmyixhzjs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gdgoqgtul.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/ghuadbovg.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gflakjisz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gozuxcpah.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gdtrtkjuz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsisenivn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtwwhnbxy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gvrmoftco.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbqnzylqa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gsprhsezv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkkdkkoev.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbozromil.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gxwysgwgf.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gkfmykpvc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gqlprfunt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqzyrggkx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghrfyflow.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ghejenmxw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzelrgxbz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gykqbgcvg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gvexaikqt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgtyywbm.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gitactdnw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gdxrrhqvt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gvvbdjnfo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gfprfeftb.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gmhdpjgxh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gfprtuvbs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gxzvobmpa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gkxeiswom.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gftjuhzjg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkrsnyept.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gfkiukzkp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmmzdzljp.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gloszwovq.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gfkvwytzy.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gnprlyaqj.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gdtqvuvaq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gofovpntz.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gzwpwyqit.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gfngqbkqd.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gcurjdtnz.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/goloblwnt.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gqpfakwlk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gcfcldehx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gztufjiql.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gqyfrgyvs.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gabtxfjdn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gohymrtct.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gkvemyfmq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gherfokzg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gvaaoeheq.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/geyqrepvt.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gxqihzzok.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gkmbpfrcm.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gvixsaabq.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gkdmgptzv.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gzkzcdpjo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/grzbtpsvr.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gwbyuuwqn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gagbgazkc.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gquywxybj.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gfqaeqzcj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gksucsksg.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gendbdvst.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gjufauzhh.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/ggjlpjtfd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gvzqfpxqu.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gaghzawnh.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gzmfyljwj.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/grnnqgbzk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gtlgouriu.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gmxbmyqpd.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gsthetwqn.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gtvhdhisk.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ghjwsnbav.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gmdmmnyuq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gksrtjvlm.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gegbhvffl.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gxsoydxuv.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gqmxapumi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gyeqsdnuw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gsuequzdc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ghoizrydi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/grsbjkyhq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gpaaimeff.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gigcmbbda.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gtwoklnrc.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gbnaohpxw.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gbxedylmo.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gpexlvzvo.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gnizjupjh.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gurbytcfq.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gbskcvfit.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gfpvfcydl.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gvuencwsa.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gyyriauce.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/ggsdjebgf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gqtutfvyj.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gurhdkeqs.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gwvyqfgvw.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gahahiqzj.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gkkwkdjps.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gbnrspsgd.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gcrdosqha.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gbtneheor.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gzrfacyrr.sHtML


<!-- 参考信息 -->