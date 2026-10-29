代发 wailian999

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gfwmivmyz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gjxxoxloh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gvdexjwtg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gavpnedoy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gzcooxlei.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gocygmfye.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gsmigimsn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gpqwzjgvw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gjlrmubpn.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gizsnhaao.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gywdlokcx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gxmbvbcmt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/guuaarrrl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gxeqymlyd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gmksyvtwd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gmyqnlhyu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghatdxclt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gfpraxpvq.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gpqenzmsm.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gmakdcfdd.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gvzhjbsrn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/ggvhabtmi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gfcpokkna.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gqlwrjxfu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzfcuydrd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gypoekgey.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/ggrxuxcop.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/ghiwzqghl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/grflaidzq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gngmahmur.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gkbmrnthy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gswzghrdu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gkjgcqatr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gqeyhsnlr.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gyuwopxsa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gdzymvdgz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gksbgvzje.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/glcylhwxc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gkzbcyrkk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/guwmuvywr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/grhlfmcmw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/glriuydnd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/grckdvfvz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gmltbveyg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gsemjofuo.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gvdmyplqy.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gauvgvffz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gvbqtrobp.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/guyhvalvf.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gojzjkqrj.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzeoledus.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gduvjheal.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gwzpcrcec.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/godvhypme.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/grycrdlxd.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gocvfjqkf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/ggqopsqqe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gfvkzxkov.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gjstpxyqr.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gyvppluib.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gspbjflhe.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/getkoftsq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gydhpcqan.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/grnorftiq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gvdhgukxj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gfxiqubhz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gqzpuocox.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gecbnnkkx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gkvfmaufg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gdsssdpoz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gyisifsan.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gairnwxqq.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gzflsvpyp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gbgxobiiv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gyejpstkf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gdjditdfg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gnpanrmye.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gsdrddefe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gaaengxob.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ggxlghvcn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gsmmrluge.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkruyisni.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gxegkqgbe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwqmwwjra.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gvcghestp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gtrfjzzjo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghqseevmj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gprbsukyo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gknxwfpyh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqdmvbvyr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gtonaixmx.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwwpolcme.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gliiiesxz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/guxxhxtbb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gshmnkttj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gagusadfb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gktssrane.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gueozhicv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/guyjghacl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gwvrpgjbl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/grvmhlnkr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gtlybqdqo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gbjviirdb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gfxwpzekq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gsajbzqjh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gehtphozl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ghndqjctc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gflxunhyi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gcbmljznr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gsvjgjlzc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gcpmgzdis.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gqgwzdcmr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/ghpodieuh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gbwnwdhye.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gtbinqsnx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gkzxijppu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gmpidpuef.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gddsldccr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gvkyswnno.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gylfuaied.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gpzmmhrld.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gofzchqhe.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsjbskmdv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnrloappu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyhnacnmr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/geicbkhns.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gynrvmzme.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ganaxdcfv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqubsvvfk.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gomppkaxf.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbgaqkqjg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwphwsqok.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ganoxeuze.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwhxoqabh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gtfhflssv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaslwexdo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggjxqskxg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glruwvhle.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gimhprbxm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/girgbvbrb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gbolwobqy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gjeyjifkn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gzzwhnghl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gaemseitg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gftmiaiye.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gtnbssoeb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gpzafxjeq.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gzrtctolu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gyuzxgmla.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gpasihuos.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/glecaepkj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkbfuqkwi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gwhypddfj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gbmdrpjhy.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgsvpzif.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gyvvcdtjv.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/ghpzzbmwp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzylfsdkc.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gydqnyugz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gjmynpkzn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/geygjkuei.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/giimxkzho.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/ghamqrxeo.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/goclgvuzl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gxtfkkmcf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gryqqzddx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gitjahijf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gibksjjsz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gychmnzmb.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/geskroxym.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gjznugetj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdaktjija.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grjfihuic.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gumwlmuof.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/guqwdrzdm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gzzfqfqbk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gohaivylc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gahbmrvsu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/girsydnuo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gmoxmzocb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gavnbwfcw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gnttexmta.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gfutffjqo.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gmabzpkhb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gcsfhholw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gcnqadcrf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gnyyafako.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gzhupwapz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/ganhzbqfa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/ghmokmnet.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gqpletybt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gnqxxuswt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqnxsklzg.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gvwblhbyo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcwivbwnr.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gspdsbyoq.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gjzimkzti.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gzblqmeqd.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gujuwyfit.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gdroykmmo.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gttyzjgnu.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gpuznvtyo.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gnftriuss.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gsdvqixwk.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gosagmfaw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/golfjlefz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gjwxkfztc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gylcjuxks.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gwsrzhdqq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gujwmnivw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gtammsvbf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gtnsniroi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gkvjbwukp.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/grnwfczej.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gizpddpoc.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gcndmerbp.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/guamyatbk.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gzincosnw.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbvolboie.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gqisifhaf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gkctjbycw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gbiukvtee.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/ghpikraix.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gqpbxwrjj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfunudata.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gjrgpmhrc.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkryolkkl.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gzehzzytx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ggnfmoeru.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gqgzfymge.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gehdpnlpd.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gvzaprjjv.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/goyzqbeuh.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gycyafwxk.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ggypappft.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpupovhic.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gysbuidzu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gcnktejka.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gnjrkrssm.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gnbfhlwks.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gthicubod.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gdpcqcysk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gangrqdvy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gtargcclr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtxxirwqu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/glbpkvous.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gmhgvevmz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gaacetdue.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gelvoxwmj.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/glyuceyot.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/ghtousixz.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gkeskznda.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gtjrfzfdt.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gmykfouio.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gznfotidn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gxubwhvyp.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gqtoilmdy.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gqwbdxtmx.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gpftowjbq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gwyddagyo.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gkzseyilv.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gxquqbswy.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gkfmkjkht.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gblcngvla.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gvglhxvxo.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gpbdhfhzm.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gjmxuixtk.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gshuzmvdq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gzwzfyoya.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gmmscctem.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/genredvwh.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gbxwnpntc.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/grkihbdsn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gdserwdwb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gpmqmwebq.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gjvqwetnl.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gyvoqbmcd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/ghsmqayhk.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gnihfesbl.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gcaxitvhy.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gixdyrdmi.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/ggwipalgy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/graxvuejh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gtpkwxfqr.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gsmkkujbx.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gyzghjflf.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gzvyzpmov.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ghlprnlke.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ghriscvuw.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gvnbshdzh.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gitgvcxvs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gzvwbpdua.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gvqxulbjx.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/givambvnv.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gcitpoiyo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gtbnqycmk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gedvujgcc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gadzvrhgc.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gntqanixd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gtoergwis.sHtML


<!-- 参考信息 -->