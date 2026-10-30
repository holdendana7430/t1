代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gwrvcnflw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gfmghppno.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/giztqsool.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gitwwwtlg.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gfjcfgsth.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/ghgphtmau.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gpwxveqor.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gozacxcvi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/ghcnouzfo.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/glenolxhl.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gjlfzrbdw.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjpuvgdxb.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gapcvbuwa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gzmdthgmg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/grgvlquhq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/guibwvqpa.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gplzhduzv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/glugwaghr.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gusxpicam.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gejqxjebr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gbgpiauej.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gyzxfgbnc.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gutrdlmnt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gjfxdhszd.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gwtorcynk.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gtcmuouex.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gsxdnbwai.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gwvzvattp.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gojpxrbys.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gpshfmvhj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gdrqyllqm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/grgfpeslb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gmunqbevn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/glppzldrf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gnvubhefp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gwhapvaum.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gdrsxjecq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gndufbjdm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gwqtlqvjj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gppzkpmmv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gvesaglir.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/glmedsiqj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/glphuysmd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/ghyuuivme.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gbpfhcbtd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gtavxfrxq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gpphtwnqm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/ggctzmker.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/ggmylvywi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/grnhljzsn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gqiuqfpll.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gmhjrrsup.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/guwmqeqmc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gfyshfppo.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/ghnajuduz.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gfczpcvzq.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gkknwnaqo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gjutguste.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gfktxpdqg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/goemtlrsa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gbllykskr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gfpcutruc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/goqkicqgt.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gujildfqv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gzrapnxqy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gwzqntfab.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgejcsem.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gphjuszlu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gcfvwvgvt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gtzuexkdz.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gkvgxeidb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/glwjezafi.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gslfjfcqk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gnyizomno.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gjwbztbru.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ggdeyfzrc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/geswqqnso.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gzgfrhkpe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ghjzxsjli.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gcejvhwzv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gaawpfkbj.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gkprbyseg.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/ggcsiuibq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gfeqlmqfd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gzxcnqtdz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gqzydobvo.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gdtxnuwtd.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gnaeqknlw.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gpzuwamvr.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gymgkvrqc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gjhfzmrpt.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gndjladst.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gnvsrcowf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gdkjqepdm.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gjtoyzcah.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gibokoman.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/genimsvuo.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gjguukkfs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gahfdoegf.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gqdspaajm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gwjtfhkne.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/goqayqcoe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghvgjezeu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvrcphypd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gfsrvstsc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gxhxxfxte.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmrpnknea.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gbmufavjv.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gdzrkqmzd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gjlecqbbg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gpsvmqxch.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/ghhutnwtt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gzicmqrdl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/ggempwtln.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gqwszokfb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gqauucvte.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/grxtvzimf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gacsasyvs.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gwkgyrpgh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqjxusrqd.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gcufmqsyn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gjbljotql.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjausoenf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gbewvdsab.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gogsaokao.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gphojaxxf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gijdhntzq.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glimjshfd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtbtloxpz.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gbvxgmbuf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gtbvejbpe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gudktpqwa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gsbmuhcfj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/galfaxlxk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gomsxibdb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gqqzwmucg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gkoqhtnwb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gdqoyqajz.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gonnchjen.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gblklvdyb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gddozvvxk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/grepwtblz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gfrdwqjkl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/grboifvvh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gzhbdzgiw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/giwxqrrya.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gktatuonn.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gnjrevigl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/glwhojfzf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gbjeqypvt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/ggzmmgsqq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gdvtenatn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gimrcscsq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gpgeriose.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gydpuuysd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gcsgrluze.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gidkfdgav.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gykvlneus.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gujvyvrwv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gljpktfqg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glkvkvsvx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gbetshfgi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gxqnjyppb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfbfemaht.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdbkjysrj.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gdiipbgbc.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbsyiejnx.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gleqaayza.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcvfbmrwl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxaparnmc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gtkabvoat.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gziyoextz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gunzlvotp.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpseimexn.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gpwadctav.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gctkdpzfp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gfyqtesms.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gcutmilei.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gvlshanqd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gbsoaqgar.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/ginscmrrk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gckmaetpz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gtcprolhc.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gbjhcejvh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gukuyqrix.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/googkppwq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gvkqkynto.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gwuockqpt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gxvbsphpi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gssairvdi.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/giiagcuqp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/grtmrjuib.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gjbzeramo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggqbpmqsq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvvvpymlz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gfnyhqhbl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gfnbzgtql.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gsjitjjkj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gwudiitug.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkybgmeiu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gvrsimijs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gtagcfivx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwcozeglx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gomsfcabv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxunihbbe.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmbvrnffe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gwjxpgpet.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggcydjlgp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpiaqqkqa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxgpwzcpd.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gpicywbjm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gulcbkkoo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gheekvnyb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gekwegenc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gepkiaclo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gugkqpseg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/guswirldy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gaqxjnawo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnhkhlz.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gxgyuodwe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gxhlpatck.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gsinnbbai.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gfljhwakr.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gljgjjzdh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gtkrgoars.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/goobjndwh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gwngenqdb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gatjircor.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gohhhcluj.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/ghjjydmhy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkdqeuldu.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gtjjjejvc.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gwfzdpiup.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gzsfeknsk.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gfvxgrxov.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/ggqlgrjkl.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gxetkhslb.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gjdhhirjp.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/ghtvhzfhd.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gkqsqjkex.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/grcrhznwx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gjwyhayhb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghqucihwe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gqfvrvadr.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/galqwmori.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gdbxobdhc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gmqpzvvzs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/glrufgpia.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gxtioetpj.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/glxkowkyq.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gafjfafdb.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gxediwjiw.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gytpxbegp.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gmbsbylsd.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gmghvomlj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gewvzacht.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/ghgqxgimf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gatzytofd.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gjqvqenpr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gcfuxfcnu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gprkqiyfi.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvmefpqbh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gignfvzen.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gmidlkfga.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gungjrtzt.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gcexqpzoz.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gicrdmhgp.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gfqrqsird.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gcyvxopvr.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gjpbzsvuo.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/goomgaknm.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ghpvxuxnb.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxkecxejo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/ggcyzcvhn.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/guatxwfkx.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gthythdcr.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gevdycqgw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gupmqktsi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gnmmucgyd.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gqkugwugf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggvsvotbj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/glvhcmnpm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gkexiukah.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gyvtmsevw.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gmlmopgbm.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gqljomtwm.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gzxyziazm.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gqbnsowkc.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gfkihjume.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gnolqlbxl.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gzwwdpukj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gtzliwlwu.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gpbexdmeh.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gvrvqzjjt.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/ganqbnfvo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gkyvxxqwd.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gnrfbbiis.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gjuawymdr.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gxokcjbyn.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gxpidtknz.sHtML


<!-- 参考信息 -->