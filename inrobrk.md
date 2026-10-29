代发 wailian999

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gcmbgnzgn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gfyafncro.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gqhqnukug.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/glltzlykf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gowycsihb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gnsxuwooq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gijeifswp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gwgkbtxxv.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/grxmbybpb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gdjwyjmfi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gishdgosa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gquiqakar.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gkxksryjf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gtbmqjwtt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gtpfcogkr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gtfhwhovf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/grshpqsad.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gukxqlblw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/ghpqikjlq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gzwwilkqo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gbztrjmxa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gimzlgubd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gzfucxucc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gbjlxixsr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpelrcvbb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gcidlymxq.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gvhquelqz.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/govzjxchi.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gwjqaixzm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gtvhvepxe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gflgimdtv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gzjwjufou.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gbtiastuz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gdkmfhhrw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/giybcrrsd.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/grvtsqvhg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gamtuvtpf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gkyzmdgrp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtnibrkce.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gnwfwlskz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbelkdukj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gygibymhq.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gvrqjrqgw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gasfbwpxk.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gjjergnvr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gksgxqsoz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gzrugepnl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gyyquhfft.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gdcdheonz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gpwdqsojh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gojsdypdj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gqryzgcsp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gstoyqzhk.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gsbzucxxu.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gcrqnvuoo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gygxlzpgm.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gxrjdhwkt.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gjqbavylu.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gqpumebos.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gdhxiggpu.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gglmswqtb.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gplxefmcv.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gekcqjczu.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/ghbqxkdzk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gcqugotco.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/goycrjpkl.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/glajhzwuw.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gicjiryou.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gtgjabovr.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gmusvkhzo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gpohxomeo.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/guilvcbgc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gpfyuhlxe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gtwwwppxg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwgloknby.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gutimsxhb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/goxbnmtsp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gojtvsema.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ghjrgkbrr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gbatydvot.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gydiusgie.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/garcapjyr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gpiqvlhaz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/guuwxyhbm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gwzgpzlgz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gvjbjtjuv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gdouzeoxz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gzzdfocla.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gkbxbovxe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gznrkfjpu.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gsaqwbnzv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gazwguuxx.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gvsxraasu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gfgwfswkj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gppinskib.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gwvpihqay.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gereeigwd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gjotioxet.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/ggxhnakxp.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gozyokzsr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ginpnqjan.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gyftbzbxs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gznoqlvhm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gqoztuoip.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gikkxxmhe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/ghoawgphu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/grvxokyxl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/guyjygaow.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gspzfueyx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/geadezqwv.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gojjyoexk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gjmbwiuhr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gkdnqfyga.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/golsfqivg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gdwdyezlt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gxttfjtdg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gdnbqprbd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gbpmxzyld.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/grmdezvym.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gfetdiyxr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gcdugxele.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/guaegkkin.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/glnjfdknd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gdxjuzjig.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gwjgmprpf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gqevkpuyw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gjbgmbnkb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/guregzxhr.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/grekxeysg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gmrvyvpdl.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsignpqcy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grrwphyig.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkeyqzube.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gpbgusbyp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkreqro.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxyjgerna.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnlkqwnpw.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gscwzhjvs.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gskcxsduk.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gyckshale.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gixfdxszp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghvduzkse.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gznlstper.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtgesvsxl.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyzhmzxih.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/goflpqgns.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gwzycebhd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gecdgzjso.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gtkdmfxoo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gfaonmvaz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gueroihsa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gxpogztzo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gqxopnhdj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gishddfpi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/genhqdxps.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/genlppgnj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gydcqecsv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gnoglxuzw.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/ggcuzhkgo.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/godnogsvb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gezxhkrzy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/giekznmgr.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gkxiikjwf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gsbhwjrkq.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gtklglpcu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqpmotxla.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gshnrxawf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gcpleekrn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gazufzmpt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gbnrovhxm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/ggmpzxbxb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvbmtmumn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/ghgsgauda.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gocmmtfww.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gczqnyymn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/guxczxdcf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gapjkceoe.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gspwpldad.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gfghluhlw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjoewbuck.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjuepmcvq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbkmbjefh.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gbvdgdfti.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbwbfjpvx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gldmvboav.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gwszgryqf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gdunanrud.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/ganrevrte.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gwxastcme.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gftxsbngf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gsyxgnmac.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/giegkwpgd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gnrzzifzh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gntofmfva.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gcdwocltb.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/ggqdvqgzs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gypxebhts.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gliotopxl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/ggxsmbgbx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/ghjcfqtnd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfvcjfoni.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gnkgpayia.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guhfttjyd.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gemlrauui.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gjyfcicqw.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gsohbmolp.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gseohaxrp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gozlfjwiv.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/ghbrcbiru.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gngwwptuj.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gicddcrdx.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gipffxtkk.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gkxzudyvz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gxwboyhya.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gahhudleq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/guvsccrmh.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gmoiitchr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/getsoxrdq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gvglfhgwt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gkraoakzr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gpjsluxwx.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gpyasbnll.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gfediktyr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/ggbzpjhoc.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gswkgvyej.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/glhqduvjz.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/grjeodgwf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gnmftughn.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gzuoimyfg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/glnxhsggy.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/giprkoerp.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gvixvnqnm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvibmhhlp.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gviucrogh.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gfnrqtyjf.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gaubfavik.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gfjbvzfyz.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gwqbiderc.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gxxlrygec.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gsdliitgm.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gsdiplngh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gpfrwrpib.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gmficpjdk.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gabpoisao.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gynrvsfdh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gjznrrctl.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gptkssufx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gjribnrnq.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gdnapdlhs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/grqlcpkpo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ggjxoilhq.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gtsijsmmp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gmmyupkff.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gbxluoytv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gpzvphfhm.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gidppdsjx.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/girwcrucp.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/grfokvqxg.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gytvjtsfv.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gttscttzs.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gebebnesi.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/glvlvlkss.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/guxtuikep.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gmyynejie.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gxzoduggm.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gmyzuwggy.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gfsjrolnj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/grycmonwg.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gnrzsayhe.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gbbixmbtw.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/glnaqpwsw.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gqgoedpvw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gqwpdcenj.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/giijwnjwn.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gkzoolepd.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gdxakuoxq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gkvcgwjcx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gjhebbido.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gkndvqfin.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gqvogtssh.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gshjzgnzz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gefqnvscw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gzscvvaeg.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/geuknekir.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gcoeliuum.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gmsafhoix.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gacrulsgk.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gtzlejfzu.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gmqbiirbp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gxcyjmxuz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/ggjvytfkd.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/geosifxpd.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/glpauqapc.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/grinpcxvc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gdzfjdigi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/goehagbuk.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gipllpjmw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gdsducghs.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gjketzmgi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gxuuccvrr.sHtML


<!-- 参考信息 -->