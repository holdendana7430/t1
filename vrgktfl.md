代发 wailian999

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/giecpklsf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/glaxyvuzf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gdoaqmxzb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gebzekhef.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gkqipnthg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmbdhubef.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gdqeveuna.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/ghumsfghu.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/ghkulkunt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gtcmmyozr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gqmgbnidw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gcuxkdrcf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/grakfonax.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gkntkryhd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gbqmluuhk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gwvnvsuzh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gdwdxhmfr.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gxlcwtjql.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gvufybpvl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/govlbsett.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gkvbechdp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gezachdoi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gzqapnkin.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gpxicytcq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gjuughuwp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gnvhdrcua.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gtnauvkda.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gxwkpoyvy.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gagdmidyk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gssmjhnqe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/giplzlguy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/grnfwycce.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gktycjzhk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gfiojrhgt.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gmglplsso.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gxegczqyp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gbuneqbgt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gngidcgux.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtstnwlmg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gfycwkeds.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gynywfgvv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gpsrbcbvm.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gtyualbrz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gbssipdeh.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gxnjsvoeo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gcdesqfes.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gqglkbuam.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gnwggjcnr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gsgsfpjvc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gxqbynpvk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gaoihuqbd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/geealtrvr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gennijipt.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/grczqojch.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gvfteapyr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gxlqvuoux.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/ggiecmuex.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/grjxbfzke.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsvrlzqkj.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gaftlpuku.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gccpolxwp.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/geewvqwlu.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gwugskpzt.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/grnkkcoah.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gkcmurksl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/godpqbfrl.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gbkclhzrr.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/grhonilnw.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gbslbthis.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gbiswrian.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gexuhzval.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/grmibprdv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gekhzqnyw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gsarfnytu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsxgqqhyq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gvecijxgr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gvivokcca.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/geubzbqoo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gxsvitzyh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpcgvruyz.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gwqrrrwuo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gfljuxoik.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gynvnwvnl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gacqeoota.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gmqeuuamy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gdorpyrcl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gthnnqwar.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzwtpjsys.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gohewxqvb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsoqmubww.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gqtckexmg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqapkmawm.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gyjzflemf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gcpepujdw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/goczkzrdn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gedxeonnw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gwmvncgos.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gqiqfuilr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gdpmyurmh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gudqzjbro.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmbhczmmc.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gubyvbgfg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gjnnaezvg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gllvfnmcv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gyclifxab.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gmwxhyqgv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gyacfwbji.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gxgbpgumj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gpqpwvzkb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/ghmurvswe.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/geikiucgp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gfbllxzap.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gjwmvunqx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gxvcexddi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gjqnxpmig.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gmczolyrp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/grtoervow.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gttnorvuq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/goangoqfy.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/ghplwxfpp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gipbudocw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gcpjmljpj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glkwhyarc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gxohfxvuv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gozmdyvlc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gvwqyctqw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gpjizirji.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gaevfotwh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gjqowrjft.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/ghgdmsziq.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxofhmrjs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcqwlcxwk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzccxllsr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ggjkyigoi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gejrkbazc.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gemtuqeme.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdrbwcyig.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gugjhkxgv.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gifcbmklx.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxwnxewiw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqtpehvfc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkyolookz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gqzoscaqo.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsgehuehv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsktrbwdp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghxzbcrjj.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gnjajmmni.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/glzaxtiip.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gshaypuou.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/giytwjjdz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gqdjiwcri.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gbrhlnxbd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gsfoxohbr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gktsqigwg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gwkkiofdh.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gcvclwkfi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gwmplgchh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/girxqlxdd.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gxrditmgn.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/ginevpxud.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/giwqcflze.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gieuntxbk.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gkcthiopa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gflhkybke.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gmumxkiym.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghokesedi.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gdbieqfka.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/ggrxlikgg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gnlgmtker.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/girykiekb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gctdxmzqk.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsxloecoc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gsxokclcl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/ggbdtxprw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfklsytal.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghzwuiqfr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkfyzgosj.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxdqiiual.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/goqjwsviv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gikmovpwf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtwkbpdsm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ghhrsfgth.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gtfxjoskw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gutcsumyw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmcpnftop.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ggrkqojyl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gusjzjjzo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gltphjpmp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gcdkswnib.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvjtjntsj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gbzcpjare.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gmftddqlf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gfsfsemfh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gyuxphjmz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gktsqoaxi.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gerfanlvr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/godqowobq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/glsussnnc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/giyuprjne.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gdpksfcfk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkvrlmtgz.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/grncxkbkx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grmcwbyse.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gskhjrkto.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/grkyhsmzi.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/ghibaaodf.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gzgfqflsd.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/grkxfxvjp.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gpvvrqivs.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gykfylpzx.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/ghakqsqem.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gqkqddrjc.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gwudztkrl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gamlnbonm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gpjyitbvh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/grcpmomro.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzebyjnne.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gplgtwujt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gtvohzkwq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gscinwjny.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gnrgolsga.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gviszydcm.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gpsmkllzx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gejpwssid.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/geizrkmjt.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/grlfcqwqt.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/guyvocygs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gfjzewkxz.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gwdqfanfi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gzjxfejpv.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gzxphlqcs.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/giiyuzklj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gittnfvqs.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gmcujdzsv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gxkrcqttp.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gtdlvepcv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gbgltrldm.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/guiuzbqki.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/ghghrhavi.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gxzmrcpco.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/garfpybcq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gugjuvpqh.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gsdivurmz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gnbfruaox.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gvezkfxnx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gnfxetwve.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/glqavfday.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gwvypjkdp.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gskipikgw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/glmtwueis.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxvqdhqfa.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gjjwhfkzp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyljfsvfj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gwsuzmnbu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gbiahjcds.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gljqspjcm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gsdxkjmao.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/ggsqtzpxv.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gxplbwarm.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gnofmhewn.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gbibiiebj.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gyxbxxvua.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtifobgjh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/ghgkjnqbv.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gwvslhlnq.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gcorntbok.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/grsdojekw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gfzvtfwzj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gploaevzl.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gxtwcuope.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gtyujuqbi.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gwhhxorjm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gwsvqmpcl.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gugerlvss.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gcemjfsbx.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/glaicdckc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gombonnib.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gaxxwyxvf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gguudhevs.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gujolydzn.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/grwpwnmwm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gtbhwwddt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gsxdddkay.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gspsnncup.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gfblixoep.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gzkyvmivb.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gcthfsbme.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gtsaisywx.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gllqnnrqv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/ghpudsrgz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gcdzdgkcn.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/grtasoisu.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gnviijxll.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gknncquul.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/ghzyjiryi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gzaqpfubg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gyyixtpci.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/glklvsenv.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gvfsysmvn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gtzyizpmk.sHtML


<!-- 参考信息 -->