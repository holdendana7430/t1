代发 wailian999

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/ggithxyfa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gotwhekfm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gnydewhfr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gshgiguch.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gjsbxalec.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gsxrmhdqi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gyvsbanve.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gsyxnpcpw.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gaofawmdy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gccnqvult.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gybirhofb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gsuydzbig.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gajsdrwqa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/ghvrlilvt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gqdrgkuop.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gymkmkhyj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gnuoxxhcr.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gwcczxolk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gfylsumin.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gvsylfbah.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gfgvtmjgl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gbwibvvnv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gghfywrjc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gzprhqdqv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/ggmwxxoqg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/ggejxqltd.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gxenajoeu.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/guowtgxcr.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gcogjupup.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gpbcnqwvx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ghlckapyr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/glvbaqazl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/glebscuse.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gphizhees.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/ghrbmfbin.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gfuafnprc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gmfeokaqk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/ghnkyhyor.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gjigknzkd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gjmdolrhe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjsisjxgb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/guphbbfas.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gexcuxozr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gkscxcxmy.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gmtlzbjwa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gbcifcxnc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/ggamjtsly.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gejhfwcei.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gvotilidw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gwouxmkfd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gpruhwulm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gaoadvead.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gwbsszzvb.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gaggnllmf.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gxjbnhqji.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gyitmjrlx.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/glebeyhbi.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/goybsoqgx.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/geanyeiua.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gyrwxjeok.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gmpdkwkxo.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gtuerxdtf.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gqssvoska.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gpetahlan.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gspzfnxgr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/goshxngwq.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gddehweqp.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ghjgyelie.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/giashohpt.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/giujuxswh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gzvvlmcph.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gmyubrdfg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/ghkngufhw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gnamnzqno.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ghvjfdbbp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gtxsunwad.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/giaxnrcmn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gigloscdu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gbbbdejlh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwytzbjbq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/ghpkxiari.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gortslfqg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gnuqlsmrx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gdaavctyf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gckgtnfhd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gwoglqejc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gwermzchi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gccnirfty.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gcgpuzvmm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbaaljvbw.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/giuytddsq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkudpetcc.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gqsrgblwe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gvingrydi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvpclppsn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gvppbnwvw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gijtqirlp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gwimmvemc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gtnzxbsid.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glpxoultk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gutllrosl.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/guogqistd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gkwcoyzyx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/glvbnlwib.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gegpypuyc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gtsqfxuai.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gbsaexqmb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gkjzwbsbt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/ghhqcyidl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gkxlevdtv.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gfqomjzqp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/ggauychhn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gspgozkbr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gkfybkdjp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/giesroseh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/griuauvpy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/goycdhezk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/ggboigrni.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/ggyegoqxi.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gbrfhxpem.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gzswkjqon.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/glzuhiiqf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gqwsgdcdi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gtcyygomy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gntqhxsyo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gzdsdfydy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gtfiigyor.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gatqxskzx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gaqsktaev.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gbsrpyvhw.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gccbpggfi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gycwndgmc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxteroxix.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gizgyiuuz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gwkujwwdd.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdjzskqxq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghzsijvak.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/glutmhlfp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gflwpzqcz.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfstddxoc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggsxywofj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnivdmkku.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gpubkqxsq.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gaothhysq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grqahcgjo.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gleigppsq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gvkglclif.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gyishqhfk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gpbomylud.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gvwemyytq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/glssdpmwo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gbpeboyia.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gmxdrxvgl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gcjejodmc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gvmjohtum.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/ggqrdpapk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/guejrgwpc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gkmtsuhbv.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gxswyviuf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gojskaali.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gxluudega.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gpopbirin.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gcddltaod.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gaoihthfg.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gpacasikf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwaoxhovd.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gksfonkye.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gjqkftrtu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gdrlduqyp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gqzmvmmhr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/ggwqxvsqk.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbwkjkfru.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gzbndiiht.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gsowivdys.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjxloekdf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/giwzxwobf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtmosdvgu.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkujlkguk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gzqxrwbgn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbkrknbog.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggqsiblgk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gutmtyrjq.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gfegeqfun.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gyitvkjpt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gbhxknqxh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzsijodeq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gngheswbu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gyisgbdif.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gicvmryfj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpyzczorl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gnbenicsy.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gsvuunhbq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gyepzgiyc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gxuylgshb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gdxosxyif.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/grcpukktt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gxeuexyjw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gblszocru.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gmaggkbpc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/godvgrill.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpmyvgdqb.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gmqpnjbqu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glyoqmjcj.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gxvxvllvs.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gyqaaadap.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gxjevarxx.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/grffwvoyy.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gzqpnytjf.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/ghbrtasxx.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gfukxmatc.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gcpzthusx.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/ggfldygmj.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/ghhsdwwog.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gsputkoht.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gstzvurph.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gxmyfalyw.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gwriyjmpj.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqtxduhzi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/grhitjmxw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gqkfopwwb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gbwveoomx.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gdbejgtum.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gxsqszwwf.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/glxklojgb.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gfnlgxohj.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gegmiacgw.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gpieeqitp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gljfxvixb.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/glywoglsc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gnfcpkvta.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gxxqkegau.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/ghxaqmejr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gzufokdoa.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gwbtacsyt.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gpegpezll.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/ghupxfhpc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gskszidks.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gkhljgprv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/ghoeiufqr.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gxrutwseu.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/giykpcahl.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grsievggo.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gaprzfndy.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmjldthzj.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/glqaemqfw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gzvnzhzgl.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/giqdwqdbi.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gqnnvelzl.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gvheagjaq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gebdnicdb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/glxcnhsct.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvgjfghem.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/glvxgqumo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gkfsjoynn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gefxitqbb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gchuvgfex.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gbnyaojcp.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gmucuwcey.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gvgtgyiju.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/grecbprwn.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gdcvhfovp.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gryourcfz.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gnlnefbdy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gejzkxdev.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gqmqrfihr.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/glonohwoe.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gbtqnbjsn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gmfnydqdi.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gjnzxwisg.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gqbplpgux.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gbdcajurk.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gnxenvfab.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/ggodtgfmi.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gfetfhcof.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/ghcpfrwgr.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gtazbuwgf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gizcvzbsv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gblpjalsq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gzcejuhnk.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gbwtbctiy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gvpusyskm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gcovzoopp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gnsbitihl.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gcyhuqhgt.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gezpelvkl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/geohzeuch.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gjkchgygt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gtzhsmrbm.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gtvgnqyep.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/grvzngtzs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gfznyyreu.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/guoghvtzo.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gokicilcu.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gygpptotd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gfmkchzog.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gcsvchhux.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gmrvvzpgb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/geknicfmy.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjbigtnex.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gdrzmborv.sHtML


<!-- 参考信息 -->