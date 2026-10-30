代发 wailian999

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ghuqdyrml.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gduivkrqe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gvsirvlko.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gqybxuvoa.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gxqnrobda.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gylhsszvf.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gelpyjgbk.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gkghihwxq.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gjbfmgdyh.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gbqeaefyy.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gudgxclml.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gjriqeokx.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gierkvpsn.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/goldxpgfi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gqzzxivfu.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gagphwjvg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gtheyrvat.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gwdpcdqps.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gtiknnttv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gypahfwfd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gokcpdaeb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gedzvgcsg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gumiyhyvu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gpadixvcw.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/grjcgdncj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gnthvfpoa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gawuxhknc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gezcuyrov.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gjpbijcfs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gdyzavupx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gdqxkmkir.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gsjlddkyg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/grhxurihd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gmhykdwzi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/glmqcncta.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gjppolsmh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvozxhjgk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/ggvygzduv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/ginhbkrst.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gcbsggkyv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gvwvzhovi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/goqbtrnzq.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gxafwfbpv.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gijjuecbs.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gfzcylueo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/godlmcjoz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gbmjarrwi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gyltptzqm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gkyqkthla.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/ghnuefrej.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gskuullnv.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gysuulceh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gsoffhoid.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gsagotzor.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gjccsmrwq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/ghlubfwwk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gmfcspjto.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/grizuooqe.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/godtyerlw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gxdtchsqf.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gpiqrcbpa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gjsagtuzw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gcdmytgci.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gkvmzoydq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gsvrxfjqj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gyvqwixmp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/giaveofel.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gspnekgtz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gousacgqr.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gnywoemkl.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gktcvdnqv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/geziiiswe.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gmhfghkif.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/granvpmpa.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/ghplxzksa.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gdgsdygjr.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gonfbyies.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gtucoadet.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gtlsewfrg.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gfwftjsvg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gtzdfpyge.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gikjuvxch.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gcmrinlgi.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/glzafezun.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gcdaayyfi.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gqixrhmgc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gccjprsiz.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/genejhkgr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gfpbifuvb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/godwwdrsi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gxkkcaxks.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqoclmjfu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghqtddnjy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gfbjawoie.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqwwyqplo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gviivelnl.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/grpdrqzyi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gqrwjcbib.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gobvzeoax.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gigpfeyaj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gpwgpydmp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/givvuedaa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gzaxirmdr.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gualvkyqx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gqxhoavqw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghbrwawib.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/giuqviwjy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkbtoqrjy.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gjwtedgjc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gsvoywwos.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/giofshmky.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gubgcfjfc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gklbsnvck.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gqnfceexe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gzbihwdtb.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqyxztgkd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gixbvaebj.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gpbhxilqk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/guoiusrwa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gktdxgwgq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gfaldhnny.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gkgdrcnvy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gtrwfzfrg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gcywastdt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gabmedjqp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gctuvdfsu.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/grqntngmu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gicpivgfu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/ggeagtshd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/guotwarer.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/grdxeyuzs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/ggylycxaw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gazwupfcy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gxgxgyxkd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/glhxaeeqg.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gvtlvibqq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gjfzdihxg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gufemfuts.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gbxaqccvo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gbkjmzpkv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gjmqvywmb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gtdpaemdx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gllfxsjqf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gjvlknqth.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/ggbrtyeic.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/ghaqfbtnh.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbnthecit.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/grikvfimg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gaqgtefes.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gkyajlhin.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/ggwkaouzg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvewlcat.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guveldjyr.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/grhgrugdf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggtqtzewe.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gitjzvnrn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyieeqcys.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grjvsnbic.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gclbeqyuk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gppipyzos.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzdcnqkge.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gsnlscnke.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gyvjhnldp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/ghfnmscno.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwkbzvya.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gvrlefvgo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gfjcftrdi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gajvkqobm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gzbpqbxah.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gojkvemdo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gaczuwpfi.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/genjjjgve.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gqhpeitfm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gooaivcmc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gnamzlcfx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gemvfvmsw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gakfutztt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gabsvdlvp.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gdiugahub.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/goqiizacs.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gjoahsuvj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/guwmkbgjs.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmhragbxe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gfnoaxhqj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/glavrhuex.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/ggqpfxyrd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gihhvcahm.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxqyqswnn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gudhvdkge.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gxbqnorgg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtraslczq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gaxfaayki.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gilgbzpea.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwovnidxw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gbtiwydbd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gqihjfavj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaxktsubz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gntdmnihw.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gwqzpygqj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ghqjxyrhp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmuoxqumc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gtbzhrbxr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gxjyvwcdg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/glxvgzypx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gfcjicfng.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqzsqlcv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gqjcolhsd.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gnqebyzrl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gyphlctke.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gwfxlhbwr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gazkpwbjh.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gousbudxt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/glxqsftvh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gohngorma.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gvhnbsejd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gentjgaxh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gskvztwss.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gevpmgsrw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxyiigpsd.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gebwwymzu.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gfszjmbis.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzkptoh.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gegwglkct.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gbageqlhz.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/girbpkhkz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/giwrbldee.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gbmgnwmff.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gmhulpzie.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gqzoibmlm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gkcgqpmfo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gltgrdotm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqytiealv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqhohqvlx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gfhitwvxz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gipgmtjlq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/ggivxdftq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gzqlehfsh.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gyednnpwr.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/glaurndtd.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gmjyjmnsz.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gzbgmgcyt.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gjdzokyoy.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gadxeouzp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gdyohfbac.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/guvjoyaly.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmtjmjccm.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/ggklvkqhd.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gdqevlpjm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gujdvvzut.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gugppcewr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gejxzhndo.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gqapcjctz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gpmmjengk.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/goqerkbch.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gcrtdwmtp.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gkcqdhaxq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gqteuxdgz.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gcusgvzcr.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghdktawhi.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gzsqkvthx.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gwedsayhf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gluogvixd.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gsnvfixru.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gvhosgiba.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/ghbouresa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gpahssmgd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ggjqgppby.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gylanzueq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gojjkyslg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggofudfds.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gyurqidao.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gtoxuyhwx.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gptvlxgnw.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gcawjffua.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gcftsdogf.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gpupokrld.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gmltwljzr.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gdcxtkwmc.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/guioqpcyb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gsewznvve.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/guwwcwphm.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkkybktnr.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gfvqemkls.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gtwsobfqt.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gzbnpetgc.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gsncpzmip.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/giwjebvfk.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gianymmzc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gsojdyxil.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/guimddrmt.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gedcaekge.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gtjcicwwp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gwwwdbcyu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/giufccurf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/grfubvfeg.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gqsrsxbwn.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gvcfwifxq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gjccihuip.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gjyomlnkm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gbrfvwovt.sHtML


<!-- 参考信息 -->