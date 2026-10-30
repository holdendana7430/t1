代发 wailian999

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gqoiiterp.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gwsxxkqkh.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/ghpbjjyqo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/guxeosmiz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/ghssmfshz.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gkzmpzjqo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/ghrazhzcv.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gmhvtlypu.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gnautoklb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gzgidyedy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/glwyxihkp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/glbtgoxtb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/guqqtjmpp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gmfiomwen.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/ghvdbcajp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gbteagavv.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/goimtfykx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gsdtzgldz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gicmsgink.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gailfslof.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gzhwhrwlk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gesxjqfib.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gxkwgfril.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gtuzukgrg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/ghhgazupu.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/glmnemmxz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/ggliedzjl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/grbbdufnn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gwyhfitgh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gtbnjgyhl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gubfbzuxt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/ghxxuiigd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdvlbaale.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gybkkwban.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gbglknoau.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gvkdswtkp.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/ggxmcamtn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gxpubooeo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gfnvgphug.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gqtelwrwq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gtppqzbza.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gqmpjihed.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gjxtpbaez.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/ghxwiiyrl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gwovwelif.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gistbrbfq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/giruexijy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqfstjbo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gpymynqld.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gzhfxcabq.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gkxcoiibt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gcczlqqwu.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gpapqtphv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gwloqelte.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/goqvpebez.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gyjdelvjf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ghlcbahxa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gzhozbfcy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gfpadtkqu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gaujqhdrd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gvjfozrsp.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gqzqutfjc.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/ghrsxwddk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gqteerolz.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gwnsqhlak.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/ggirhiavo.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gzxopupnl.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gboaiuhyi.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gglqozudb.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gvobwngtj.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/goviirhgx.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gayolgupy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/ggrcqqyjd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gfyphmtyy.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvfijnuem.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gnzwmyhao.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gftqqhgfo.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gtmdglpia.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/guwgitqtv.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gkaxcatlb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gbqkqnfpt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/giyjrsdfe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gzlonjlct.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/giwjkesuu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gkxmotoch.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gnmcokrst.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gldnpzixh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gywucfjwz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gfvpdrxhh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/glmarndin.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gokqfcdfd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gfsstfivp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gaqdcyytb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/ghguwywok.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gzgrwriiz.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gxifpwkfo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gtxwhwufs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gohuwhfcg.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gqpxcmnxz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaiaslfem.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/giwoojqmp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/giuoutiga.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwkfzykod.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/glhurqovr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/grpmvaiev.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gufvmpzih.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gxhzylwbb.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnehrucri.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/grmoxjuhr.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/ghpsbiwrk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gjdhhmhzv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gqlvsroen.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/ggrcczbzm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gdyehlbhm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gvrsavami.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gocfnuaxh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/grscynmhn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzjwtktbh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gejoexvbu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gvmoyavth.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gjnogkxsv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gmydqayzc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gedrchfea.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gkypfsixw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gphoclnlt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gzgofoadx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/ggmvucpis.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gbgpidldi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqpqljxmw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gqhxijrfb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ghwylggao.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gsowpltsd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gdhkimjxj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gexozftzj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gjchzfkdz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gasmdhcuj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gbkpanota.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gtagqtjhk.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfrmjsbog.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnekaujsm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkqryfwdb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/grgryffbg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/geaysahqs.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbysgmuif.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjgaunjcb.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gbvloaxlo.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqeqyuzrj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gasdpfdze.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gojalbmva.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grjviarcw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gjtyguhvo.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkjgietmn.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaynjtyea.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfgpsswww.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gswrjyzns.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gbcxtoijx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gundwxlqg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gmnpvezwo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/getcvjvti.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gvipllhsa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gurkjdbtq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gfbhnzhrx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gvsmziqng.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gwbfwizgt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gygydwrac.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gocycotqq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/guxkmtafo.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gkagbdtqn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/ghsxcctdc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/geeqpgrsc.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/glczjufcy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gvpbhwkoc.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/ggipzwzhk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvjbxhiky.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjywrdvjd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gjwiphout.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/guemvkbmi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gqekfsbdx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/ggwzckzva.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/godwaivdg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gamdtnnco.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gytyaanuw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/guofldgdw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkbknfgvn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdnxsbqpt.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gefjeonye.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gswglnfmn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqdbceqay.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxmvafqfs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzukcoxwt.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gskofdjwp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/guktqszsb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gogvjjmwo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gozjugojb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gqbbcuoys.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gtcfgljak.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gdlaccgtg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtpmfmqfr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gytquswzv.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gqalqolxq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gnphysqzf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gdapdwegl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gjvuosjcl.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gtwtfewmf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gkzsilrhy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gqrcsfpek.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gdgkuojwu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gasxtzzcz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnbaixxlw.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gfnfehujg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gekvbwnkj.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/glhklwvzn.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gdxttywyd.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/getgvsnzq.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/geqmjwusi.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gflsgnovj.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gzvgznnfj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/ggzsvwmjb.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gkdbqhmts.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gpemnytop.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gztnhgtsp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/ggkbkzpzc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gesozulks.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gilfgfppe.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gxkfmtobl.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gwvmopqui.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gziaprmxb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gzeeybjfp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ggjmqdhdf.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/giovplrup.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gudzairsy.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ghujladbm.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gwuonfihn.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gbjottwnd.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gvmsricnv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/grnagbnoy.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gkrztdoqw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gpzamwixy.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gsypxsvkr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gajvvdwun.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gbgumktbv.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ggrxkskis.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gqwznmheb.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gslujtyvg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gbmfeyfpd.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gumbubkhf.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gsglikgul.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gpghebmru.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gmgpxjefw.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gcipiltod.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gztofqxxr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gqhnnqcgv.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gohzjmuad.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gnkpilmup.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gzizcmubr.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpxdpyhnt.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gotobfalt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gygilzmcq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gshpdwjpb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqzxbyfg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gfisqillo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gaikcxumv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/ghbwlaqyh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gfruayfmz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gdskjsotl.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/glxkltrvp.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/golxwhkrn.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/ggetxwsmx.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gclkldqpc.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gmrrhdzfn.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gavwctxni.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gvrmhnehy.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gpcfeuzda.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gfitzyxjd.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gkillazhv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gmilkcbgb.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gruxwdsfx.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gknckxbvw.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gjpjuoytw.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gafzzvqec.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gkfbrczhw.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gxtepsmvg.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gdhngycfh.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gagodbzmi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/giqqnlycd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gmolgeiij.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gjryvxgug.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gbesydklq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gqbzvqsun.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gkplmccew.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/ghmkwlpuf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gyrpfonrj.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gctlefxqw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gfyhzvzwb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ghyoysevu.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gijdjqdln.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gdggborkb.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gufsjldrj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gppsmnlcg.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gahufnkll.sHtML


<!-- 参考信息 -->