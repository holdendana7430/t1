代发 wailian999

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gxyiekowd.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gqxqbzvhl.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gldyesmhm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/geawelcmn.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gyyqnuhhp.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gnoarwwey.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gyjxdmmaf.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gnnbhsrqb.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/grhoeuwoe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gcdskpiqf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/govdlsion.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gmrtvcibi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gdnwrnxjs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gsbldopcs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/ghycphrff.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/grjdrxcay.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gjfecmbwn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gesmdjrug.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gouizjtpl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gkeftemll.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gqszyooth.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gicjdmalu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gkqohnjqz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gzsehqwso.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gsyildwsc.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/guyqwsuub.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gtyldvdwi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gkfzieked.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/ghsvozqpd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gpkwvltkt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gmgriglmo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gfkmjaxhb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/goxtlwnlo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gratjvfjb.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gqkspfqvm.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gyrvxckai.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/glhgvyvzv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gkpegjfty.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gvfvnncdm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gepbzomot.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gaidcuuhr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gxjkyiyij.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/guoqwhuop.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gzfcxtkuw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/glnprvopu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gpmktlbff.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gvxbytwzi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/ghjcootzd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghoonkgmc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gvdbvbsar.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gpuverysz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/ghciqjatv.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gxtasmgxl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gekuqpoty.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/guxwrjfxd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gnwhxwvdk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggxkwlipm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gcgpegscc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gulnpwjlc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gusdcodho.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gzomgcnrb.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/glwrbcnaz.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gsbtxqlwn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gbdwzdqty.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/ggakantww.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gyshfpawa.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/ggvzkrlxl.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gykuxwagn.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gnoaumant.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gikusddqp.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gpwebpwgz.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/grdcpzwaz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gbenxttwk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gfaufjjyv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gjytpafny.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gydpfztoi.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gdqefycvh.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gezbpqvyb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gvhrgzkfw.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gtfjlluxy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gzhwbxbqr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gullarifb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gxhnoixxd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbnfoazqn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghaaximdv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gfedhahfx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ghkvkwbkn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gwmljiyrb.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gnbfkyjib.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/geriyzggn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gqzpjxyfv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gbfbpitfc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/ggipksrcj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gvtuanxre.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gyshxnhez.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gkbgruoer.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gdqrekvpv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gciihuget.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gvfzuameb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaupvtlcd.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gviczlmkp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/geprmuyry.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzofukweq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gbloeefuy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gcrcwumon.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gklqmrofq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gqlmhgsnp.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwwnbteqj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gsdbajzsm.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gouinjpmc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gnghkxspy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gjdgvhmsp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gqakhjsvw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gdjcotebt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gytcwhrho.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gtyxqcqfx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gsjemvtbd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gmjhiqyev.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gvdlrkfhy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gdbtidesn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/ggwgpkhrg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gisieewdd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gndqofhud.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gdeieiqdv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsyitzwx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gahwlbxht.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/groqwajlp.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gcmnlxkqf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gbhjhbznm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gqujmqeke.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gcqgwsgdc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gxrmeqqlr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/glzyiqerf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gilysthro.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gdkanocno.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gcsflokkh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gbedohima.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gxaspeytd.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdfstizxr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpozosdpe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdyezghbu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gagzprnwx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gbfxrxxlt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkgdvnbkf.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzlbmwhuy.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gatlnqdki.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpfaraeqy.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfrkwsprr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkuzaunaq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxgokowpb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gexhyidun.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gatqsupur.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/giruofflj.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwphatfgp.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/glnzsnowl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gkjgzdppy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gjkrarjjh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gzsqhigkg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gpkykdudn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gcvkbmxhl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gcfnvatbu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/ghhlocdll.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/glmsxmrie.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gzzfzfcki.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gvvdcgyrd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gkuifwofl.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/ggafltekx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gzanaarcx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gkfzxoifp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gpugitemz.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/glajfvcku.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gqginducs.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gbzcynyfg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqjlxgfkp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grjaocbrs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gzciisuez.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gyombrral.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gwmymtjfu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gickflzkk.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggtfhcmxr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gktmyphbl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gbtwrwzwf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdykvruua.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grpfypkhs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfcoagzkv.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbfghmltl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gleafxntv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjnvhjulq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmsxtfsoy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtokotrfc.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gewiuyydi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gidhlkppp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gyjbbbriq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gctynodug.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gmjheemmh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gmhnfawnn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gfppgklyd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/grulgffie.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/geherwtcb.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gvvndoaeq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gdjxgczbc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gjywbqprl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/guzpjdyfv.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gjijvcohg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gfwvwaktu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/grhffpliu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gayypwrpm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/glyylngei.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzrcazlhn.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/ghyibwacy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggdpxcuam.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gmrxvxldb.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gikbpxwkv.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmixkzodp.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/ghtltesbm.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gajadlecu.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gsxmorgek.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gqexscfbs.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gxbiownxb.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gcxqkipdx.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gmokackbl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gjqxyxkgu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/guzkfhlnx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gfoiyqvwy.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gxdysyxts.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gldrevaft.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gdxvcyiwt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gjiukphgz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/grqishxez.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/glpewgsfd.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gpkryasmh.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gjwxjohks.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gcvjdhslr.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gzbfwaoux.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gmohotkgs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gsumcztwm.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gqtyicuec.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gfkxzsema.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gwvtibzkw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gyqxlnyvf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/goualfuoo.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gntuwexvi.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjsvssbep.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gxnxpxett.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gwizylnqx.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gwdeqmmxx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gpcvgctnq.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gcquaewws.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gctanqamh.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gtrauxlvc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gsposooue.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gorhnmwoy.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfkyvipgp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gqvnnorvs.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gwxbrxsxu.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gcjwymbpz.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gugukemli.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gzualyyxq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbckopibj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmlycjvya.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gwpknpqbn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gfudokanm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gbusjnkts.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gniwsxczr.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gopcabpid.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gyispxakc.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gmxnqjknb.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gjydmwujg.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gsccwdbod.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/glhldhkaj.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gfkeancob.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gcncszduz.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gktsdnrha.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gonobmuop.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/geeoindtb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gmpuffmiy.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/ghiisznio.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gaybmokrj.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/guofzkovv.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gdrnwqleg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/glgaicvvl.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gziyszvhe.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gfijduwxr.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gxiurebrt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gftmvahrh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gscgwjtzc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gipcoazji.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gxuwsifua.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gttepusrr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gnjsfksrg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/glqfogequ.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gwuocpmxw.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/ggbttbovq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gnwkbcqbx.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/guqkcypig.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/ghghemngs.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gbisrueww.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gqqklgfah.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gjfwnrlda.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/grgidwjal.sHtML


<!-- 参考信息 -->