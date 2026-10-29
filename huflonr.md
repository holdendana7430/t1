代发 wailian999

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gcxntwxsk.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/ganmwroae.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/glhercdex.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gdvcbfveg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gjibjxtxy.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/ghziiwlos.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gfrwpxiyt.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gziztyfgn.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/glwjgpqxt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gpfiimqnd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gtbecqszp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gojtnirqa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gpxquukgz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gtetgzwjy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gkdyukibw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gwayvzmcg.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gjellgykm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gqrneduvc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwxqaddyz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gnmceqwml.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggptnwadv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/guwbjqlxa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gaczocpdx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gqqkpfodv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gyjdeuwls.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gsdffvyjv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/ghbewveej.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/glmyslczv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gthncbdow.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gmykbezjz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/giluohgud.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gewaaymjm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyhstmau.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gnefaktis.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gjfhygyje.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gizphnboi.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gndwezlcn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gmbhsnlae.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gvmmsxncd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/ghrvxqlxh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/ggdbzpkqq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gfmjmcxuh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gdhbijeuf.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gpwhslceb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gbpgqjggr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/ghzwdkzym.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gylbtdmgc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gcxivapmb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gtuwggwud.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gryxnofqx.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/guerhazrh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/ginwjnslr.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/guochfald.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gpkybgxzm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/giwdtteon.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/glfmstrfi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gzciritkk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gbxqvtzxd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gkiyurogw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/guzowxqbn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/guciqwgwo.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhwybgm.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gehvqxnlu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gcdvqdttw.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gcptpdefg.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gqzsccfsx.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gutzrxeur.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gghavyptf.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/ggjlkhifz.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/ggigcjsla.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/grssfhylv.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gqjcphzjt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gfmnainqo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghglkmcic.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/grfnhpyfg.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gbkzvzivg.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gbctnjlqg.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gsxlsrsut.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gxvaryolt.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gtpdqydiw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gwgidcled.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmnpkzmcm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gdqnzchbb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gjxhignes.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gorbvgidq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gnxhjqenc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gkaynoapg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gggavlppm.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gdtyomacb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gywccvwsq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gnhoihjqr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gxivetlrv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gtzzjqvio.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gxfttnlih.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gkyvefwnm.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ghywrsfru.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gokrsmcxc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmpgwgjqp.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gtdyaoxux.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gstcqvmqd.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gdmdzgclq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gxuetqiuz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcytwhrpv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gcqpqqvmq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/grfbyvyfd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gdyssbfzz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gdstreijf.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkidszsug.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqgaokyxr.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/geqcruatc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/geiuyuooz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/ghjzswrtg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gdbzrvvln.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gfjudxvjl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gkljrsles.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gqfcytxhb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/ggvfbsgxl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gwwimdonh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gzvyrsknw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gpexnxupz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gcsmogcau.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gklevydpl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gamwzlbad.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gwzvzsyum.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gjfegnuxo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gasqwxgvp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gmyoorqjd.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gtajizron.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/glzblkcey.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gmtzncftp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gxrdfgkjv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvhfdozzu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gychgfntq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gnrdqwvdy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gjijsnmuk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gwslydkiv.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gmdoyvonp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gjgbplywk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghqxrkxqe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtressmng.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjdklyfld.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gkuumjnqc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gkecqdjfl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjpniagob.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyhnnjrhc.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gdaplwjop.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggpvdofno.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gujuzveug.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxjkoiuil.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbzezzeyf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gkzspplqf.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gopuadvem.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghheogrln.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghqiqpevf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gwucyezqo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfxkwlikz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gvttjzgbb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gmaxycyob.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ggakrvcar.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gznocvfji.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gncpbxcht.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gccvqaghq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gsnpdbbex.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gagrciadk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/glrhylhnw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gkeyblpcb.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gcqjqyikb.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gyvjdiglp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/glcazqgwy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gstgfxaug.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gqaiodexv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gdbvpjkmz.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gpllbgvnu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqdixpqph.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/graebbiwk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gbtzpsfbm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gafncsdzb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gwhlevqsq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/glimrqkbw.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnikhznas.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gyaosydnw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gxbxncvjp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gozajfamq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggqbuuoks.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glwofmbgo.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfslctauw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gfwxhmfbd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmbvnhkzp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gftvcajmk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gilaprjzx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gdxbuqhue.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnmbiefke.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gydfkjepg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gapndnukp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gwpmuhhus.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gydxsuwzj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gdvbzcgqt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gxuaszrwh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gstrqwezh.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gbiqpvfqf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/guimdclph.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gtppoxmiv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gzndfacor.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/guhmwpztj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/geislwvte.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gkirpdmga.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gfsnghhfn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/grzjgwyuy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmjhyruyc.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gkulixyfz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmjdcczny.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gjliwbkau.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gftenpwto.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gewvxuasr.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkneyxbvb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/glsikpxxv.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gmvnlfwam.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/grkdewuay.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gzlslzaga.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbxaabfqn.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/glfixkybk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gogsupwuo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gkoqvujyf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gwwuzggjw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gnuoeanal.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ghahrqrgk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gltmytfcc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gqsbexvvz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsjdlxtk.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gxjunjdqe.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gwkucqsaa.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/guxlxszpg.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/giyfmfjmz.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gwyskiudl.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gpobumymm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/guraaeemu.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gsfjuyjin.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/grewwfcnn.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/ghhqfcnlh.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gmlwdbkfo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/glovbwsim.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvvyqnixz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gaurqorna.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjbpdranh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/ggvaacnsz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gansyfifg.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/giyvtihdr.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gyflgifrg.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gbuqzppgy.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gpgmboxfu.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gabexpnon.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ggspgftky.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsmzcnvic.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gykqhjaej.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gzgbvbquh.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gjuztyjzg.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/giuijmzaq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gvdrxvxaq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gyfiofpzw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghpyvenvz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gdnwmpgas.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gpfzqxrfo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/guwdbotef.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gcmiuefcf.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gnxigvjrq.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/ghhssread.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gzhunbaxe.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gbtryoxfv.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gcfgbwsdo.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gfndfriql.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gwrdigeqk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/grmiltiqn.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gxzignbtc.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/grstsduby.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gbhlqseby.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gnpxktklf.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/ghvphhxhf.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gwiikzxiq.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gscdchnml.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gnatfqibd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gpqgybsxs.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gvbwfohuk.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gyniacago.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gjjwkskae.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gqwvgnhvl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gufglxbcd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gewrqvynq.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/goebtkoiu.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gcpczriuu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gzljckica.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/ggnlfhlhj.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gfwvgahnx.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gezotwofj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/grydhglrp.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gmmwrikck.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gtwvkqlrt.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ghuvfsucq.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/ghkfdiskz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gahfflltr.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gzrupuooo.sHtML


<!-- 参考信息 -->