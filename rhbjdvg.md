代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gsxygjcwa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gpxyomntx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gtmdptxza.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gnkztktil.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gcybcfjwg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gcametadp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gaxkwhtkc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gpxjunqkx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gogvrvdgi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/geeielgbu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/grahtqbmg.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/glxwajwgj.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ghtfzsoqc.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gttllxbwr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gtprhnebh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gkfxnzrji.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gmsrjmwkz.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gzqejvmbl.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gvshjyrby.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gtcftoswl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gmepxqjya.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/grsiqdwpz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gvpsyoxoi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/ghlctlzks.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gvwfjoice.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gdwiwuiko.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gcjaefuyx.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gugidgndd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/ggbqzufpc.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gamaszmvk.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gmkwkphvd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/godxwkpem.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gawstkvpx.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/glquavcly.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gzgdwifsw.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gwmjugygv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gqoducely.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gmcwmbzhf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/goevdhdnc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gdqugckvc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gzvvvueyl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gdgzcgema.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gtlknbkzs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gfsbhawel.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/guguucggm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gunpzjwsq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gutojxhda.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gqleznpmj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gwvzguspo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ghjghgces.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/guzkucnux.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gobgrsxnw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gfzfshwpp.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gzhemouby.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gkwuqlajp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gloxsmdgj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gebgazjzs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/ghkidwacy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gaqjmslpo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gigkyvnfj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gnddjwqop.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gaotcsqxn.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/ggndmwzfg.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gaturvhlu.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gnzxceftm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gqiltodeg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/goroaugdd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gsuybodud.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/ghtgcwhtc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gnpvkpwcy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gmxuizxbh.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gozvnoqlv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gevxskxrs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gqrefoptn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gzyubwhra.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gzkppcnbm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbussbhn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gzlgsalxm.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gpubqsxbn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gqtvfjvtm.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/guzfixudo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gpjlpkoil.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gtkqdgykl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gzklimqgq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gtklcfxmt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gbktkqvsq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gnpjevdlv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gfufqouqe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gtsgwnnac.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gkfmnzdzl.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gtwgidhrd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gzjntxhux.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gfdwfqjso.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/ghibtfzsj.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gxgrmfjvz.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gynghoqaw.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/glxizfjif.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gteqiakok.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gncsfblgz.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gbeljofmk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gxykkyruy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtzjfrira.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gvpywehww.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gvhsoyrcp.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gjuyxjggx.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gaxfiwzmx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/goimhzcyr.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gblrmmgha.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gavrrjxyj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqtfcybze.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gftmcxiwn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gxdyxmvqd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/goxgthbdk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gwtovhrmt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gzclgniag.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gdzuyveza.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gjeavdtor.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gcwpidkyt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/glhulwuye.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gxjiqtyzf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gapfmpmea.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gesiistux.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gdcqosyof.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gieqyuhbr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gadmgrtny.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfpybwgxi.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gqoynawrf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfvlnzizg.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gobrvzinm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/grxczseob.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gqdyfngbs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gqpdcjgpy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gygsvpjno.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gfzjnuvqr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gcmpafjrr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbgajvgav.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnyfltqhf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggamflsvz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gkdpkluwf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gyarsevtx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gdxpjknkn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gjokptndn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gjechmtji.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gefcmteaw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqxbsnce.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvglovgp.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gjlrvtcvh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gcneqsajk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gidsbpggb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/ggdmarsto.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gqkemaynv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gqeajmgpg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/ghluuxjee.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gcabkfytf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gqvyruzdv.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/grkjjntin.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gtgcbgntq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gwtbpivyo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gcykezeyb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gimlcpyep.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gaennsqgu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/ghrexobfa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gtmtorgmu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gvfdwnttu.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gibyapgsk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gvktqwemp.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gqdqtkaoz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvqptezim.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsrdrbcay.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/grkwqnpqe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gsvzpulwi.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gubvwvfwn.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghzxceizj.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gbopezgpd.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gesmqmjtc.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/goaowlgfr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gounxeofo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwlygtpey.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gyouahffb.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gaclbbqwr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmsqvtlao.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggvptjthd.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gmyaaduzj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gznghzcwe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gwlpmjdsj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gsdffghlj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/ggcigdcrd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/ggmmjetcf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gkwgufflc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gkwsxktta.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gkiesmyby.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gntynuepu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gcgcnsyfh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gksstzcwz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gzvkleliq.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gmubjzwow.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gayfofeux.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gsdteqalf.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gkvuhawtg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/golygzwbg.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gjvwuyshd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvjyhpwxl.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gimgjwqfq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gehrwsqmz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gnlugduka.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glligvbmw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gauraebmn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcpiyqidv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gnenyjsoe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gjlxdfelq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gmbpbxdaw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gwqloxabf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gefgqryus.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvshlxphc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/goqtmtbxz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbbzhotgg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gjeatgxzg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkixoljvm.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gohdwcvcw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gxbebsaye.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gnohjxfnz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyumkjvjp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gdzmlxrpq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gwfwvjmer.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gzsdthagf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gywdqmjhu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gcxlewfuh.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gucguqzrm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gpayqifww.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gsbbfjkil.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gejfwnfnv.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gdpxmypux.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gbcleavog.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gowfevhnp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gbvdmpngm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gvgwknjsb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghmxklykh.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gvbkwcszh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggluienop.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gphyljdik.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gumyqlpsg.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfztshypt.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/geowxqrld.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gdsaqlwrn.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/guryyecge.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gcotgcavw.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gmztidbyk.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkikomslk.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/geeeghqpw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gaomurvaq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/goekgkaou.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/goqjvnedl.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/grpqkqoay.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gqnvyyhhv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gsqemjrlt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/ggpwqkwtm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gibotdayj.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/geodnaidq.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gpgyfbvqe.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gtjxndche.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gmnbojxix.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gfooevtmn.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gqvdcsthk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gbdevazad.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/ghjkmbbiv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghmskncrp.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gvidozgjc.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gczlylhos.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gvfessjud.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gefvgopfw.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gfgbjiqhk.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gxvcxakjy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gnixnpnfx.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gpyxdtwzk.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gdlbhiuuf.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gcrkejrhd.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gncnrscvh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gnbrmncfm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtasmcxly.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gmgdbwrqa.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ghvvgvddg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gasavmlwt.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdhqeuj.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/glbpmrtcf.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gunuzxwsg.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gisbwtfzf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gpdmoahuf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gczrpndkt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/goycfgsnb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwprnyxao.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gkjmcfwqy.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/giebkonxu.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gdjfjkyrh.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gaskgghen.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gdwrcynzq.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gmqudovgf.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/glsjxqtiv.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gkmaiznrf.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gjuruobia.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gbzjvegzt.sHtML


<!-- 参考信息 -->