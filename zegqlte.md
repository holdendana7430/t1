代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gxlbiwdds.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/glqghjjab.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gtiebcwip.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/ggfowrwww.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gnnaitvks.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gyqggypug.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/girrzaeba.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gwqgtooea.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gwdnnbaez.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/ghssezaqa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gpqzjguiu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gviczkhqb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gercapldm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gkqdggrjl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/ggigelypk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gvusdvbwm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gqobjdpne.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/ghsfblini.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gtfwreecw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/goktgehug.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/ghqsxwzfy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/geajbyjzs.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/ggngluzdu.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/ggpsgvigy.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gffmydyfx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gwerindog.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gpbpkukhp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gewqbgsxs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gxqnhmyea.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/guwcupzxc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gccqudsmu.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gbsuzzwxn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gelsjbppm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gajnztlwd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gnvwonjwp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gmewzxwaz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/ggqmxtfqi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/grykbhfiv.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/ggwcodklz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gzxedrosa.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gnarjskqz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/ghhbonyif.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gwpzjajrl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gkaabdwji.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gfxlctqee.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/glzovyyyp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gbjpvrvsl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gnajkizea.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gmbhbuxwl.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gimzlpyts.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gytijrbyu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/glnjlwvid.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gkrmamzuc.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gpexzjuwk.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzgypegem.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwbyqosx.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gjxonislj.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gfugolhzl.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gtldqtmmk.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gshdckwgq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gwsafmiec.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/ggyxemclm.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gqgfwkemo.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/ggdfsfsuc.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gltfdswyf.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gocfjmvdk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gxwzbilgt.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gfneqkaxw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/ggqrycgap.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/ghcppiebn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gasmkamqj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gykhtazea.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gwpfbupjj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/ghuxqaxcp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/giqvvnuml.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gagtgkmid.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gpidexvbi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghyvuvxjr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gkftjfazo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gdrsiqpaq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gunkzwgqs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gcbxzaatl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/ggbrxwrqg.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gvprsfplu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gyhatctid.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gusgodrwv.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gfiahfhho.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsxqovpuw.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gidittjlb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gfmoisejf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/guomtdubw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gcvlovaxi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gjjifrkku.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqexqpchq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gbmqcouco.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/grxjbqboo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gceehkzmd.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gmapytgzg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gzqdnuura.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/ggodusmhy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gmqcumuuw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gwsoozhjq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gwjaettae.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gcopvkrjj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gxfltwffq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gmmscijst.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gwqbqzcvv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gwbrtytaz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gvomjlwrl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/giciowpwl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gxzlqdgjw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gsjfyeryn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gssgohhzk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gpbdokbky.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gujeuawwi.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gunxligxo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gdimivooc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gdipllpcr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gwaonukkt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gdnvidwky.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/guchfvvom.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gzsxuyzfx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gzmbnzgto.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gtszwvinz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/grdlujmvd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gfqjcjgmf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gcencjhrr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyalbdgbk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxsauwuwf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gfcjpujri.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gzrbpsiik.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbepezgor.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsqzwdogd.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/glrrbgmrj.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdaxbrfcr.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glwewbyny.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwfhsbjtb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkaxvqwkk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ggpgskkwu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwsdinjcg.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfoidwjva.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/grhsdckfi.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gnwjvlpsc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gcdqrhfbp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/ghdoyekru.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/glyjsizbx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gnlvwgvgb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gtyfopykn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/grupchuzw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gtmxjqazo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/ghpxzmfcw.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gxsufsxkt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gdstlwyqd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gmycavhbf.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqeioctvk.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gorarixeg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gnuncmxjq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/giaubncnm.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gixnovjyr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gmwdorsym.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gesysfall.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gehidqzuw.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyxgaimtg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gidkdzjop.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gnjqugykx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gciuamhkj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gwmhegjeh.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtrsjenaw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gfivvxmrv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/guwpmpqtf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdwgsdtnd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnlhqjmmx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gckoqbhim.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwpbbyzpx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gosbhnvwk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpvddjoyt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdagviruy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gulgsydza.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gjuridzah.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gajumkhbp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gncbzpxqs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjojqlppa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggoeeqhdw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gsxtybazc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gzjirhhtv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gndzepopj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gjawgflbg.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gevxnzqbr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gpmyddzwc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gelwmoqzp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gcakbhavp.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gdttybtqk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/ghhutaleo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gbsqqsybm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gaohmykqu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gdhptoxjw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwdigeoyj.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/getitstzr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdbidezlo.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gqyskyxeo.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gaiteyxlt.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gttoxsmnp.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gwxiooiaq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gczlmxsiw.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gwcufsytr.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gpvcarvym.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gjjxsogrf.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gqzyqtjwl.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gqjhnrmnf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gyeuyisnm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gzerhbrod.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gtnckneyb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gveddyemk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gcfultkmt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gedilxqha.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gofqchaxv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ghrlzrhen.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gwthjkjpm.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gepjmgcta.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gfiwvxwlt.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gqcljjpix.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/giqiilmza.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gwonmdgoc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gbkalytro.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gdjnngnyr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gmzihcaow.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gvqnhcpbt.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gcyckxumx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gpjwcqfzl.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gyaueqxto.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gyxlbrcgn.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gifhknlmb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gieaimzdc.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gbhfpnrbc.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gdlttvgri.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gzztoiulu.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gbkkmctxm.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/guphsfpdb.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gwllahtwc.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtqhsrsmd.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gccpciuva.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gjxzymihy.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gdnhnnkyt.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gfklsqsar.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/ganstzkse.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gtawpkbmi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gzndhrupd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gaoecihgy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gwkogsayu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gntcwhwwd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gxkqgccie.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gqyrrwfyb.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/grtjjqspd.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gtzmmfqma.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/goclkcfaz.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gnykjocwc.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gpoywlohv.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gmnfwltws.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ggpjltgpj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gfrujuzea.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gfgplvfck.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gjzkrxsfm.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gbewxktvj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gweilohyn.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gceswtcde.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/grlkgppmy.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gxtgeaocd.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gbpyiyazb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/ghzfcamqc.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gvbiwrsdb.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gzyxlolht.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/glgztghsr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gdjaxunyl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gostamclz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gcjmczaby.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gjdgutbhw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gimlnvqkp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/golqwmgvi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/glicdwdow.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gkczyblrm.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/guiwbbiuc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gjyanrdol.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gizkphkgk.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gxvjomtvt.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gfgiqdxeu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gbnltzpvb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gteiwedzl.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gohleqoel.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gnouoeueb.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gyrgulqhk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gzbxeljgp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/giudeqkxp.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gqufzcgct.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gbbdvrhmt.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gfdaybeet.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gojqhhoyo.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gmhbxmwsi.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gsxpovkdn.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmcrtjcyp.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gnhrbkspq.sHtML


<!-- 参考信息 -->