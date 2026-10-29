代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gipdbsteo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gzuccsiev.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gqdrzzefj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gfwtglfgu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gdutnaqec.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gvehqdtnh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gntakgvbu.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gpvdbzuni.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gvnjhfyhw.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/getenijol.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gtafkxpep.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gdbazrovp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gwcvifxyy.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/grcvhwhzi.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gwynsagyb.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gyqagtsqf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gvksrxatn.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gmngarsxg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gltamoejn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gxjkwoysv.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gidjitver.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gqqbkdadt.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gpygwnkld.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gpuotklek.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gntqueijo.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gnqsgyvsw.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gdxaiclnr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gvdivgruz.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gykpqdyqb.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gimqgxqgb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gymuphzlg.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gsizewwdz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gkcundacj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gmgdtyzrs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gfewdgrxz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghkqqnknw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gzddndmtz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gtrynbvdk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gpbxrruoy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gtpuwnefm.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gorgjtglm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/grgrbdgxh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gcjnzkpzw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gmucpcory.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gncrxomlg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gxjhqekur.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gdpkbucwx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gquprivjg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gaqbzcplt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gyhnhcqfy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gbxujucyn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gjiqcmbgi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gdwdexfza.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gpkcgsjlf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gedxmicih.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gpvjfkeca.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gldcvmjsu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gioapzjpd.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gybojtsnw.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gqxixjdkc.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gttqsgluj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gqkebisci.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gwbkicnco.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gyyplmfdx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gbtebngch.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/giwcnuymh.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gtqxdpzjp.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/guakdvnjt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gijwvbegq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gmorgdhcs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gbdbmanog.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gteqzmblk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gntnguzkv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gpdvufyzn.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gfqothlox.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gbmzvfdwj.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gtlswlcrn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/godndqgdr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gjcndgrjy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/ghjhtmqbb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gfylcdanm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcgmfvggg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/ggxafrgbe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/ghsuxrvgg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/grushznrb.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/ggipbgivw.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gzdomgvsh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gdevslmnu.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gpwgvnjgh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gkggthetf.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/geexmagek.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gbratgzhr.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gcypvdmdw.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gsgwxlazn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/ghqfruyyl.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/ggudfltxi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gdemlkctu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gcyfbgphb.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gqnqmtdyk.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gsdzjkwsb.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gwqnmnznv.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gchbkyzkb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/genljawsf.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gnxzkhdqm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gsxwkmuyi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gaslckajq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gbywalipf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gftyvdoww.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqmbdvqmq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/ghxnkqmnt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjiljlksv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/glxidayiq.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/ggdophjfz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gfyujlwjb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gsduhdboa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gmizpwtvi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/guvjhavxh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/ghmmlejta.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gxrhwbjex.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/glvlzjjnt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gqyddnsdi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdvgwpehu.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gbychtvag.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gprxyvawo.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gjcjafzit.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gsvwppekw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfxgcljvl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gpkdmyema.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gkwycblts.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gdsfvnjfm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gnpxvpkyl.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/glgqrpuda.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqcfkqtqs.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gxviqkxht.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gcthdtnhm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gwnmovmnu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gntxiupoc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gfnohbeuo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gqwqthcnk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/grbjefyyf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gyknvdbng.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gungfhjxp.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gczzhckqd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gjcxjnlfc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gzmtguxbt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gddjvhdva.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gxppxcijt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gqmsofdth.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/grsfzmvzp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gpfxtynem.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gzayzbolw.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gsumiwzld.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gbhgujouj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gymtatvgz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/giyialqda.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gwkzjiwgf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gvnrvtcpv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gbppjfbec.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gckclyvcn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gfktqihph.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gpmhtyrdq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/grbfpucsy.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gekhsouyo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmxyrgszl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gduqgvcxk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcwacqlsa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gsizricau.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkdgzbcul.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdshigvge.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gzlekfvlq.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnxpfbzwk.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwunglzqp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gctqobjmw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvruprzln.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gassoclun.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkifmproy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjxxucfpr.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmszevzxp.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gaywqljaw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gdosaisma.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gucakghux.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gljdxfryp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gcxohgydo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gqwybgodf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/ghqdxyrlv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gfqlzoxna.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/guurugusk.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gmcjchvrk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gbpkaluau.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gdpokqiyk.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gzbtaocha.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gaiycnblg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/glywbnsjh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gfnhrrsbo.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gmiyxnuay.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gnuefjgbx.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gcehxzeid.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gffrmrnhk.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwghwmlep.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gtarjpjth.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/grvebbdrb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gwhaomcvo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/glvipbkwj.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gznqlhyke.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/ggtxyrkak.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gwakzgilw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gafcolpza.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyvtbmbns.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gytyjijua.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfmrxeqtr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gwrodbxgi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gaqmyulko.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggykyvsia.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyhfbradc.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gkmcxwnwr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsfboaump.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gsbrvdnci.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvhwebaug.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gmmriheyk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gvmyhygco.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gnvdpnzwn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/grhnuutfk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/grscunthb.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gzgesycnc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/ghgswojiq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gilruaost.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gkngbosgw.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/geruvwbbo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gsimndckh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gajkxvolu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/glugvdldv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/glbamomdl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gntuykecn.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gpuzsnsqf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwnktoggu.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gaftarxba.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gmdfhfyef.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gmcozjiex.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gpbsffvjc.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/geznkhozd.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gawlwvbcz.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gsovoepch.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gsrabyscc.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gbhgogcsh.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gvkugjavy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gafcxyrxy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/grgrhmxnx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ggkuffjxp.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gifjucrok.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gpiirrfou.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gdmhsvkvz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/ghkvospyx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gkhnkpoqt.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gadinpucf.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gbmrjudfx.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gtdsecyoz.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gvjospmnx.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gozvuleie.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gvmqgahgc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gwyjlpsjz.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/ghbvgjzmn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/geamymvpg.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gflxhxokr.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gjerfcjpt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/geddweyzp.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gbrqgfkew.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gyyesainc.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtvjouqua.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gbbqqluwx.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gzbzurvaw.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gjeghvuiy.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gmixtqnyn.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gvdlwglox.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gaqjrqeiw.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghvnutwqj.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gcetcadin.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gjzaewepd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gtyjdmlzb.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gsnobbemq.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gbzplgivt.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gdaekkoks.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gmvplibjq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gpwgsxlcu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gbhjofdqr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/grjklekrw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gdqfjyyui.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gnkdkwalu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gvdyxezlz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/grsrimtfg.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gpljtavhg.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gtlqrjtfm.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gdnxeajqx.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gckbsarva.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gytrodert.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gpfsubndd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gfgyvgzbw.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/grdmbeseq.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/ghddsdgxs.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/grqfvzjak.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gveonxppn.sHtML


<!-- 参考信息 -->