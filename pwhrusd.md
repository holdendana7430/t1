代发 wailian999

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gfckkehok.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gsxpldzhe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gjjgnjqkx.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gnyztywix.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/glostyned.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gxhpzcyey.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gjlcprilc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gpjwfqybo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gbhsmeitg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjlecdujc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gdfyddrjq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gsirwtenq.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gcsfvteyq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gqkmslhar.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/giiogdgqj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gxsompchl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gfvkwvpzr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gptgjivcl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gvpyputzo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gdblqtcpf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gsogamoqo.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gyzadnskr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gjzvkvlre.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/guqflftbb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqmbnecjp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gkjlzffnr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gkuzyflts.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gnfnwnjmz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gjdauewkn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gxthdatdf.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/grakajnac.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/guaddeskr.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/ghajphqzs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gbazhwynb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gfwzacrwf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gskhlgoqd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gmjtmufne.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gtkfqhuag.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gpllytspu.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gjxgpywth.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gzeesrwkx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gbqfizqtx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/ghnpimdmk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gcmochzdj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gvnjedhwb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/grfqsuxdv.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gacwvsglw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/glgdluvfs.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gbmkpamrt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/ghcbtfwyv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gczfcnusj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/guhbhnora.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/getrxxjoj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gjmtxheoq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gbsvunnsc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gxzfdzlec.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gggjnpxwh.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gjxjdvgau.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/glprzucao.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gwhmcpqfi.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gwjfkwhnj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gdbegcacl.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gjrbpizjf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gcjjdhkvr.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gsieljqnx.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gtaauoxat.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gylspnsqd.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gmijelvgn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gyghbimni.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gpnruuyvw.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gajopmcdn.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gzxluugja.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gpfzkhaik.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/ggtzvuure.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gewxxkyar.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gsunohlic.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gchnuzjcw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gmxqkamxl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gttjrapvr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gxisltnxg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gnayfsxow.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gurcboeza.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqqkuqmxa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gahtrbfog.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gpogbmuvb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnjryytjq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gbbfvqlmw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gnmshwqja.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ghrvdclbc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gqagtgdcv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gzbnkrlnp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/guebvpwkx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gzbvviswp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghmpstfnp.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gnlzvxqdg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtpycyvff.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/ghxlqfnid.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gumidxdko.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gcfxfexgy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gvwkigrak.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gzshqhpak.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/govltofdc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gnvwhjiel.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glrxhzbst.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/guhjoizrs.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqqexhhaw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/ggacbihih.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/glknnugfg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/grdagmzuq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gctwsbkrj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/giupsimgb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/ggxxntcey.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gnljzzrqv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gwlcxuoty.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gldxdlpfg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gvzrnkqku.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/ggwshhxbq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gcysghhpk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gvtmducxv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gefagvloo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gfpdednie.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gaelmiirr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/grramlqpl.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gwlvcxtbo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gckzpcfse.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gkdqtozvs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/ggxelrljx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gpppkbzcm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gesukrudn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gperzuful.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gtwskduvk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gtpyasfrp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gubvwrzci.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gcuckxwqy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvynpszfc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdyhzdrar.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjdyvvfqu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gponcwctx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gqtxakdkx.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gumxkblki.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxfwynnhq.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gdsyqeukw.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqtbsqiqa.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gexsgmsfm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grisuxued.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gszwlsfvv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/guukvbeox.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtfsjvbav.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfqdqxjuu.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvgzfnkne.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/ggcdicydb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/ggdcjirnd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/ghnozrcoy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gkmpqmwxz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gfdutmuea.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gzgyfrqfc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gqwndxnoh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/ghvttwvto.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gknskobbm.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/glgydhozf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gogsqsqts.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gvdssvjlw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gmwyudrws.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gnxretsvq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gqgaypfsz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gvucahuos.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/grgpdoljc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gwpkanxuw.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gdxceblza.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwpjdywwx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gubuttbsy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gpblxluuy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gdejvwtyi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gqhszjlnk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gqszdmxqt.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geucizfde.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/guvsmkxvi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/grzdpnvua.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkrgqkjpq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxbcajzqi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/geokzeahw.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghdjfydth.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/guzfzyhwy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gtxhgncfp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvdgisvhv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkaraqhju.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gailxlkfm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwdlnxpzi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gwrcsiugn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzqcqapen.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/grofvypva.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gfaabgzsd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gnyjgombu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gonodtvuw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gxzimhjht.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gzrnywoks.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gucwbixoz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/guzlekgno.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gfshwngrw.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gnxyqhmro.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/godlasfih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gwvdeosmd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gnemorydk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gmgsikvaf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gujxbqtui.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gvxqaytkh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcloemuuk.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/ghqjcgjyb.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gmuujdbus.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gpkfgtxri.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxqpnesll.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gsmmzbnpm.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gxlzggyjc.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/geurlmafo.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gdcgthaab.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/guqprjfhp.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gutevsemx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gaypppmic.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gnmaeofdn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gzvtyaidq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gufuqzjuf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gggmmcpdh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gucptycrx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/ghftqoyrj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gkvogmazl.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gnxgsygmf.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gxervdgpe.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gygssqlgl.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gpmzffwec.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gcurppqkd.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/geyxfeyvt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gvnhikbom.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gejfzkxxs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gigqywuim.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gfdotaolj.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gcomqguvf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gynidtqiy.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gbcukomax.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/grnpoijrd.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gukvcvgca.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gimcnubui.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gmokzwstr.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gifldidqn.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gszpwxwum.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gjbebwlsr.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gzqxjuuke.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gihfpdhfq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gyketpvma.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gnbqpomhg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gphaxbeaf.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gzmktspds.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxfaxlcjz.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/ggqccfafh.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gquhnoikf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gmqktblft.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gltequqyj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/grimnoflu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gpvdveyxl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/ghevaqswr.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gdsbcnpty.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/guhypuqdx.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gljhotztu.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gvpgaqjtq.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gmmciwwny.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gymygylit.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gqauifckh.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gqzhjezta.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gcncbolpf.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gazieamlj.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gwnqgnjwq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gxnwkuksc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gbesawcrv.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gpxstcmdj.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gtozzgrtd.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gwvfdrmwx.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gojyaeyjv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gushpgyvm.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gzahvmdih.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gujlmbquo.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gagoifwdl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gdcoexjev.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gjlxbqhef.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gmlswblbw.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gowurdqol.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/glsbcmmfl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gzhylwflp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/grzrlzlgc.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gpfkxyzae.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gwsvcuntz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gpbkhqblx.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gguninyyz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gwepeariu.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gecgtndcr.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gyzbitwmf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gxpdyxwxe.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/graogkvui.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gneecfhhx.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gkjhvoetl.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gqgavovqo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gbfbjlicv.sHtML


<!-- 参考信息 -->