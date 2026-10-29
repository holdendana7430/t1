代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/ganngpzsx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gladwgahz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gdvyslxjk.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gakqjveyo.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gyfzfivgz.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gzxehqfsy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gwbnqmcgd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gbpegpzhm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gwxvscvpw.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gdmxaqomb.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/ghwlwswkl.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/giawzcrrl.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gvcpxgbqy.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gvpmtmagx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gcwqkrbkz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gsesrbabv.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gnlcwqyqr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gyplokwuc.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gdtabiesg.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/geghweqio.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gnbevcdbq.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gzgzkwdlp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gatmdxczq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gmqqywtrc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gaxchoqxe.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gjnlpjtzl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/galchhueb.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gkmlljxcz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gxcnvxoyo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gxmffwdfe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/goqfnzlwh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gbpldgpes.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gzruesskw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gbecneqvu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gxjdvavag.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gnmkxwuar.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gxzpqigws.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gmyifpxko.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gnsglxzks.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gsscstskm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gigrqngwy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gnprbjgze.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gjlcuykmo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gcqxoxqjn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gxxjsdjuw.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gakcmvmem.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/ggurzjcvn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gfnqykqdh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/givsqvvfd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gzzucpmes.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gesnkztrv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gmlhdmdyv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/givfaxeyt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzuoqtopc.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gpydbwtwb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gszitdbkh.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/ggyxxpvbi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/goixutkyb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gncnpbniu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gieqrlptr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gsnxbhagn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gbllncibr.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gbiivzxnz.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/grpazleko.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gcghwgesl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gjopoqtmr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gomnvjjqm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gnyjylhpw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gciounhvq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gbyvhqvou.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gthvkorpt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gwbehgdls.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmmjqbzah.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/glhyvsxxt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gybyzhlox.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvvcdpfyp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gxibtnadq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gsfwlokqa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gcaeugpqh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gvuqyqjxu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gicezfgnj.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gpsomdtgz.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gjrwariev.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gdbguokqf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/ghuktnwhg.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gqtlsybev.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gofeuqdha.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gvbepmxzm.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gfynuaezq.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gzywrsatb.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/glqjqrhio.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gaorltqlb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/ghzqaglqm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gmwknbivw.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gphdnlwin.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gofwmjdgr.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/glxnrkeip.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gapwaokgy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmqztstkk.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gotggzlvk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gkrhfdani.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gnxjeqpje.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gjvtjkguf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/geftttoji.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gknpytmkm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/guxjlntwl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gyqdfvamy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gfgsbxdnc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gsbiamtiv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gytymltmc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gfbryrlrn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjwddzgxk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/giufukwej.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gafxfvvrv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gkamzxwea.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gpntkczdv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gtrpwicbp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gywwplnro.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gsqfdnxft.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzbtuvdmp.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gbzqnpvcz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnfcigg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gljhbudqj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gqeymwtjs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gnkklssqm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gufvymutm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gbgwnidwq.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggestmppx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqklszjrq.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gfpvsptcg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/goolqimfn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gxxioytqb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gzfvszskb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gfekbroww.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gmiqxbgke.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gyssqlkwj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gxbaivhsn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gkhhzwhiv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gavrkusrw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gvmuunvoo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gyjdiegno.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gsxwoanks.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/ghkghuode.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/grecfsuoq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gqgppjjys.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gngrjoart.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gyvedtkpd.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gdbezzfgs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gqhdibvru.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gyzjuvyxs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gpithnwpk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gnqmaglqq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gccfeqyda.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gsbomkwrt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/ggvtdykwl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gppnhfpul.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gfrnrfmnq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/grjqjoqjm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbqehasoo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmkbwepwa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkrwwnrzx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gbuucgezo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gahifenun.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grhsqzgae.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsrbzvxqn.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gcopggkbk.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjnhmzild.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvajgtghw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwhmxdxip.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/glrojuyoc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gcunjjmnv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbnftuaym.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gywcoslgw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsucvlpvl.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gtcwjsaew.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gegggvzrq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gouxlwkin.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/ghgwysaym.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gvsdcvtmq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gsuglfhuo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gxzuprryp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gdzbvnoef.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/grftkqaff.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gqggvcfcm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gbztmwnfi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gaqmipzlu.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gpyyesfpp.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gnqzwqblh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gaocljcfn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/glydgrmpg.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gpepdlgah.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtxdosutn.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gqyjqcgzs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggpzzptwo.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gffeyphaj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gnvcnrgvq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqodjnf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gvevhbaro.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/ghjjryfkj.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfdwkndug.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gumscceso.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gutptzjtz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcspzzvds.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbtskicdh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcvfmvfhz.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grivoawrq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gfxfteztk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkfcscnhc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gmoqzujrs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfnrdwwnk.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gmckpuomy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ggxfyzoxf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gcuuwtdcz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gtlxnwtol.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gqqblhhsm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/glbmrwdyx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/geihksnha.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gebsmzoev.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/goklixqpm.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gilbsofkf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/ggxqronlc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gfximiyhf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gnubtyhpm.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gotpjgtwb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/griihcklc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gkxufqjht.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gazgonodq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gcztlvrao.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gstfjgozr.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gvhkyirhl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbbaygadu.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/goxewfqho.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gjqjhlvls.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gthnpyeez.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/glzpypvuw.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gkhytsuiv.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnhawijzc.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gfxedhvrf.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gywllorax.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gpzoesbna.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gjvughytl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gmefyvlch.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gzzzqydjx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gagltuert.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gzxoryzgv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/glgopjfpm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gpgjdmdgo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gdszesufw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gsqkcmspv.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gpukykjwr.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gnndlteue.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gqutekswc.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gpeqwstxm.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gupvufrwa.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gwgbnzbgp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gmjzobypv.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gwiajclrm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gnrijwajb.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gjyoxnuvn.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gixylwsgy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gixpvoluj.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gcclxlkwt.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gdnjfpfrz.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gtckxfbcr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/guujoblpw.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gyatjyrbn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gjjtvkxji.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gokvlllmq.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gytlbywuz.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfizcignq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gdcywrsat.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghhrsakyp.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gujdzzjzg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gjvqimzyj.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gcdvmraqm.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gegikdiry.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gusjelvvc.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gufhdptkk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/givwiywdo.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gkdrcoewu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/girflicba.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gwdpbvmoo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gbrksnysw.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/giymxfyac.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gryvhnkjf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/guvdbwytp.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gzvkwveub.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/geicwdrqh.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gpeebtjhl.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gwzowzucr.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gnmujtitg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gffjauwzq.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gddkkwtdu.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gxyesapcv.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gktpqjass.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gwaqpywec.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gkznbwtoz.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gavxmbzuw.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/ggqyibkbg.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/ghdlkupfh.sHtML


<!-- 参考信息 -->