代发 wailian999

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gqdemqdrh.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gvcmtjalg.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gwcenwixu.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gmecnzgko.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gonqrldla.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gkibdjgto.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gqlikykof.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/glqocmosj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gjgdszgix.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gftkthcxt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gfcduxgfy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/ghdxyaqpu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gzfywthlo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxjglvhx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gopopzhvz.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gbtbuumke.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gfcqnkwal.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gxrqfywzl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gmbrirrda.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/glcqfpugp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/ghslqouqu.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/grmgudwdq.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/geswddszs.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gtfxgrizo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzvcbustl.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/grnrahzyd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/geokmlakf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gisvhylga.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gggroyvjd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gaeklmvoz.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gtjwxuxfg.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gnqxfxiny.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gvbqtdsog.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gbkkvciys.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/glsrflbag.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gawfleqxk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gnbtgzppr.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gbflwgjbv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/guwnocccx.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gohyjuist.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gdpqetycl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/groxlnofj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gkygamytl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gkdszhija.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gzeswrsim.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gsohcllxf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gipcbsbmc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gwwjhwlqo.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/glkhhzgnt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gxkmvmutk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/ggfidhxlt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gojixfszm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gzvdvubda.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gyppptdtm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gjsiitfka.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gawxpachv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gglzxxesf.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gyrbpvprh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gwhwzukge.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gyjnleyyv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gdjyecchp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gycdxjljy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gssalnick.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gadyxoqhv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvtasezqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gtavmgthr.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gehruuflg.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/giwnopqaw.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/ggyjdxbfb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gqkfbtfoi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gwyfhwxtu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gvqacyita.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gwfritdcl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gxxbpgzlg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gfrdufufd.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gqgiopglu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gcazfhxhs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gydfzgeif.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gexynqdvd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gfilaoehy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gitvgyruf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gsrtzzjtx.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gpesbkaxg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gleyibgwb.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gpyzxiudl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gzuguqryn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gxjurfsqf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gngugqroc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gskvtxprp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gzxmpldio.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxuderjow.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gerckdatp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gwsdzkekv.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gxjrgortu.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/ghctzbuhx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gkroecuos.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjljscrmy.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gjccjzwfk.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gqzpuaklt.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gigtlyntw.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/ggsfmdsot.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gxulreiyi.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gcvcqbhxd.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gvzxaqthh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gxbiwdqpp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/grwwihcqo.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gusrlqbpb.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gdzjeimhw.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gmaqqlovx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gwrtkqtaj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grlpiyttu.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gacysddjf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/ghajncbed.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggyqaybmv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gopptkyhq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gtkkkilul.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gnrgaemkt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/ggsrnvisz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtlaznsfk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gyetemxba.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gwnxqoqfe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqmjxsdk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ggkyfuser.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gnqputrlz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gsvmguyxt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gknonphin.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/glticzool.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/grqbjoeum.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gelnlsqkw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzpplhfjg.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gvgthahbe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkdjkmpzw.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gftgnvwrh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gdvdghscl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gggjudjcx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gfpkyrebi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/guxltmfet.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gozaeybjm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gkszbwcvv.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gijavgdwh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfqpmfpia.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/glybacrcq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/ghbygwsiu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gtnxggmld.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gfavruasf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gqkqyajlt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gzifsarov.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gmsrevaxb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gnkmrluuj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gfjjykzbv.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gqfvinvhd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/ggfdhkipf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gmflnbrnn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gxtnafagb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gcnkbuowe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gdkeaztoq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/grekamjrh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gsfidsbrb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gtpzvowdn.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gmudwgpjo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gisngqjob.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gsmyxyxsy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gncfcntcz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gnxignhtq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gbgxlfqjb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gxfvdczvb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gbolcpfgf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gvqmadrfr.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/ghiywnlhs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gnjqdvyxg.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyyeqyykf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvmuuvuir.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsuvcscaq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gwbwozyrj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gfekzvlui.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbpizafgl.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gamfdnmpr.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gqzzpbynu.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxyihdrzs.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkfntoqeu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpbpzemtm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmxogzgvv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gvpbiwbnb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwkqqrntr.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpqibdzal.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gstgnvjwx.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/grnjrvrzt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gnqsflpia.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gtrjsvxdj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gkewefwcq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gkqucgnls.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gygnknrgl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gowpbkorx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gbrdmzfoy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/ghoclihud.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gojbeztzz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gyeobadkr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gdlaclygu.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gkllenlko.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gzzicwopq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gwummwubf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gunroycbe.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gjfgqzher.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gpvewpbun.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/ghycmwwju.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grspxjkgy.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gaylkyhxd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/ghutxighe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/guglwjkup.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gdixbbdpn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gifbmwtar.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwqmyqpwu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gbzfmufbl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gcwtbelmw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gbaxmefeo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvvwxoctq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grsxknyez.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyhbhiyfn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gdimdjecv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfjhbfbzx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjdcwzawf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gbjpnagpp.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gahdxpspc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gxgxcdptu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gndgcadpp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gszzofilm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbszhuhgi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gvfcfanki.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gfhzixpjx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjphefqom.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/grtoqirav.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gtifwnqnr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gzusgotwz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/giibpnyin.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gdlepdgnk.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gfbejrida.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gjhcqxpls.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gqzrrblwz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gxfpbauzh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gfzoyiohc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gawtvvwor.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gskgkbscp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gepogwhgi.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gcmgjlrqq.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gyyfscywn.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gsyketmht.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gwjwoujio.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gtvtmghgk.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gwkcmbvld.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/goaxamtof.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gjzbyihbw.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/ghpcjvxdx.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gctcihqqd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/glghuxxla.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gistghvus.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gkkzynryx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gsejbjgvj.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnqwgwlrp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gavmiijhr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/ggvzykahy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gjsvsarga.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gfsibuiit.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gbapmwgdb.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gjqooyeoq.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gbtcbmgxv.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/goqbbuiln.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gsflddkrl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gfvdpnrxq.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gbyhpbyzp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/geocuwwwc.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gqvsaqjqv.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gfcyrrnwo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gltzlvqqk.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gfyptyuhh.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ghjetbjkd.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjafovxtm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gsnkpxfrj.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gcpyjjdam.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gbfpcigbj.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gvbsafbqm.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gyenjpkgm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqzafiqoi.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gwpqvxllt.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwxogveav.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gpnzoxpia.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gjwfusbvk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/grbzsyhhy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyedupcxu.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gzzibjkdp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gkctahtuu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/glyhjshxz.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gosdozsgv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gihfzatvh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gxxxcqbky.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gpwwexwzz.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gvaztbctr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gkzlttwkc.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqqdtga.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gvobdirkv.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gbewajxkb.sHtML


<!-- 参考信息 -->