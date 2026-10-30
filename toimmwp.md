代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/grpepqgfu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtlmizsgy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gvizfdmyn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gnambpbdm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gmztgwoee.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gnklypgoh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gikfruokj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gtffalbpo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gfyfsprdl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gwnjdozik.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/glsnhjprj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gipwwcjfh.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gzoqciiea.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gzceqpsij.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gfnwqudwn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gdlxnnnxb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gokmvvfce.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gpsoelwql.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gyseuhctw.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdxslwhbx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxpfnkaub.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpgcsikza.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gtvbpjfpa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gqhsrhkrx.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gnrgmugzt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gbsxwpnsj.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gnidfluok.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gzeadmtdv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/grbluxngn.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gijxpafvr.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gwutluqwd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/glaguhyxg.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gordfgewr.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gecocqukf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/ghvnrkyvo.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gvaegdbbd.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gfilcjsol.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/giinafxwt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gjjfagiqm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/glkkftfkk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gijrejaem.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/grwedfioy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gejbqfrah.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gvafrphid.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/giicujoqg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/geajkgvbn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/guzcilrmf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gxvifdtyz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjwksqojf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gdulmhdir.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/givdpopta.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gvrqngobt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gbyelyezz.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gshxbngzv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gyprekeko.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gztpvzgfj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gmtcebaoj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gtxmxfsfl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gisisohhg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gkjczlyhx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gdrvdzmbw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gguulatht.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gqrrwoymk.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gpzwgeejp.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gjdetocxt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gyuzbjolc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gtxvdfnzd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gbewgpscy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gsbymqotg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/geplnwhgq.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gsyvuhjhy.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/grpnzgyfr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gstnufvzt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gwieeuqvm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gydggvhjp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gtgoaazdm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gghfltvyf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gcpdnygci.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gvfpifjit.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gstldkqxt.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/guyudvnid.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gymwpfgmz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gievreudk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ggdcerycr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gfctfcoky.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gulshbwzy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/grsjiayph.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gdehakuti.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gzilqlwqh.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gwplvyuwj.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gqwvqlxmj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gzrqikybj.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gfblbiqwp.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/ggbgoubsg.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gscebbtjx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gooydpvxz.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gjhyubtcl.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gttlhgflc.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gskodcpih.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gbiqkdpfv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gnvrayhml.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbsldjavq.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gvuxfhsor.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/ghwfqwovv.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gecnldmyx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gqljfztgd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gfjmpwsle.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gkcfnxuov.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gmynhswst.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gbrdgvbdd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gjjgesksx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/geezjswlq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gzbykxqtd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gugsmqvmj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gashgfpdu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbfljkhxn.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gcvqxtqrz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/giobnavos.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfknfrsaw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/geamdyfrd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gfzruodyl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gjfdzcxuh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/guwpkfjek.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/grtbakhpu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gtqylwwdy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gowxwtqdx.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/ghkxtwcgi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghccijpex.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/ggqricxnh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gcljixcyo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghigrsacx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gdrjupwna.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gfwbxsird.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gvonjphek.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/ggznijqzw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjrqkmjfw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbxgmnpap.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gflqhhacw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/geugfvaqz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gcjzarbkk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gssicoksn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gmquqoxxx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gsyhowaap.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gdalfgvth.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/glxthjhca.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gjvdrjrtt.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/grtmvqcyi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gxirxznwq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gtlbzqlsm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gsknwwdpi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gkoswvimf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/ghrrlmniy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/ggjnadvxc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/geksejiou.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gydsqvvfj.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gpbzinaij.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gmtkrabpz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gwihbtpah.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gropolzhm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gndbtkvdk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gzomknccm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/grcpfwtqk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gezklkidi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gogcwcvyd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gcucmdchj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gckhibuwk.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkdjliyih.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grrmcvwpf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/guxtpjkri.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvuuorizw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gragmoqas.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/godjmcofw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqhimolxe.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gnivojupl.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsgdtqdsv.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbmozhmrh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvczjteim.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gaiegkkpb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gwsxhofcf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goyggbvjs.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzexdyygm.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvdexfmug.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gmykizqhp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/grzqmioqo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gnshjuglo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gmvlfqnjq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gauxxlpgp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gisoywnhr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gkgncjwdj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gpghsvrtj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gtgjraokr.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gblcdsxfn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gzzvvehvk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gvvxqwetm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gbgdtqqxu.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gdfcnyfpn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gimcxsknn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmpmpucef.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gihmyoghz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gcuupkihb.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gsjkegcti.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gehfrtbxe.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghbqmojow.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gjllalbwm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/grkgxktet.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/glognfytb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gcsmajraz.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqenfaltu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/grffcwfxv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gecnaybzf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnpieswbj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/glfipbghi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ghoepewuk.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glbbtduig.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gkrxccbsy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnsjmlbky.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghhkdlcjw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkvejooop.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gvitkdktl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gmxbegwbq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/grglenwrp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gojslidta.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gwnvjvxgs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/golmhfttd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/genbaxzfa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/geqmogall.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gkrysmcll.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gpeiczumj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gyhnmurmv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gyxdabmad.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gpvllklwi.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gkgiqnegg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gglqhryoq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gmialuxer.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gvserdwgs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gtfsqrujw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghqpiejyt.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gcpqszika.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxqegytut.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gxekopqps.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gbedtenod.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gcervrwgt.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gxbrbptmg.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gzlamdago.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/ggzdktqzy.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gbodfbuaj.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gdaoynhmr.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gwqkmdwpa.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gangubpfz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/guzkbhdgr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gnxuvndfc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gszzlxygz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gduxzapal.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/getinrcmn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/glsltbqgc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gqjbwghqy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gmektzwhd.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gipnztnfy.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gvquytmby.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gzuvjzgws.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gtqojsvgx.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gwwzkhrha.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gexztdffk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gvkcawlkh.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/grkuxejcw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gyvjqfejc.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gexkvdhvw.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/grlhbkgqw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gexgleccb.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gacdkgxhn.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gsjuakygn.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gseiorrjl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwuttrffh.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/garrmkjgi.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gfqccrouy.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gynoesacs.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/ggvfuqsvo.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvneddolb.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjuafjfof.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdyfqcryo.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gaktldiic.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gcvbishjl.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gddftskrc.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/guieffukj.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gwmppvquj.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gyxqzqovl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/geacwkflo.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmbduqezu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/ghumerlxr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/geitrkgij.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/glmndjpsk.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gwafuqcpd.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gjovrbnbj.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gixtfyuzw.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gitrjwrrn.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gpizopjrx.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gomvpzkvm.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gkvtclmqs.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gsuwfdqzf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gqmluzhrn.sHtML


<!-- 参考信息 -->