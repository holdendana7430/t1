代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gawtcwowf.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gnctiifna.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gmtmedglk.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gvkpavqms.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gbujtjhgs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gubqqpbjt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gdsypvgii.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gwlnfskjw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/glofntypq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gvaqtoipr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gafizhydw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ggvwwpvjy.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gioaylehm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gysjwjwzb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/ghbzqwrxj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/ghqsqpjkn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gtjjybfjq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gsnsxexgm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gxndrfsvo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/glqnrqnvi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gghqbgylp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gemkbskfr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gkyejtyqy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gwpqnwykt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gobnhnara.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gnwqicaan.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gycdtgkgu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/ggqhrurmm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/galgekbcx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/ggbqwidzq.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/grnvwnpuq.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/glejhyhwc.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gcrfqbhhm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gfrcyxzvl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/glqtsewdo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/goyjgzudf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gvgxunksw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gjwlvoejp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gnksoehdw.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/ghvrcdvyb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gbwcmiejz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gmmlwprut.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gpdreevgh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/grgiljnzg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gcyyjstzs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gmjwjjken.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhstgiz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gahnhqitq.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gojxwgxhf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gksuyulhp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gfgjmsahi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gfuyyxvoj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gicwutwen.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gzfvznjoh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gcrqnlcgo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gysgjsydi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gcyathvzv.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gjtmoaaci.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gzhzfnotm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gopeqhkks.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gyjlzdaor.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gjpvhucby.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gmwfddxwy.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/giiyfaiko.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gekdweolf.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gswtclkus.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/grjbuxgrw.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/grupsjhde.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gfxyivibm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gzocbiuse.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gmlifbxtc.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gidmppcpr.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gnghghcaa.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gmgtfsptt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gjicqeyxs.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gyumzoanz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gbmkctsip.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gpefwtigl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ggncbvvov.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gsbapvbtv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gtbwwwvsu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/giqzbuwkq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gchveukiz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gjlfhfydd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gawyrnkir.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gevjolvun.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gnysbslux.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjzuojftv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/ghzjmziem.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gnukelbvg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/ggmymdmqs.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gradwikqs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gybafqsoa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtaubhgtr.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gshihewcy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvowdtxkf.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gjlqiufrm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gburjvgyi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqieakdgs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/guymltmry.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gduylkphg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gjixcofid.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gqbwlwyxw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbwxebpxr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggmxcyszf.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/grsrejdwy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gqskucude.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ggstxtaoy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gjtzdwrxh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gtzkixnul.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gasuxynxh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gmfkxdnnx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gyviaoxsn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gkwwiydjk.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gzprmqmmf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gqfrbcccw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gygqxrcnt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gtjrasgzu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/glnagnryk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gfiamgfqw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gmrkihitp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/grsxbpcvd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gbjwbrcmj.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gtszfniek.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gnoyplqbm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gsgddevjf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/ggvtmrsgf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/grqegkvjq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gizdsjotp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gnixipnew.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gunlxjvsq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/grpgtzekq.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gfzuitmvq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gnitganmc.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpqlzhxsp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gesczatba.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geabxwzmg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gtvacrupy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gaowhqfao.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gftiubtul.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkwzhckib.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/glzyacmat.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbegenaqf.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/grdopcfca.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcvjtdxro.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjqadeqwh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gebegfrym.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gguybfsyt.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcntkexrs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtfhpfvqh.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gqdromksj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gdlhhozab.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/giyilnhew.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/guxplaplj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ggsupgktf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gwuwclmpn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gghcdmkko.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gkrjulqog.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gnnuzqamr.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gttcdbfdx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gnwytrqir.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gqzfcxrqr.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gcwjodaav.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gusoyijai.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gsbldjuix.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gqypmftwo.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gxycyjnnk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/ggpqxdamo.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gqhjulndd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqrvyknnq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grqualtlr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gzbjovaad.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gxzrectvn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gctysmoir.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gnveemnit.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggflztvag.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gxatsspru.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gyldvfayf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gfebinflr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/grnbjogxl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjllnhswj.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkhpnrshx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gjfewuhzp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvolrgtqk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grivmkqhr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmqneeevo.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gwardbntb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gbbsznzrs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/glvagoeth.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gpbbhkvmw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxaakasck.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gvgxswoiu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gbzwfjaig.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpmezbftv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gwefeyepl.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gxorbhkso.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gmtlzberx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gfpazigrt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gypmymrez.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gtrwfkssv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gktdgabzf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/goqjwifyu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gfvsslzrn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gpsrusrcj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvxyopbuy.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gfzfyxqkt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzsekmfig.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gsscwpnhd.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gyscasekz.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gvawllajs.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gsrncdjqg.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gdjplhsks.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/glnoiyxvn.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gcrzegetx.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpyvdmoch.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/ghkxhcqpc.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gspyogpbu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gignmddzg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gjjadzzwi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxzqlxtvr.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gbsypgloq.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ghpwkejqp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gthiegdgr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gwqpiqyiv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gdjsuohpb.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gpaubllku.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gummymdhf.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gogfplovq.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gjnignlhf.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gvuowoqyr.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gtvszmach.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gtboacjok.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gptfbscde.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gfdcoazqp.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/ghpcvwfjk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gonzqflao.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gpylcnjye.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gwrhexbrw.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gklgtzvwt.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gciknfsxp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ggdcmeojx.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gznkzompq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/ghevwakvd.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gsiyzswjn.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gxrnhgujg.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gshlrtugh.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/grgmkwqep.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gpjmhstjt.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gvcwbiuvo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gvcsnpota.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gszxsfxgh.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gzxduktyd.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/guyevsiuh.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gcjnjvcxf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjaevnsg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ghyyihkou.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gbbpivpwg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gzozknvwo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/glimuduov.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gehlocvmu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gwxtguuum.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gyiohlqwt.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gymxkilio.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gnuxmgltk.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gfynyagae.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gqnokzmpg.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gomucftds.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gggotwuhl.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gypkorgfa.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gkybqyyfp.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gtwtrzwpa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/ggtlfyqwn.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gpcbhehth.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gmrjiknse.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gmikbblld.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gjgvihvgl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/grzxmryjq.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gpomnrbfm.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/grrhvbraz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gqdvuykrm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gcbtrlyvp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gcazvdull.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gjvqgdlsp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gmqpnyspz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkzvuqihz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gwpvvlpcm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gsjhejyfv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmlaarmbe.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gvrdtbpnb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gixkojpcn.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/guoupqkzd.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gzwsiyoda.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gehiyfbyr.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/ggaqjmnue.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gulvroaih.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gctmfhzwi.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gumgwagio.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gklpzpzwd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gdqvyywna.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gzbrfducg.sHtML


<!-- 参考信息 -->