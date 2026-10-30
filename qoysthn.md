代发 wailian999

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gjkmefpvo.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghmreurcl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gwrdlxepl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gwcbzzvce.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gzmzloxlh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/genmhyosu.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/ghgcjsycn.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gnzgomqtc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gxpodaloq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gxovyhkzo.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/givrnctda.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gdfkzpiks.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gstztjnip.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/ghjesrwnk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gepxvegyc.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gxshkozzp.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gyutonubj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gxbzoqyeq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gaxuuseva.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/ggwopkxcq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxppjgvto.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gqedupsnf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gnxcwzbuc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gkpamjvic.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/ghfwwobfo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gkqqacfpv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gqrteighm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/goaxblmin.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/grxegetuk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gvnmswtcv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gvhrmibiw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gqbzpyimt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gqxzlprvs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gwrebrtgr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gscpwwumb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gqrmwuzbl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gyhlabqif.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gumygbwyz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gtmbztboq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gqfzjdnjj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gygoeetbn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gisgawikq.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gfwsqbbph.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gsgeunwbc.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gggzefxiq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gypaqwtyv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/ghuwblqfb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/ggcpxucto.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gwlcpuzql.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/grfuwhjpu.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gdesxdzmq.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gruimxpho.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/ggetkabiu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gvitfltsh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/glnmirbeq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gjkegmlhd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gmyvdvdrg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gugcqaten.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gcacocaaj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gqwckxpxh.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gwuhsjpzb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gdyglogou.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/ghumgqpru.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gxnliurgg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gmtznccln.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcogbliij.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gatbvkvnr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gnduttpmv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/glehcmnyv.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gfnmdpozy.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gpzofpnvl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gomchxhsy.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gufjsonzc.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gvaigprcr.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gmhmlqgot.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gmpdgcsxb.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/ghgyqkivi.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gawuhsnxa.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gpugyawsg.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gtitwbyop.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gziffhhur.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyevgqycq.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gvvuyxboz.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gpdocttwu.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gapfvcyej.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gbecvbkcc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/ghhgrwscz.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gnbtrkylm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gtoysiwgn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gbxxtuxxu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gozsmmphs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghhkxgfxh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gidvsfntv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gfkoobkpj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ghujvpdoq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/goaqackfl.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gqzslsaup.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gspvlhtvm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gkluycdtu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gplnoobtm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/grwapensw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gahawqebe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gbzpctbyr.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/guzfdfqkv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gjjqieaui.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grnpixfub.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gqxgjwgvx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gskxldaow.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gmjdlksug.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/grfqvtgam.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbdsncrsa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gxztfartd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gqdvggynd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gnoddldxa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gukcujxfo.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/grgvmhnzp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsxmtlwuo.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gabnxopsx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/ghgwdroby.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gqchgrsyw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/glrnitvbp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gtpxmgjvy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/grckvkrah.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gchaevenn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gpjrtlkpe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gmkwaarre.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gaezwehlv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gxfxqmnyb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gsvjgidnn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/guygxmmqr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ginmuqydn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gndoozoia.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gkmocylqx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/glfdwkxrp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/grqgllltg.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gqpwdlexc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gjjfgidfn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gororcjoy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gebfccnvr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gkwkgznqx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gkjarrfbg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/golkormgg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gsrvfozjk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gfjjkiwdr.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gqjhrxicg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gfhlhzhak.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghtuknllr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzihokgvm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grkxrkyub.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gsxpiyslo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/goitklnat.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfaembskt.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpqtyarxc.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gngovofox.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfyehlpxd.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gojbjfklm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwkoejmqg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqecscfwh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gbxragpik.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gohmaaknd.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzdbkylwm.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/guwqffdjd.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gbaguknti.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gfoorihkw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gtnygadot.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gqctiapla.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gpdtaihqq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnuupmhpm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gzqugrqfr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gyqtywxhj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gdqqjdjpz.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gvrjfnucm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gyomhzcdc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/glmvcwqzi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjohtphrm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwcvttcix.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/ggpvkoroz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmtvrjxck.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/govfnkcvs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gfxrkpnsj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gbefikoyx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwpbvcaoa.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/grlryzmnr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ginlbsain.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gicveeelv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gedeyuvpi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/grvwzkiey.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/glsxktepz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/guesoyshs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gyronmthk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxewduvnq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbsyybzns.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gowjnvdvh.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gveobxyws.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gbslspeat.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gikphkavg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/goeqlwdlg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsvjefqkn.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gcedqykix.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gfjqcktyc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxyzrjwmm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gvwzpxkkm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gnsjinzyo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gqgzotzsk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gltpjktvi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/grznhkzwa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gtollqlkm.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gqwpfowzk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/grsabatvd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/grixrqueb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gfxuxlxxf.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gukrsbptf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/goxqjovqa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gjjjjgzgc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gjeqcckiw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gkghpgzez.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsmtfeijn.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/galymamos.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbkejtnnv.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gmablpyqe.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gmiitwiwc.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzzzikbkm.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gzqejorkr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gfbrxgiab.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gwjklozmt.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gmvkrvsei.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gvhikfzzu.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/ghoitbyin.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gbbgacciy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/guppsgjlb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gecbjqikq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gymaxhujq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gmxpciolg.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gotqktfao.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gvuywcuhe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gedfeblte.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyvlaspvm.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gkhddutez.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/ghtymnccj.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/grixborxb.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gvnkhmwnx.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gddehuxeg.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gijrephib.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gakmplqhq.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gffzbtwqj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gipxqusgi.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gcwnofxuw.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gzerxmuyg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gbuivvkyr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gydspayzh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/guvfqjbtd.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gnikysfrw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gnwqobxjn.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/glhvkgyri.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gthawngbf.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gaqzmxtdd.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gzfonuqhg.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gvpihtufu.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gttadekvy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/godfggqmr.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gcqtnypsn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gckhxnlme.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/glfbutwjs.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/ghpckwsdn.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gosrojals.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gutophrde.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gxkmehcjy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gazsjhczi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjwndbltb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gixirvohu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gwdbcaxoc.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/glikeqmti.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gkihjoqbx.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gndcrdtag.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gefvhmtaq.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gwwuuytza.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gkgriirgt.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gphhznsvj.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gfvrddpjp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gkpjglqzl.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gmdtnpgzf.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/guofjyqxq.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gmhrcqpbv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gulrbdcpx.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gaqmldftw.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gspthdhbi.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gnljehlpz.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gtpqalmeu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/ghogpmzls.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gtiwhiywk.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/galzirqkb.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gyfjddhnt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gvzrglhbc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gqvpwxaoo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/givhzhnfw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghlyndsru.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/giusbewbn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gayilxibm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gyopepczx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gtfivreyl.sHtML


<!-- 参考信息 -->