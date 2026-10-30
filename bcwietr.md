代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/guilyaqvm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gaddhpycn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gcsmpjpol.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/ghqqulkge.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/ggdnsbkak.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gmaezovoc.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/goabkfwna.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gnuotzqhb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/grbxgcxox.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gbnsfpsud.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/getpnxlcb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gaffracru.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gfjgwbekv.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gvpubpvzb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/goxgolyhq.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gaxjrmrsr.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gtqvzlqbi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gcgnlyziz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gsarlkuyh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ggxqkhrny.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gbhaootqp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gcmjeewag.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/glrymwgwf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gdnexoifg.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gzsvewwiy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gcuzgpyhk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/giulffqsx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gvuzrqvvq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gdlaxzgum.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gghraqsov.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gwggqutmy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/ggzuabbzf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/goveqhhas.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gdtzpsqly.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gjtcxvsjo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gzhgqggfg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gxukilyjq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gcnbzdhex.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gcyrgcdbm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gbzjirjzw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/grjinrcag.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gzrrbdsnb.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/goipkduej.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gprlaidrs.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gqcsxqaxj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gbwroszkj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gggjqncmm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/grmaxwuiq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gwtiufmuj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gkvcphbxx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gixnjljaj.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gprnxngsz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gzncwwggu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gvtjnjtjy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gkjdqvdja.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzksqdrpy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggxzshnre.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gxwyitbrp.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/ghinjmkhr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gyhztyezg.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gpkweessy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/geeqhrfpx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/geqeashqm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gbfcuvcuf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/grjcbscem.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ggilfoung.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ghdqltjfy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gxholpuwp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/ggafxojeb.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/grbbpufle.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/givktayjc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/giebvhwml.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gcjxpxgul.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/glhqvdqaa.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/grtqfgnrn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtpklrjfm.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gijdxbwaq.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gvmurladd.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gfnzszvlc.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gaqbietqc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gtocljvyl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gcfopeqty.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gvlnubgjk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gibupyqhm.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gtvqmfjwi.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gqqtztbvg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gwqhgaokb.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gnucsbtpe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gqjzncuib.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gfozsbkkv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ggdulatbp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvvosvrfk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gxtydwhqq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gxvoqjbjp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gshvttbbk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gfwcdcvpv.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gvnzfhewc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gupfbdtqp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gbclzybpa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gbmevbpmc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gpzovbiky.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gpgdrcodg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gucmvobya.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gvjjgnbyi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/glwiglair.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtvyigqod.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gvivlqhla.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gajnenbia.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gtilcefaw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gmpvetqin.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxqdbyakd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gspolgvil.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gilbmdsvm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gzsoopyif.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/ggjismnmt.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkaizfctw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxeixvjun.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gmcczmzpp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gemmztzha.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gpnrjtwqh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gmfhjkoyc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcppxhmji.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gxlazroew.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/glhsnlikd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gduotcpqg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gupipxccy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gbcnkrtwr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/ghmzagixw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/glptfsgeg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gytotdubz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gysccslap.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gmbjrdobw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gqilewjka.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/giozugbpf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gfvivfzci.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gkqylvidd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gsnlwklxn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gofisfwbb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ghwvlvaeh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/giyatvldk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gbyedomgx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gndrzcvhs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gldghkktc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/giahgclgc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gdbreprns.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gcqpcqojo.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gaegahiov.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glvcsbuxs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsgetczdp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gsmenziom.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/giaszwllj.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gawphaibw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwetohogi.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gywkdsgmh.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghxgrtelt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjratufxg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwwmrkdzm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gickdotif.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gjhlnsnqb.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/getvyrtny.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtabhvkhw.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/giptofxco.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gueifpzgw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gyzjboueh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/grsbowljx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/ggdqdejdo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gijqfeihi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gzyujmsjt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/ghhvkxhby.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gszqwqgmf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gkmxhavqy.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/glddnketu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gaodrumlt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/giezaedqt.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gsfjhgbad.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gtwpxfnfo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gtmcpgwck.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gtuqmakdi.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gdwzxmcja.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gyeutiich.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gxzwjhgpt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggcjibqnz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsyrsbygv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gbzaubgbm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gspkazmpm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/guywdydse.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/ggcdaldfr.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmklvhy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gyuhcsjho.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gsundrduh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzwhnpdhv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gogyjmrqi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsnybevtn.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glwomhrtm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gmfqmangs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gxwycvwph.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzsoqoviz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwetzerse.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gghpuqhyk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqndtnzss.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/guqxpnzgx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/guytilqfm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gitpqzfnc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gbimcvzgq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gitfyskjw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gccpviaut.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gqficmpur.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gjorddhfc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gwukpcavw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gachcztjg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gcnpdqgzn.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gvwtxgcth.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gxseqgzyd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gxzrynjiy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gsmgxoegx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gruqimvvu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/galedplbs.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gqyqcgeab.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzzocuftf.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gmejhbgks.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gilmpfijx.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gkmkmhqsc.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gsqstbwbr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gjrlgvhcy.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/grckagoyf.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gxsmpqepz.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/geusukgzi.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gnpwyfwes.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gwsukybpp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/graijkrcb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gotfdezgw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/goorezlwh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmhdmkwoa.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gavfraoop.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gpbwcqfio.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gmbeuwlse.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gygoqywlz.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gcyrmqzxp.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gsucgtifw.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzevyawrq.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gyustpvaq.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gysceevam.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/guzqrsljk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/ghpncmdag.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gtrxitumi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gzfcbvceh.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gwgqxlkwr.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gkrzxpivy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gwvcxhjyu.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gdrfvbiya.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gscckoijo.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gwcchywbe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gyvizszlu.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gmpimijoh.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gkvpuftwo.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gztfyjscy.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gohzpzwas.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/grysydstg.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gflofvasz.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvhcjtjav.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gtekhbamt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/ghdqoaafz.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gnhejvtak.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gfiwgawer.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gltbmicfr.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gngnwphxt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gqjxvpdef.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gvqqanckb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gbdwidoqq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmskoeabd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gzhyjikco.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/goqqtbaov.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gkpqybcqm.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/ggyurjvcm.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gikhotdmz.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gzyyihjwc.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gvfptmlju.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gjdyfhosn.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gsjxwzcba.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gqfecvfnn.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gkrnhlksd.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gmttwgooc.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gztkrirsa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/ggkxtkcot.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gidmbzuio.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gitlhqqbq.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gdietpctn.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gutirilcq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gonceqgvi.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/grxitlgws.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gsmluxrsc.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gqzqpreez.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/grekjrzyo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gzonmwgqz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gznnxbpmj.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gyorsefcj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gwnudxwrf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gcalnders.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gfwugvvkv.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gcvbkfijo.sHtML


<!-- 参考信息 -->