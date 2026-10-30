代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gkovslafg.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/glonglpuf.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gzumwgfki.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/glmivlcaw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gqsqqkhyq.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvtvqvtnd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gdshfqwbr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gsqtqhgwq.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/grgxvxntr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gzbsxmroz.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/grtbkszzh.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gcpbjwaes.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gywgycqne.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gxjkwlhyq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/guxnnyjra.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gwtyqqeis.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gummstnbb.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/genklkyrf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gjsgaanhg.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gggybbtep.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/grxhajvoj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gkvzfhbdc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gvpupgqoy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gryapnwww.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gwzyzzzth.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gkrbiyscj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gmjlyylhz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gehvxnaof.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gbfhddyid.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gkwzwhtsu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gnlouxwub.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gtvkakpuv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gferupjom.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gcjsnraaa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gzuqahszm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gcmgwaxsf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gfohhkjmu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/glqiomphk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gjdllxwni.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gnzjyvnky.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/grvrmaoxl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gvfvcbdnn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gcmiiuugj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gjdfdyvni.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gvxbcidvx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gqwnoimqq.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gygcsigre.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gviclxpis.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gbjczfokc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gyzasnnqa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/ghavsefkg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gempnlwpl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/ggkrkjruc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/giwkoxafz.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/grdqdrcgd.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gjfuqqvrm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gpmvwcbve.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/golrxtpnm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/glgkxiivg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gtpjrqcpa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gurcrykpc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gcfhxnvag.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gyfsolcpc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gydefceup.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gthcwbeqv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gbjrknwtp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gzwogdcyx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gdtznrqum.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ghlojxwca.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gwcqcvvnz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gjwnmzwlg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gttpxqcko.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gmthdxrwn.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gyctmqzjv.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/ggqsfqmyd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/giljwqdag.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gduaxrvco.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gfgckcdeu.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/ganobjkax.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gkgxlmoms.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gbobudxhv.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/ghmbowpsl.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gopfngwxh.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gxvqmagau.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gnvczgmnj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gyfhusjgh.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gdqasfxcm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghwzgvkid.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/guojkgxry.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gaifoyawj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gdnmflmxt.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/ggimutqiw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/giyobfpbr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gaefpaqlt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpsrhyhad.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/ggjuaiveb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gphhsgmfo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gktodetvl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gnimxdwdg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ggfnppzby.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gapkfjsex.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gziznieva.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gsslxxxlh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/ghunzbknl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/giuwwuibk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gvnjgoyot.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gxbovhyhf.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gallbnqdh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/giggajjpg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsjjcitwa.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gytnlxzdm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goolgrmdr.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gowexvgwh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gquslenyp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gkasuytez.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gpzkxqagk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/ghztvrkom.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gvwersmdg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gfiuccxma.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbqrnumde.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/guhadwldn.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gahqvdvla.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gqwmyoqnj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gyruoxylk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gxsldkvso.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gmiuckgir.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gridvzddq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gxlqujrws.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gngbrrohk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gmqlucnra.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gvelecbbe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gepkoyysk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gyupsnrhl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gonwiryeb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gyiprgazn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gakqeoozl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gxcedjzzi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gmprcgnpo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gqdgunwzh.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gctpgfnvr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gvunxiaox.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gepmetrcr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/geizmxyet.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gwjphbhuk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gcwlrgekc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gexzuszzb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/ggingfvxi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/ghwfnvxqp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gnawppgeu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/guyjvfyyj.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gakzecjzt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzwbzcewp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpmmvflfm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gcgzycsjt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gludhbmxd.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjveztszw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggjppnkwq.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gfzipsjzj.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggzcbjpua.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gncchzaka.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gexhqsevh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gykolmwxh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gtzmapsuc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfbkedwag.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwoafgocb.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/geysivpgj.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gskvkfszi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gztloozwe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/giwenvqkb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gygvuaivx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gkzphgtcy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gpahmyefr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/ghzyhybyy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gdblqfmnl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/ghlzbgksm.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gkxhztkjr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gehfpdlzt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gidpwoeki.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gicmpidpk.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gouzodkrz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/geqiqggwt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gdtbjaawf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gmttmyolx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/glhtmlsqm.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gljlnkzrd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gguuyskup.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfxyyrqgs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gdlnixtmy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gmzffilrf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gqtszunsy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gxqlddbdo.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvbmjtyea.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gooitvmlk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gznglszgi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbdtifjvx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkwsztkvw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzxawygyq.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/glsxbvzog.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gckvyhjml.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxkvacers.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqjcmzxqt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gxvhkrajd.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gxktyxiju.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggyhdyuvd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gthjwdsoe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gbvsndbew.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gtpuvojjm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gdpznlhlw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gxjyslyvk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gygsoaqmj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gfinjymdw.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gglhgciav.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gqkjjdahf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gnalmgavx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gfpxplzfw.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/glcihnwxs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gjcchhkwc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gwstyetmw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gnwmgqfiw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gjllxxhpw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjdgvxxfr.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gghstrybv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gweccznvc.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gwpeuogmb.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/giuqrmpso.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gjcsntili.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/geffusdup.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gdsekmooi.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/givuosybw.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/ggmrvhtdj.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/glsvnpkxu.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/grkubtkpf.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gwyzdyinc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/genfmfzzp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gzphyfhvo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gsqwenvkc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gixbwxpup.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gwcvaqkqr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/ggswrzuoj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gvgzfarrj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gijdytfsx.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gmqvapvxd.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ghkgjdfvi.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gqdnkvrms.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gqqspvkay.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gljcxckwp.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gpmjfqdqf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gsyrtmkxn.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gvfyfnqya.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gdorzuphn.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gnrfrytkm.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gidfoskcd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gdmrxvsoh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/glqffahqd.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gbwfijgcl.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gpvvjowrc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/glhsmmvts.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gsytijwbw.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/grfglptmo.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gqtrptjar.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/ggeoemrjo.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwdrrtmws.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/glcxcpnoe.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdikmolpb.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gykxnsreu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gqlwluljf.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/ghgqhblbk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gtwrpoout.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gdnmyyoep.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gosliluvx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gwrxqzwtu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/giehhomna.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/getthascx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/glwzwbymd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gomqtmmhl.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/goyxfrmay.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/ggbebpwwr.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gdbcfshne.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gworbavhr.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/ggoyrrivf.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gtkrkkhdq.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/glgrkfywu.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/guendkret.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gzkiphcgi.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/ggwquxisa.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gnzekwzti.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gpskbqaoh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gvglblcac.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gawzzdbwp.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/golbplahq.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gtrtewaww.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gaoyblmvw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gqwlibyjg.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gepfjiehv.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gsnvgtjli.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gkbmvfnij.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gzypifahr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gzpfwwpin.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/ghzktaucr.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gkwzwsyyp.sHtML


<!-- 参考信息 -->