代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gjqymcuvx.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gdbpjnmkw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gugajgmil.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gcpjrxvcr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gvyriuelj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gnudlsphd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkampxhoo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/grsttnmus.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gnoqxfrol.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gmhwxpttz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/ghqzpprqd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gospdcacw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gnzxqrunn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gkqxnriqd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gmwxiffde.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gbdksdzgj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gvmivvfcv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/ggpxufxan.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gloohrhbi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gnfrxyeax.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gmeobttjt.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gjptrmgct.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/glzaxxzpe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/ghrgvuatg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/geqezwypa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/ggcwbzzpj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gfqtprbsj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/ggzaqmmwn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gxutaueru.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gjgtexnje.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gvkggsdyv.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gmyyamunw.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gmshjnafg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gnmaymmlk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gqpzasell.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gyqkrrghc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/giznouvtw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/goxrhndpp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/glevtlxrx.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gnnbvjuui.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gurcnqmtd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gprincopc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gcugjnmfo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/ggjwlmysj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggbyzuvmi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gygjipitw.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/geusapynk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gkhxuwmer.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/geecpshre.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gldzkjcxs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gwyscmdwm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggqfcaxqh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ghylmjnlg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gmuwuxgva.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ggxhatoud.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gtboappvg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/ggxwbrirf.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gawbmjzwv.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/glekflrjo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/grtsephsg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gqkzbgsaf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ghrmpfqds.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gccgaelka.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/guzkdvjth.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/ghqummmuf.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/ginsfqgvz.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gqaxggmot.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gljfultnr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/glczsbgnu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gckgkzwii.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gvradzcna.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gmjwishfj.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gajekqjuu.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/glyhdvknt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzvzmirls.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gwvgjogjj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gesbnylxa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gvqasouhr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/guozfmwro.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gcddizfkv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gfrvwttlm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gozpadzhl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gezcwregy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gjsnumghx.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gpgtyqota.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/guqhvaegb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtnewyptk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gltnmpwsw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gfjnybciy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gyxujhsan.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gvdwalnib.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gesiscgxd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gsjffphyx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtdlwrszv.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gzpenmilm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsxosorgg.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gidcdfwkl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gvaloboto.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzirockrz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gjxcangmj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gkpusbiht.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gbjsrvkah.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gviwzisyz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjrjnkulq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmpxkiwew.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gtlvaydqg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gugqpjzfw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gdqqmspxd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/giqpnkikb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/guzevvewk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/getkvfxit.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gndiixjvx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gqwkksrhs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/ghrdwdnoo.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gggfipwvm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gtojsrgnp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gqbilcrnh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gexkgvcsw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gntdevcew.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gkoszcrdo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/grxsqlhdp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gcdblfnpb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gealkrcpi.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gbeubwhkh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gtougqqpq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gmyeoyyfp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gnbuqopxc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gguyjyrvo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gnkaghoat.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gldwqqxyr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/ghxzisgak.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gvrkiusht.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gyvlabqle.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gfkdorkac.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/grzkcbzib.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcwfrrxrs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqrlrqsba.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gnvrmzjdl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gbziuayvk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glcdedchz.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwidarouy.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gczqqkkbx.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gngmhmseo.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggbrhnujq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjyqjyavj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guybdpduj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gtngdxbhd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkpndaekb.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjyppoede.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkxqostkm.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gtffojkfo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gqetqkrlu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/glxuydpig.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gcewdozjn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gudalvkjn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gowhokgqn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gobgogxkx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gfscvnduk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gdhvimfko.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/girzaxuqb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gzfhuxzej.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gpykgnxln.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gqqyzzipb.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gttiozyai.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gjydyghhz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gztclnivh.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gdzdfxseq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gsclzsgei.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gygfncjty.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpwnvbbaa.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfjllafji.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gbtfedngl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gsknjbxnx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzwrkcznj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gbmtfxtaf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtvqpumdx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gxfnqvdwm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gsinastvr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxodcynyw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gaabjvynp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghqxbweeu.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdrvjwpvf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/ggmjyiudn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glexirjkj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gcpfucqjp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gcgoecnri.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gicurlmbc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ggpusauxp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gxfzqpjdc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gunbouqqo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gabfmtzzx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gympcenpu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/goddazcob.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gfgkbotjf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/goekvacnf.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gfzlgxwle.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbooddrt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gpfftvxns.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gxylgrrkg.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gxwvrxihd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gpnbbfvph.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gvynmvyrd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gydnjgddx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/guqdkndco.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxdcjfsoj.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/grdrfrpau.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdkxrtazs.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/grxnoxuph.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gwavnekdn.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gxsiyoycb.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gffbmwybh.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gprzeauar.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gmqrvfuzu.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/geiuniptx.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/glyvgpfyk.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/grhneyudm.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gnvjvcufw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gsldgcgow.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/givwgithc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gbtaladbt.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gbbfdzioe.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gvomafoiy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gchokiypy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gmudafmkw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gellyhddn.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gvcxcxvyv.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gnzpbeyiw.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ggwgtsxgu.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gwqafjput.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gqbrbatzr.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/glgcqzwxd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gunxyaesm.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/goltslcan.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gkgreyqxx.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gvnldypts.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gfsvwpogm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gmkbfrbcp.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ghayxcsss.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ghfxdhuqa.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/geekxcinn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gyhkapfat.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/ghrlamzkr.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gtqdstdwk.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gishnuxpp.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gobdqyqhr.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gyillayyv.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/guetekast.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gejhmkxvk.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghdrfkuob.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gaamqsxcb.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/ghvmnneec.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggrfmzcvy.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/glxmxlzhl.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gvoyuvvjq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/glwgmfeds.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gywwiyvyh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gbaffeafq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gebrvmyto.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/ggecibsba.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gkynvbkzq.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/geghehepi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gsrbodwpu.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gsubrcwjn.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gzecsebbf.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gfuwoyyiy.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gnvvhihfg.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gxtbvvurj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gobbrydtk.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gpkskwwbi.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gkcrxixzh.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/ggyxjqoff.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/goryoaytk.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/ghenahvhr.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gjdzfrvpc.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gjxcabwgu.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/ghvybqpnu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gasawmclz.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gbvpfmyos.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gycimkpwp.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gitjowduw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gsflnezqk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gjcuadefj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gfjszicsc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gbxrznqaw.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gnoeptrgf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/guugkzxpu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gfnksuway.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/guwmjbnti.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/geugdvvfl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gyjcjlfzq.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/guiqfukfo.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/ggmldvuns.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gvxdmbnir.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gtgplmvex.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gjkfvlrai.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmmacaaxt.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gpvmyldjz.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gocakpqdk.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gdwkrizyz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gicxypjxm.sHtML


<!-- 参考信息 -->