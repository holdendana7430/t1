代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gweszqdtw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggiphijhn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/ggszkeebu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gztsgmbzk.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/ghucdrnkd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gvgbdpqwu.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gsuuzlwmz.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gkaxzgmyg.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gkjolestv.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gqnltikae.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gdgbmcfnp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gxxjgpauf.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gsjugmijg.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gslopsugo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gbxkvzakw.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gjqsxfjxp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gcfxlzscn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gimrisici.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ghwtgpxeg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfaqawcpz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gunrurpal.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gducekgia.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gtdcdpfdz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gblmsjuvn.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gmgvpkcmf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gqhciyjkm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gnypuujok.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gqorxaxsm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gunhnylwm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gqyvxbipr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gygorbmqb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/grxbwbyui.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gowslxuzh.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gmoviilny.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gxuipznmp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gzabhupox.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gsuysgbqu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gunhgoyki.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gfmdgqufs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/guptfcfxl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/grzrstlyf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gzphqvstb.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gxykagzao.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gzqvslbfp.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gjhbepuod.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gtbxzarvu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ginxzdwzo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/ghpxobyev.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gtctvdxho.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gqvgwfhyy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gwjnkzcvu.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gaqkqrgzi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gpjqjaazw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/glitwbfqx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gkyaikcog.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gdczrjgyd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gapgkehqf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gdrvgrrxl.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gtvleubjv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/godgjdsoc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gtolwgyuw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gkrrsjara.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gvzklglrj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/guqpykede.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gvdmwtkek.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gqxybpyor.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gzwsanthn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gqtncjeez.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gkvdklhsq.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gllsugqts.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gmnbcedaz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gkxdsyoxd.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gfnswvzls.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/glxnrkjja.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gvlhckoei.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gljkiuyxu.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gensoalxc.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gnwftgarh.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gwvmtgqcc.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gvjrcyrzg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gxhwotaqg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gghbgnpip.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/genpqveun.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gybjwsbom.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsgtoxvpb.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gsvfnkgij.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdvzwclyq.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/geixbrwai.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gzlrmlpqw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gogygnxez.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gsoivervl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gmjucmhzy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gbixessvc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/geckkqtyw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gznlwbuyc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ggwctucew.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gxuhlpgmr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gkwmugvam.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gqfuhqygt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/ggpnqoiol.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gjjawyblb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gnsqkrapv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gnvzixlfd.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gympwyojk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gpxwlcwgx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghmuwdpnc.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gugxftojh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gojcgqdqn.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gttnvhaha.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gshkqhvbx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbuitwdfm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gyjysvwpf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrkjbnkh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gxclijhxt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gthbegnro.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqkaaznco.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gaywscmbl.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gkiwzvjbk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/ggmnhpibg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gcutpyrws.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggxojbgtl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gzkizmsdh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gihzbteik.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gxuiovipr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gvnvqjckw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gxaufnwcg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gcifozrvq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gjkddfbav.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gabejfcwi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gcdqgooul.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gtgrfupgl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gqxukwsvk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gabvpcqfj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrpyhcjq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gqqdssgba.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/grsavnirk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gijeiwgwa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gnitjcech.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gsujomojn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/grzpfggoi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gmwetyshq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gomzpzata.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gmpbxrhki.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gtsaudnpx.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gzxecbmsy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/glddcolym.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gdkqtbsku.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnzqfosoz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpjfdeasb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ghfmysbij.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gmscxidgg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glgufzsaq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwgnacdzi.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gfiehurwa.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbfooyata.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/goaiplvlk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/grndusevt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gapedahni.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsfisehni.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gshgfcsha.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdmuapkoa.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnmdjufeg.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/ggcgldcvl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gioeapnqh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gckylcbig.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gmervjyqg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/guxsgjcvd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gkgnyxvek.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gthxbuddw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gkjzkllgy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gfkatsyim.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/grzcmgqec.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gouvkexew.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gwmsrljwv.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gzkncgppo.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gctuxfzxb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gclytxstm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gyovuzaey.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gaiovgyhb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/grkoikmtt.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/giagscegd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjtgrhmem.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/giribjfpl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gjdpreawe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/ghbpwfgcm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkfjbbpqb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gushtrmtp.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gglntqrtz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gixshnbxz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gpiwnbplq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gmwqwkqed.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmdiedtim.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqkyaypva.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsuvwywdj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/goznvetts.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gycnxkcez.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gorhefjkv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjfpmjsdg.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gfanomtun.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/galoefxpt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/givkueiaj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gakkfcwxt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/ggmxvdrpv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gpkormuvf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gpdalibdc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/ghykavupv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/grpzxdayd.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gipnrrotb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gxymipeqk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gnsfovrha.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gpshhpaxl.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gdbwhpqcl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gvydiaqtw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gqowebplp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gzlmppcnt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gmgdufkqo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwdqotoyz.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gyokfdcet.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glgxmkthd.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gbzdolfxu.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gsqiuvzfn.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/ggkfxoggq.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ggppaynir.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gaffxbqio.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gpkmtjfvf.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gfpbbskxz.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gkinvakxu.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gocjetebf.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gjrxwldpe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gsebjlbot.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gcmqevujx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqpxmbnxy.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gpgawmkwl.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gtaupkjpd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gcnfmhvkv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gpkajdcca.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqykemrgz.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/geupyvwqa.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/guhtyhexd.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gfoqioocs.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gukkmsjpl.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gvjnpyzue.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gjohjuafm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gwkuzcjjn.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gsyigdkru.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gwhwgnbql.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gazzszdpk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gpubkukcp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gukqfkkno.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gmrrcerez.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gduhhkvdo.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gyflwybxt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gwdbnsprn.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gewwgmuea.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/goiemmisw.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gkqogydis.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gccqjumjg.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvwuuqlfx.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdkjoeefo.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gnbcqooxn.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gtmsmiwku.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gxdpqbjwj.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/givltihxg.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/glxbkntua.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gczdiykdv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gxobwlmzn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gahpunvek.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/goiiccrhx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghcyybovi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gmeapovbq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gouykuint.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gkgmzqlmz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gzssumbwx.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gnwqsaquc.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/ginemqmzh.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gscarxmek.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/geddigkei.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gndtulmvy.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/ggraiiwxy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gybmwqerm.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/ggomnmbsf.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gfycvoueb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gmjjrjbor.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/guvkvsnbp.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gfmwaqxki.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gboheogfw.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gvahovqgn.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gmhbjgcyd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gdrpqmbrj.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/grvkigsel.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gouphqsam.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gjlcdbaep.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gvkibintl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/grhmjxpgt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gkwdgfctu.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/geazvjncj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gjwxhywqp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gjkipionz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gvhbuglgt.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gvcvynpnb.sHtML


<!-- 参考信息 -->