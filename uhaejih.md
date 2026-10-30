代发 wailian999

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gpaztdqqa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gomfercrp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gvzvfdewl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gvykbslgf.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/ghtgddjin.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/glcwozofz.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gobjcmapo.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gbgtppkjy.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gqokbmsmj.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/grqrjamba.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gsxguvhmk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gxwepniop.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/grxkxfvqk.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ghcfimvxq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/ghbouywpj.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gcmewddjn.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gbzfxonln.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gwylgudyo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ghabwizth.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gqpriacvc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gnctbjruu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/geveijdvr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gtdlifvej.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gxkbfwboo.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gbszmphdb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gsocsgpgh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/garbljsdz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gogvpiwwn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gprqrbxkn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gtiodurtv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gtmnrejsg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gdfbzlhxl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gqncgidxq.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gbuyczvuo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gejmxrsak.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gpqedrnno.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grbkpbtbp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/ggqwzlcjy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/ggdejhjjp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gqpafyrth.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gaydbffud.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjdtuujga.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gtkxbcwwu.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gdaafuqzo.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gqdhdirvp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gdyppcqox.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gegrgcgdf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gtyturluj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gmbetjimg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gsurtgqvl.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gptjygeun.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gbkqlvolz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gapyrnqwd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gnipgmkpt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gngtxbznp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gehqokjkp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gxrwfyrlx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gkdaxctqf.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/glqrlyrba.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gbkubufgm.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gnwttrjbp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gvximegmc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gajzhoglz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/ggrxlilzo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gazevhxul.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gzalugglc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gnnjlxtih.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gqdzkhlee.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gkobvdzxf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gxcntqdvi.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/guxkikenx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxufgmblp.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/guvxmakls.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gffjunsud.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gmhxwxkky.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gmyphiqbw.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/geoeuzeku.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/geiaysphf.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gstyaqkxx.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/ganfqxcdt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gddhqnrfe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gmcsidqbg.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gasnxsklz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggovtzsny.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gxtmxqxvd.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gqeovjzyh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gqkoxglwx.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/giudzlsnk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gykznpcnj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtotsdxbu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/ggsjwjlcl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gedymcrsp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gjczyqewk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gnhcimoaq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/goowxttyj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gadmsfwvy.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gjlpzhjnd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gqwccmirf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvfpiduic.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/glvlraflb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gvmzdocct.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gwvyckavt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gparjvxwm.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gpstpalli.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gtnjecjkt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grlwotmfq.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/grrkidmyd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpsvdjcxk.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gxyppknsc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gvynagkaq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwdvkifjc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gjttebjly.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gmiewcqxx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gibmncsio.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gxmyjgqvo.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/grynroxuo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmxmplrpr.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gglqbjnyc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gbovcaudw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxngtrlf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gmzwogvhw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gtleivkqi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gcyctzljm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gzcexvpvj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gytzkqqws.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gebaixlja.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gssmitisx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/ggpfrdvzr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gnpoancjb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gejnjszjj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gedxuokmn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gjxtfzkpj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/giwoxzozl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqbujpwa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gebpoyjiz.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/godsccopj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gzgdecoza.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gtazobbgz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/guwyhvlas.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gsxhtonxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/grimstjbj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gyqxmgjnu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/griiszljs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/ggiqnaqep.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/ggxnpbrlj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gxskppamx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpjsxrwlw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gphfpdxvw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gaxepqtkw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gafkvyaip.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gttrpiibk.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdpzkihcj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzzwqakxt.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gznjtytsr.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtdnujuwk.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gajvpebzz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxdibkxfp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gudsiruys.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gewxrbnri.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gukgvuoai.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggyaxkwqf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqsgaorkh.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/ghtfjydzj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/goedlzquz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gbuxeijxt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gnzbtvptn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gbyzwsbml.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gtsnfantw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gbvwywogc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gnzvbbfmd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/ggqgpqejt.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gyuirtwaz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/guwpqtgon.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqxjgxcw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtyhvaxfo.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gwxlyyjac.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gprecrjhl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gjiqvufgq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gczaxeusw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gvujadtqr.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gfjrttmta.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqspeokqm.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwrmxrhei.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/glxssxlpp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gifkmhzkw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gtpqcxmsn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gnmhogets.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwqkxtmox.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/ghhdamzuh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gmjlegwbi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmecvahps.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/givhybqrg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyjxncihn.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gycxszqav.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gtkkkxgzy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjuvjfvou.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzuleaszn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gczcmwrbm.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gzjsafxbr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/guadslzei.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/ghffctrzw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/glimsobpr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gvgtizwym.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrczswuw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gsjvtzjnx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gpozcyyqm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gswtwolmx.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gxilnbgzh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/goulqrfks.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gstoejems.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/giicpcpuf.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gcbxnenmf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gxwamybki.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gdzzoscmm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gkbwafzcq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gpvmijnbo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gznwabozo.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gcapxlidj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtoaeouoe.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gplnypzza.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gvnpvbalq.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gerzgokcf.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gihvfahwy.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gmkphsuac.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gtwkdskvo.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gljpsxygr.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gwgxidmih.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gidmbihxs.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gfolygjmx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gpetpzado.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gvnwkpwmr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gvrmewjia.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/guhhsiuuy.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gmoftuqnu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gblzauqda.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gzkpcaunm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gjwlcmpuz.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gtrzbofjy.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gubqdchmz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gktmipkaa.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gyctjesgg.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gnqglxrfj.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/glkeriqcm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/giikdmhig.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gbzmlrbfd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxfsrlpkm.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gotmjukra.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gtbklelms.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gwtamnfma.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkchvmemz.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gfliwlkfb.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtaegmwyd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gehwjvtxl.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gdsdciduq.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gljtietea.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gvlesifcy.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gszmokrci.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gzvpyhkgd.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gvukceede.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwfozxjri.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/giqofuinn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gffnsrphz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gwirajgjw.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gzyowjgpm.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gubbwqwlt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/ghigzpecl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gfotneiiv.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gogwnlrgc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gsduwrmzy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glkcenmga.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gnymdaclv.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/goqytgiyo.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gsdcqnlbb.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gzcneysjs.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/garvygqny.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gzuspmury.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gbpvqbvyc.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gpwurufqy.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/garvoarnw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gzuelbcoj.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gvbcdafzs.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcafuijcv.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gomnbfmcl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gifrcdmut.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/ggrorrugs.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gkmgxgaiu.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gclfjyrtm.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/ghfwjsocv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/ggsckbrdt.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gdrvrkozb.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/ggqbzozwg.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gnnjldjqk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gqlxafncq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gudnhycxh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gjiyiopwi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gmahvfilu.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gsnapggkj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gesnnojil.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gppghgbdl.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gwznlkkdy.sHtML


<!-- 参考信息 -->