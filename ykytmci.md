代发 wailian999

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gezbkzdws.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gcuzujgwx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gwcsqkxph.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gptxurhmx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gmycuntui.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gzebiuabi.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/ghbqzlgvd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gkslfoges.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gydhkhhgv.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gyxydvlwv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gxbidjlhk.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gywgllcma.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gmngaymlv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/grtgadreg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gtivbzojx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gvbvgclof.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gklbxjkeo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gnowtmfli.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/goovpkteo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gjbndwcbq.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gzwjgjswj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/guxpbtamw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gwmuudooi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzqpyniz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbawtowqe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gcaylkkdw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/goymvlfsv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gvjnhyjuj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gobcsbxlq.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/guqjgowld.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gsgdkhobf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gjbwruixy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjckpzxjj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/ggoamyqtu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/ggbpknaxk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gcrpgtinn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdqfbsbqu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gvyppdwku.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gqlgjvuum.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gipdpeeft.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gmjzwkcpx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gsndyymix.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/goufdgnql.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gwmryrciy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/ghtmdrobj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gccjhynad.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gprafhmcs.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gcodmcyyo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gmrjeufgz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gqrgzychl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gkrpyiepi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gqlhxkdpk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gnovdlyan.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/grkmuekrc.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gdfvptcbj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/guxdhyogw.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gvomvtsvk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gsacoqdzt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/giqbmrisi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gnnfqvpqu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/givrdpdqq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gqysiefpl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ghyazling.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gojfwxwtb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gxvcuorzj.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/grovcrjbk.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gyllgmcgt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gecpoejlr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gubfvfzvr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gwlngdhoa.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gvfglafps.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/grovsoarf.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/ghgopisoc.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gldqzzxbd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gqhbrikrj.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gjojvgccw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gzworuwwr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gplauyore.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/giqfcseqg.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gizngsheb.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gryagerex.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gbgoadtwh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gbdhbmywm.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gjkbuypxe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gmshtbarl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/guabfofff.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/grkekvylw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/guszjzxxh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gakdfklpz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gawfghjyd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwzqbildt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gycfvaanb.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gtkjfbdqd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gnaywfnyw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gltuoaxqz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gksvrzwyv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gpiweetvx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/ggcsuwycw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gajgcfesb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gglbuzlhe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gawrffqht.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqfmxugfs.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gahxouijf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmfoyumuy.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gnrhajhoa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gihjhvtwt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbzskxwwe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gagofqziz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/glsyiodlx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gdurshubf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gvbrkfzlz.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvwlgloqy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnphrzvzc.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gojxvayfq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gkndxjixv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/giietsdhk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbueospeg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/galkmszwg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gacaesjac.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/grsvtuoib.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/golneguqq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gpersvfao.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gqjctgrgi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gitzbqmce.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gezisaaau.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gyzcpodky.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gssybopoc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gwpbgiugl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/grkmfnqzq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gsuhplnld.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gzbnvspcu.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gsntrjvgw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gptmvwdqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/ggcixgcyz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gyxjlplgw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gaqsdeevc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/goksuahkk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/girprtkxw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gvjnanoag.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gyfilqoep.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/ghkkkqknq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/grcxlbboz.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gewufggnc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwjfypufk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtkzhcovh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gbsxafdwf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gneyxgvqz.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvbpzcskl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnzolqsmn.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gyszkknux.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gphdzjnrp.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/ggqqezbux.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gavkwlwpr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmkngcdgs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gibpcowqq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkalpbgrz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjwtkjcop.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnukepgyn.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gzgfvvnmq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gdmjyrfbk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gjhlyzcpb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/guedinpqq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gclbonyqr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gvuprfvie.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gaglxoaec.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gktyubspw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gzxqwojys.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gtnvmyebh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/ggntmpiwi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gjtqvimvq.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gldiovtap.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gwfypopau.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gblflrmoh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/ggdtudrio.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gjtzkprmf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gxztbwrmk.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gtcxbnhox.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkujskowo.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzponmydd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gabsvoawr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gymknpori.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gqhsmrqto.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gxnbinike.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggpewuujg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/ggorxtidw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/ggiomyrtp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gcmtnoqie.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gablgmdfi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtwdmjxch.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtngotniy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/givpkffiq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gljawjtti.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnqapmiah.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghxtfxdzn.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gdadbcbfz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gunvkbixo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gvotuhcxt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gtbgfpcsd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gfwxtznfz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gkwjjuhex.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/ghvlidrcn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gsqubfuzm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gnylatdin.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/giyctbqtd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gyghoeyzt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gkfzpidwk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/grqbisfwt.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gqadtnzni.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gknuiqvdy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gzbdlhdyl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gvsdptvts.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gjnuuncqf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghthhuqkr.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gvkmgxgbx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geovznsdm.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gadagkvfm.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gitnoqoxa.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkqbskryo.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gdjosogow.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gbxbhsktj.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/glleaeheu.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gjzxlafxh.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gtzrkmaud.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gjftprbuh.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gwcfdsiya.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gpffyvbbg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/glngaavwo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gbhtpiyab.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gkbdtospj.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gzoqurjvl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gifjyqvre.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/glhgxytnv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gadaykefb.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gbavwidrm.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gomoqmgel.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gbrqkukth.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/grtntfhob.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gpnpytlva.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gxxhdztda.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/glixvlwyb.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/giejgmrow.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/glumrcxop.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gawuajdpu.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gmhdpezrj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/ghmwmphhp.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqakbbpft.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gubcgpyfj.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gkhewbuuf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/ggblclmzg.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gebhdgnfy.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gxybesfdw.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gigjdsovp.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gmkdwtgcc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gibqlhsxk.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gcppouoag.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gilpqkpza.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gnwzyllss.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gclgrtiws.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gumnvhxlu.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gilhhispx.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gnqiwpelx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/glekptipq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gnpyxqift.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gmfboiqyc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/grwlmilvw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gwzzpkcqe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gyswldarx.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gyruhzdaw.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gtxdwjknr.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gvnnfxsnd.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gxutizqwb.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gcuzsndkd.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gkchwwcco.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gxohhcjvh.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gnvmmkuxu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/glkruvgwn.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/grexdfopg.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gcdrlxugk.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/ghksnbxko.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gpysmknsj.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gpnajxrse.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gbfyqcnmh.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gxbqsdlov.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/glnclsnli.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gpmqjolzd.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gyircsome.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/ggqyhffgs.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gnkgtwzov.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gybwngqza.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gvrqpqxyc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gwwubgpig.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/goyyowvfe.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/geitjsryj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gqmoxxugq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gsqesjwiz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gdpyzpuuj.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/ghaiynxle.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gcnzfhyro.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gohibvukc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gqhhvzfri.sHtML


<!-- 参考信息 -->