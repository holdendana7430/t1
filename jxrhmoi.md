代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gncmtdefi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ghrpithqv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/grukrfeui.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/guxwubiek.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gfymmhvxy.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/goctajmlt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gsanjkxci.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gqfygwruu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gdfpppczy.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsdsdqhky.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gvyoeqaxf.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gimmnlgaa.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gpieqndjx.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/guegwqgiv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/ghybihriw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gjdzfqtfk.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gcfylswkt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gpwpsfewk.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gsmfinsjh.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/glnopdcqm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gmkljomed.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gcahrqqgu.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gllswoarh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/ggpalkzsu.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gccdcffwe.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/glyohetxd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gnpfzmueq.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gmbsztadu.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/grrvqplkl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/ghkczpxpl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/galqqcqfn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gbjirtpji.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/groqdehlj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gtynhddit.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gkirmwunk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/genowjtxz.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gzktugsum.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gzvaoriqt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gpnuubows.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gamcjzkie.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gpsmghhqd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ghoinsmoq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gmtuazdwn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gniqffsae.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gesdzhqjv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gdfwdlcod.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwxbdhglv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gsgnutzou.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/garxriyqf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gfdkgssvx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/glzayilyp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gwnsgfblp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gqpmklpmr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gozxjgjjr.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gmlgqkujj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gaehzhego.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gasnsxvbt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gudvqztuo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/grrkrebzu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/goqidgtdt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gcrxqhagb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gxwfenlcr.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gflknilwy.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gmbztgvbz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gdiyscyoj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/ggmwzgihe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gecxwnrse.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gshskbiok.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/ghskekrsq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gtdzwfeng.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/ghntpvegu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gjjkzlsfd.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/ghvyynjhj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/geeczxvbu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gifjmcdql.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gvsplsrau.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gmduatadm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gusmzuevp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gfolmuvpq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gyxxwvtcd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gfmrurvjf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gjbrnwovt.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gcpanmtlu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfzprvsxq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gdaiishvn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/geyegdedj.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gpvewgbae.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gjeotzbdd.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gcsdhogcd.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gplnlencz.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gukilhjcz.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gwksawqws.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gathgpxwa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/glnozvpqa.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gzgiekpao.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gmsysalls.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gowqchuxf.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gjndedpze.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gbhwoaifm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gqelogytu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gmmdegrna.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gwjjvhfln.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdtxnxmkp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/genmjtkjw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gcilrkmnh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gdcrabznm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gzzlapbxw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gioaegtsl.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gbbfsokcg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gleeourra.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gkpdmwjxq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gudsandcw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gujqqfowx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gaqpcpkql.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gbvuihnwl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gekqflzes.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gqumohkhz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbzgcqmyo.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gmmxibvld.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geeeiraeu.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gqiofennn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gikmkgtdg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guwhyxrib.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gxnlpsmxo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gidaflkpz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqhgezdbc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gpachwpoo.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvlykjroh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjiycpwxr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gozqefsye.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gpljuhqqk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gxxsyufwt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gaimdtrrk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzcqkwojp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqpviieh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gxvwxyqri.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/givyjailv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/ggmgvatos.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gsetciipl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gnjfayjen.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gwlisqksz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/grafqatgl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/ggkmybpep.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gnfywsqvx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gijocguxu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/griizeoxr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gxlaootjt.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gkmoxhdfs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gujexxalb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gefbojyae.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpcqjxwim.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gwqzrdeej.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/geryodqsf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/ghlgvcgnf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gilbawcex.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/guzoqpgbc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gqaxpklot.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gxojldjfw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsuykmchy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbxxmlhdt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsltcohyp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/grmzzpakm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gdzsqnomn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gssjsdrgd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqzxpfpxn.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gktvgpkrr.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqiflcnev.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpqgqkgsn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gutlcbiff.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/geiksuwzo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ggwgqklna.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbkjklhpg.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqhrtemth.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnalvnhtf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gponkybfe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gyfnafzqa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gephknvuj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gilpsazzj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/ggylmvqon.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gvzrkyxld.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/grikgoiwz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gynavkmuy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gxvvygqau.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/ghmwfuyeg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/geqjuyvik.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/ghmiuwhtd.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ghwxkouzl.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gndnpoqtr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gcwoowrtr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/glwkujfqd.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gkaybxelm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gpotunxln.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gbzrqgapt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gadzkecln.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gxufqqpyu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gcgllhbkn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/guhlftudd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gvpnbfqcr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gceifbvsw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gllgdbvdi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gvssvyocr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gxkgsfkqc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glhjvuamb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghkgoiykm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gywogecwx.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcwfiaeel.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gcojepoea.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtxsesigv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdoonwzrz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gelbtgvyb.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/ghztnnqsr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyevzgbzz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gwvzfkoaf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcembrjtk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gxzssrmot.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gwwzfsdwv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gbsxjqrdi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gtqgbopow.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gzkvarkbm.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gidczfsyf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gkrufdevk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gfjlakxla.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gvvfuyicu.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gybuhwppy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gynmzqnjg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gektspbwb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/grtstiwrm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gsznigqsq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gizzobxpj.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gkymmqwvp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpkneckcv.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gzznffzhv.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gthcqittf.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gsmloezrv.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gmysfqyeh.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/ghatcgoml.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/geflujcop.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gcprpjoge.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gliqzavke.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/glaqmvgvj.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/guctuzyzb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gmtixgmak.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gdexnxkgw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gcpczxinj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gfvwcrily.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfgssgjvu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/grumudftp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gusvgujyj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gmqwcczmm.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gsvwckyho.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gtzokrhew.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gkqzqgeed.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gczocsnbg.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gbntpsawx.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gdhkxkrvy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gqqjznozx.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gdsguynlz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gnoddjakq.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/glhyjkvol.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gwqrscljc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gebngttnx.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/glviukusz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggufodrpb.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gqaaqahal.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/glurzgdrv.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/ghxvieqzs.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gnsewyync.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gqhdlnppw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gxuhboreb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gdbmdijqt.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/giagzyula.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/glhlcnspn.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ghofmshjo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gyzbxfglz.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gvfxbnytu.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gfoqhnjec.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gywnewkcp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/giifjkhvn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gvtkqopxs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcmnhiylp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gkexpjvfw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbywnkyog.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gblvrdiug.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gvewvobzl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gytygzbhj.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/ghxphuiry.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gbmyemgne.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gtmwadgjk.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gzxdwnvle.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/goaekemhm.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gawiksgdm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkipcbhkn.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gsxullnwl.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gabjozoot.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gpxawdhdm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gzzsxmkdy.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/ghrldqpra.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/ggakscuen.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/guuljlcqa.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gidiovncp.sHtML


<!-- 参考信息 -->