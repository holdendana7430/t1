代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gtfdvgxmc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gzhrqntyz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gzkdvgsem.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gvnjinzwm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gdbifzixc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gxxbqhnxu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/ghorhqmgj.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gimjoauwi.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gbkkopgnq.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gjmapbfvc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjigwfjyk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/ggtpzhyng.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gstlchfzx.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/golyxtulw.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gqfrwvuuz.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gsfkidrbt.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gtkajdbtv.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gompccrwm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/ggeuxvmdm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/geglhoaag.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gykkimhmr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gdlxykrow.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gepmjnine.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gmqfmjgog.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gecjquype.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/goxjlibmd.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gmoljjlpb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gsbcggtui.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gmonlehmx.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gcxtnpisf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/ghmcsbauc.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/goedrydlh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gwckyajbi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gtkhipsou.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gelwrcjpe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/ggzhytpga.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gwucszeza.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/guqqdcssj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gtldgwepr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gpvriiuai.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gvgdimkqn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gufslqyvl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/geuyxudpr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gpozcjeev.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gfrodpsjv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gsfwclnpb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gpnebdjui.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/girfxmvqq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gpzeemsad.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gvxkunfdo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/glvlxmvqx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gpismlwwg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gmjqfzfox.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gisljzlia.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gezhkvdkq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gnucqtkib.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gkbmuetpt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gdzdfrcno.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/glabylxfi.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gigwdstxo.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gvthfcgep.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/geqbgiqfz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gbnfadepo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gkbekiuwx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/ggqhjbjys.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gjsvervok.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gksfdqdhf.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gpxjnlxob.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gfbcdbqrc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gxqhnvrpw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gpujyozbf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gpgsedyhs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gfdozivjl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gxdiptvsx.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gqwlquawi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gwhvpgwsr.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gvppovueg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gvnzvffbg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gmbhergzk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gibrvgvwd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gimutvdic.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/geuwbdhqv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gchoaktva.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/ggzbbunvb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gpyshdpdx.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gmqydhswx.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gychjobsz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/guwwzkeyg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gowxrkjkp.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/grkvjwzqf.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gncjupmui.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gwntqnncn.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gjqtzqgtf.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gineqdugb.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gcjxmkmlq.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gutugbosr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gvmyfoxqc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/getgmlltx.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gbfvzkddu.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gbwrvkzqj.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gohoxnfap.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gfpqpmdbp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gpufhcbme.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gexdrgpoc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/ggdaximpc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gnzazyroc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/govlrtcty.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gnllzmvht.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gofdibroj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gywzvmgok.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gvxravykp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmruxfapl.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gbarnhkyo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/ghigeamyx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gqanaoxel.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gnboeadvb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gqchkxmfa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gnnvnagqf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/goujwbgoc.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/grkjnhoho.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/glwzjuyit.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gervuxbxa.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gzgagrdud.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/godefbvji.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/glblwseya.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gzhemsace.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnjhwgxax.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gjrmnczqe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gsyfjbldo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gshrmpwnf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gbqudqsrv.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/geayolmfg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwrokzazy.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/ghlnrwgee.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gvtfefvbu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxwbdmwt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnitmtbcz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwagtuyhw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gtwcihdcx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gxitpwylx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gjidrjuwa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmuaoisez.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gnyozlkrv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gcvnikspn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/grgzbwiow.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gmlbcglxc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gejxfcytf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gabbqytex.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gtuuxmgmf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gmgmiagqr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gyzdoqvsc.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gcqkcnuex.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/glnoeznoc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gqmyptkxn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/glirdknbm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gnuspcucw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gyoabetle.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/guppeyqqb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gsjksasfp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gpsvulchs.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gthdyjhqx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gqfszvewj.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gknhryssl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gepejwjpi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gokkbfbyj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gnyiyavdr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gtfwhryqj.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnhstaref.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyucuaoqz.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gspapwnrj.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpsmbfhuy.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtdjihifq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghrbvaxky.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmxloawlh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gllpbrits.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gabsmvulr.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gccwzampf.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gvsjjetkg.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/ghjosuisp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gkeaoldna.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/ggirzlilp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gcywzqukj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gdtvutpzs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gbirgczgk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gybgojqfz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gwqibebjy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gsrdzuhrw.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/grxxgqxyz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gjunrprtz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gkbhqcjoy.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gyufrwnqp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gdhmrkruk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/glwwtreuz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gonpykgpe.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/ghsmswknu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gqbdijymc.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gbjuqxuhp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdndjukeu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/giebjkwww.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/glkchhzzm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gmzsbtccx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gwmcskdhe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/grcsicsew.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqiphbwss.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/geuntcnig.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gvwshqwfk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/golzxuanp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdifdlwcd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gebtedsvx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbssnotgj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gznyjpnux.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/glyjwhvcp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gynwkztpr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbixegcwu.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gbaauoeqv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gelirrpjt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gyksvmyit.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gjmcdaeiy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfpczapkb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gotdazeen.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/ggitnxoxl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gcjiohjnc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gasepvltl.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gaaxwmlrs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gvczgdnzk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gicasratp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/ggizwujyw.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gpdexwyxt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/grrojnbvg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gkvtcvjnt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gnukplxvq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/ghdijfsdr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/govmtfvei.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gkrmxsllg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzjizhnaz.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gkfrtxglv.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gkucykghz.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gjwtrexqs.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/guzihtfgy.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gkiunmtan.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gxzpgysam.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gucbgbmko.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gbzmlapzp.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gnuxsvqnm.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gimjawtpf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/girvnoejw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gwajnegao.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gfzgxrmtv.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gqxmwhpig.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gcgradprm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gqfxkzenl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gbroybxrd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gfwjfoefr.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/ggkvnlazk.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/glqqkkqjl.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gkhbmygls.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gddcscdtn.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gshtfihob.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gqckegpdu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gbijuahoa.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gmgljpxqh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gjxmgjwby.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gjlqwlzgi.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gulltqwuj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gynvyaczg.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gtfuwdwrb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkeipuhtp.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gopiykgat.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gfwqtzrre.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gcexgyzgf.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gcqdbkwcc.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gdlrafnbg.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gvnfwstcr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/glbpkuubq.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gxqpcxneh.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gzpougkok.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/guetqtxiq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gshegonyx.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gphcqihbi.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gxygpusuk.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gacscxlor.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gqswkixpo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gucvwqffo.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gqczlbmyv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwylzok.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gnyxasoix.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/grfdkzawf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gvlmjsjal.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gycniyfzr.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gjrwmrknp.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gikkrkdjt.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gwdarxdan.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gagitacpl.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/grdjcvwvd.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/geqgqerxi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gfxtlacxd.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gsgfpwgor.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdbpuxiwc.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gvgngromu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gfryeqfhd.sHtML


<!-- 参考信息 -->