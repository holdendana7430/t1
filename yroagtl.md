代发 wailian999

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gsyanjlgu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gnwiortet.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gktdlsqix.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghaxcgjbk.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/ghwtuaxei.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gmhfsutec.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gqhhfxchh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gnfxudunh.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gabpayfoi.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gwgzonora.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gezzqzoov.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/geuonvbag.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/ggkfjumud.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjpkprgt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gsztgntfs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/giitrcbhd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gibmttdtl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gatyxtxeo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gcfuencoh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gtwbzvrsh.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gxmuypaxk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gboiotdxb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gjnxhwmdp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gktonzhoz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gimchyylz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/glophohku.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gcilibhhx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/guydinqxg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gfxuniyzc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gqusqkqku.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gxpalbcpz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gbmapokzh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gmszvvcpn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gbubxkjcx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gbwbqxefq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gioeipvgs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/glnfvzdmm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gqrqrkhis.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gmnqqdzuu.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gmkuhibmv.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gxkcariza.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gpxkoiyes.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gwsygnlio.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gifllknva.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gzlzthulo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gtrphiayv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gtafymwjn.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gnlkwmzlv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gmsqdohjm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gqhieiurz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gxjctxgzn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnidkkkwl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gbpayjiqc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gfczmbzho.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gnuxtcdze.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gjoohgxth.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/guglwvhbx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/glweeihgx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/ggbsznrjs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gvriaclsh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gjecljbpr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvwfazkh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gywedvjck.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gqpsxuyrj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gnethjlnl.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/grhgohlin.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gwexurcpk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gktvqswgl.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gfpsqgqfk.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gvcpbuwpe.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gjmcpapui.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gxrspwryq.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gyeghnvun.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gvvyxpuvn.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gdmvmdkea.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gbuhnucnu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gutoduprd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gckzznuif.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gooyjrmeb.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gcdydeqkk.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gqxmdzubk.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gyxzstgnv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gtddwkeni.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/ggxuydaha.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/giqspcpzg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/giyerpyed.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gospsntvx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpzbndfjz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfbjlyjvw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gvdbsdluv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gnyhkzpxa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gpglbmxfz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gqppomsmy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gtlaipcfj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/guarfvsbm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/guraeyhqx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/greusulki.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gllndlosx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gfjdeuknb.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gudjotkbt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gfdytwoah.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbguhalzc.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gjrauiwhj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyslchenl.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gbhhydlpl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gwumdfrbr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/grxhehebr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gmzjzzxbs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gkbjpbjnv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkmnacejk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/ghullgjbj.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gacwtekma.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gplhhfitq.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gibsvsxkw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gulydopmk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gsdmstloc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gdskxnfnu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gacdzgtrf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gwwkjgcdl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gvxrjmhip.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/goqhkxyfp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gheyejoke.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/guowkofbk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gkmifntai.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/ghyzloxjl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gkxyvbszk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbmsvpdx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gszojgirc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gbglqoxms.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gedbcqwwu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gfluslktd.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gbnxwcrlb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gdoaevffc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/grdcojqhl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gyogsljop.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gljrsdonr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gimwcivxc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gwzyrpihl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gzruebflp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gkthqyamn.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gnksblili.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gqtqxfjmt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmgdslnlf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/geierhapw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gelhjaqog.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/glkhmgpby.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gxsiyhvjv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gorsxhoox.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghfexqhzr.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gizaenhgo.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxmcnyqft.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjkkpuftj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmdewayfp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjlehumoz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gzwtjwatv.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gurvbojag.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvgaufgnb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfojlfwcm.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gjjlqglmy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/griykphjj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gmqynnrva.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/ghaxqbmrk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ghxcdoyhl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gqbyyhewl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpzspnii.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gqzyskgng.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gafppxunz.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gtbihljxd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gnjwiqweo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gjcppgmvx.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gffdplmjm.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gtzhlfksy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gxxcozwue.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gtimluvfp.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gvbmlwnpj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gxvkuuluj.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gfjavdrzj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzoetmqdu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtblkjvec.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gioetfeie.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gsqmwmzlh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gqfmkbfne.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gkixwaiwm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyfeeawpd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gfoasnfbm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gvslukorz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gijjyjdpm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkneswqye.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/guyezxocn.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdsiykfoo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gsvmbucby.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxvtoyvoh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqshwpauv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gboxnqudt.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gugefridn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxqtbrdj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvdtikkcq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmmoxuecv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gtahhyrdn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gotbnpbmv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/glatnawbc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpdhqjcpr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/glpwyinrl.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gnsuicjdr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gtqenruqe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/ghvxmwnpv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gvzovrjnc.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gfgjiunpi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gqakbrtiw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/ghjgfjmmn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gxezxhuia.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/guxiwmwdp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaummzkfs.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gxkkvckno.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gguulmlcs.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gnjhdcwrv.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gaxuxowfj.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gaflbqagn.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/glinbfyxr.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gebfaicne.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gtlfafwuf.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvkdtpmu.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gtnfacuna.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gbknhbxfs.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gitpdntym.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gpcfbkwcc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gnnxaanol.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glylwurpy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/goxzhpesf.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gnnncebjj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gcybnqugq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gmersgeje.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gvgoeawdj.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gpqfkjzqu.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gmhpsasnj.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gkfdmusvy.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gmyydxtbb.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/glzkrqdgc.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gpljwsxqv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gljuttfox.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gsnlavhdv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gccaxxusq.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gxuyaxcev.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/guqtbgjrf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gsofdusvp.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gdycbkjtw.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gosegtktv.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gmqseounc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gcuqgkznq.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gdfwfmmoa.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gqirbwiiu.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gqmlocvoc.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gsppqueln.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gsadexuvk.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/goruljvmm.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gcklbdqdt.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gazutltaw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gxnscpxky.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gnlwadwur.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gtbvgdevn.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gwuvubdbm.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gnkfehocp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gcnyyklgu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gzarlfyzi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gtbbtviqk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gguuvsdfy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/guvbrsyya.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gzakxmzcq.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gfkqzqulu.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gwpcvrjqx.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gkraoypsv.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/grlwgzxzy.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ganvkbcjt.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gmbtxkjuz.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/guqrshfwg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gtxvrdebi.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gucfhysgo.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ggjhkbjxg.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/ggdgflwgc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gsjybcxyg.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/genpqmhsd.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gjeklbtjx.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gkbibmdly.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gwyfndujb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gajmafazr.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/ggmblrgns.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gomxkpkcj.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gaspmhwzv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gkzdxyaoh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbnoyxlh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gmvobscro.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gcibooyxg.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gkwoapywy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwsdjmg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gmjztqhgu.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gtlmlvysg.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/guwgjvjnl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/ggzatlaao.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gazlfqxty.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/ghrzzahey.sHtML


<!-- 参考信息 -->