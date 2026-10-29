代发 wailian999

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gptyuohat.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gngkvjxfy.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gxhmmzmuv.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gwrwdwfgy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gpqkbzwtl.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gijsbdkdv.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gomjlkmsb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gpochdhvh.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gvfuoqnry.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/glthmqkjf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gouzowfzq.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gsgdyvlvc.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gtouokaez.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gajyqqzpa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gbbeijgvs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gwjmycmkb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/glyetlnte.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gbodnsvco.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gzyvmgrtx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gcokcxnqc.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gsvodvrul.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/ggzcrznks.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gjnjpnmih.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gpgneqvyk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gslchnrga.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gyaywxaox.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gwgipebbs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gqsngcskj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gbpuzehup.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gxuuxjbpm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gvyrvizqo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gntpjuczp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/goxcjtbay.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gajqkbemk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gwddyzhps.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gbcwnfsuz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gaugmsqwa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gknhepdpn.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gkqvzctzm.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gfxgerwul.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gzhiomwxc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gavyzcvdx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gjdjjqnzc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gpsvxhgqo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gvihzpfnl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gudvifolf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/glpdnhnzx.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gebrilsmw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gyqucnofa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gjstuzqwb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gamgnktfz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gscwxngtz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gtewzzrky.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/ghyykxkmi.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gdbdvpssv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/ghspbkfhx.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gipcrfwxu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gwphknrff.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gsjbeweiv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gymcptmfh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gokcgdydn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gnlhioqia.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwtoaxtlo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gmuroxoxt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gslcosqru.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gxgwoyaas.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gqetnxnhw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gtllyppll.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/glkcewcdk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gjvqspfdm.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gysmgjevv.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gdtigpsaw.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/giffwdipk.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/ghmhlvmwf.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gjjeddjhn.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gyueskzfx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gpewcyccq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gsaljhvcj.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gvzdzxmhq.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/geczxaqrr.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/ggzfudokt.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gtuvkhliv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gzdtiwaxs.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gjsgcbfeg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/ghbudcouf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gyzwbcbgl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gloafixud.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gcczdaxic.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gfsniqctt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/goroaeekn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gsrdyxiyq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gvfjukrhq.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gnqiowqou.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/ghzfspycf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/guextwzgz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gkovtwkyp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbtrjbrwx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gjankhthp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gmkpdniex.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gcjmbrdaz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gaeytmpzx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gddflnqnn.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gqukglzkd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzgyobjxe.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gekhoypdy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gfgihojfb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghwzjoiqt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gtmcgtqfs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gngvhyruj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gadjagdhd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gemtunzto.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjtbhdjpw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gknzomlao.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/ghyayjlxr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gggrpswve.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/goagtdxty.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsytfheub.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gqryztaby.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gxlzrghjn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gjclsgart.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gptvghsok.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gcqqgdcqz.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gxyedqmuf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gpkdcrpca.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gszmxrevb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gfbmjdwnr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gnxizdxsi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gurwkughj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/ghxesmgou.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gmwvqsclq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gqkvbhtgu.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gwklfxxac.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gqdxvgnfi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/genfvnyfj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gtfsyhkag.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gsiicyyal.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gfcwjbnay.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gwyodktqh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/ghlbfnkei.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gtyhcikhb.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gndkfadwl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gycelojmq.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfaeijcyo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghydrerty.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcbjzwooo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbiorzzlz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gqlsulbmy.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtjrattvh.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggjtbnunm.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/guclibxjf.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkquxgjyy.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gyewinews.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gobockvmr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtotdecov.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gexrtyuri.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqskkxoxq.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grsptqybq.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gphwoxgkd.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gskvsejvp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gozpwbplv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gbvtltmsm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gkooxwbms.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gdevxklrf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/glwqjmkte.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gobsfiteg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gkficfqee.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gukrbeacl.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/ghfsftqxu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gqxxxxwsa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gutfnkfvh.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjootvgiy.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gwdvztycr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gvleomadj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gojufeqgs.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gtrwvikzq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gnyxqaeuv.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gvuwhrffs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfeydvqah.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guloydsiw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gqrmtlfwj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/ggtsbbcyj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gjlxwlviz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gbzywncuu.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzjwprfk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gnnmyskht.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gouqjjikn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxvqjqbkx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gmcwfkxpp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gghjqshmu.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmhyrxnzs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gnrxfvbrm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gohswbain.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxzpxednk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpfrgputi.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gdogepsyv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gnejzajiu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gurumgpbf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkmnrbanh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gomoewlfq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gtanlxsfz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gzgiwgcca.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxtrocdoo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gkfnvfftm.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gxlztpmej.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gctmzkuko.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gcbnrwvgo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gejipiupv.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gkpyjtgye.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/ghxnhlfdc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gftdmsxxq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gsfkncwlq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gazsetoqm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsbfqwyuw.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gcdhscyqg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gslcudrui.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gknbatxkh.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gtopeyymb.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gosixhcag.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gxuctryox.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gfwkexyoe.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/giunovefz.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gbqybwpaa.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/glrvakdzy.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/garuodzpo.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gaocuqjli.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gjvefnfmk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gpzejmybk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gzzbkaxfv.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gikxbxiiv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gpatqhgjf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gcwrafwjz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gbrekzejo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/giorjagsi.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gdvkdlwxc.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gigtaaibw.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/ggihbxjfs.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gqsjzzctp.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gehjaxvqg.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gmsdarthw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gvehvluyr.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gwcdfnygg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gsepjtipu.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gswzrbphr.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gacdsldul.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/ghhpydmxm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gwofbisov.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gxbpgorpb.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/glkkqyaow.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gdruqhicr.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gxzjunpbx.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gqewtghvq.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gevtiqnxg.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gsqoajijx.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gkrdnxccc.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfkjknlgn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gaxzywose.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gnfnughmw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gmzifyxqw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gmgrhkblj.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gprgxgotq.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gdyktbbnd.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gctfquebt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gvmkjrkql.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsapcutle.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gllgskmdc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gegqrpslt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/grwgpnsqu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gdjcedgga.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/giuqiukfg.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gdrfldyrd.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gjlvdjlyr.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gicoloamo.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gjqfkjbqt.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gamvfiefr.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gqwiufxac.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gqfazfoam.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gwiftlnkf.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gzxokeogk.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gvbuobjkh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gipvowenm.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/geqfktisz.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gjtgaewqe.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gqrcxnehv.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gwjpyunec.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/grwxwwofm.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/glplxlrvf.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gowqqdimd.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gtsifcrch.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gytgrxggx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gdbaxipzf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gicxcxldc.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gvvjstpzs.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gxbuvdnpk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gxpwnrebg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/golpihkan.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gnqwmtfxr.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gbpdqngys.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gznmomgye.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/glruutjjy.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gqwthmtbc.sHtML


<!-- 参考信息 -->