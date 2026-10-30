代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gfsuzkqfd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gzvnujwel.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gxztkfiht.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gzzbqvizm.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwlwzvzgb.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gqjvxqyzs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gxsbrolib.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gieqkdqnb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gyuerfsze.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gbjdofbio.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/grcjrsqez.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gfqsyaiii.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gchwzmufk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/ghrcpisus.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gvmybjsbu.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gsclpnrcl.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gutdxihop.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gogxhaxml.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gdcptyajb.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gxlthqnye.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gfqayaohj.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gssnuexsi.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gpmaoeyol.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gqrujyrix.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gjgtvapai.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gicmfrvhy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gzqzcgtbf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gosxtmaym.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gslejfukf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gdtcraiux.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gwqrqgkiu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gwvubzxxd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gxdvcjvtr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gikriviqw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/ghflblcmp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gbxwvwmui.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gegvfhbgf.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gzmdrjnjn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gkmwtjplv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gowfayuhz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gqzuzyhkb.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gzfjbjcbm.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gmtokundk.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/grwmyaheh.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gikvyxyuj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gyhtphxru.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gkixwmwva.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gjxiosyfm.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbmenreju.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gsiustxhk.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gowtncisa.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gtdeiwsws.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gllyjjnrh.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gumrwcgzp.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gjrvvziwt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gfphcuxki.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqhkodqmr.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/goukxnfii.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gakeiflcs.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gyiyymepl.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/glamoobxb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gckfipume.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gzlbijsyl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/grnodhrdm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvojuifw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/grrgwskci.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/grwcwttdl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gazzatmvz.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gscdjnokf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gpkrtlijj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gooalhzrp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gwmzbsgdn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gqtetxpdm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/grkoeybpf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gewbsrjhc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gausjjkuf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gqaafodpi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gfwcdqsdd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gvidwjwcp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/giumxgjmb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gjlmtelfq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gyyxgvbxf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gnwwfdqpg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdtcrvxu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gomrjsfzx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gvshxmvxd.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/ghggyvxiz.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/glzpfijri.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gdvaniksk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gevfakmhs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gmdtjbvag.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gnanyizjy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gxqalpanz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gftzvvifh.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gjrfjkoxq.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gipqgjfll.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gkgxuzojg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/grlpwzfcn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gegepuonn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/galotpcae.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gywjszzsl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/ghopfogfx.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/ghxxgcwqo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/geroltqqf.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gssmzxjly.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gslkdaflc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gqynaxksx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gsrdsnfuu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gnsskzhxu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gpkssrvjc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gusubgcru.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/godifrvyw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gycrouupf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/ghrimhppx.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gawqiyavr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/guqdoambf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gseazsofl.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gcrwldunz.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gynpinngc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/grtdviswv.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gxldluszl.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gcqvxksdw.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/ggctrannz.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gcgjehguw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gygxdtkcr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggsfbgptj.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gphhcvnja.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gyfgfsfym.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gunmjlakc.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gozmlyovh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/ggeofcozl.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/grvcrmffx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gtkkohbpx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/goyrlleaw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdvaehzwt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/giwpmgxew.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gyivdarnf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gdiohmduh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gpascqdyq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gtkhebziv.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gdykeiesi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gnypqbumt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gmjuwftdv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gsbdbedqs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gymuukyah.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gcbtyxqni.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gpafxzkvv.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzbecdrwq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/grolycvvs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtylnreoe.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gjfzkouzy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwvjdbamf.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gickbzhjw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gskjygkjc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfdneoqft.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gmygroutj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gonauibps.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gkhcpqibx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gcddwlvtj.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guohdddgc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvvdbugbs.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/goyvltofd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gqhpjomio.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gtgsxnmkg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gkvqcxlhi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gqmagmjnx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/geiksggfw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gxilrbqnn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gfunvzptz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gleilnlsa.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gwcwebmwu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gfcvkuljc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/glkeftptf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/ghpiblezl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjuqunrva.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/ghmgdwmdd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gehgoavov.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gzewmvzxn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gzbahjtza.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gnsegyuku.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gikcfxjlm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gfyosxyhd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gmncxlamq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gmmpylbdr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gwjhhruug.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gpnjsgeed.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gukggfzsa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gninisxwl.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gclswambv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gfqoaocmw.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvtkzixtb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghuveutqv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghwlmfvxg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gtbupafxj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/ggztevaoe.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gchzlodju.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkgzfadgm.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gdxziecpb.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkplewqif.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gfchgpigw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggfickyhk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkusamnre.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gqtdixdsj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzylpxsgy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggpqwtlck.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gackgajxj.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/geozjuqhf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gbtfxiauc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gslutxtqh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gcewkblzw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ghkqwjvij.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gncbazowl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gkphvowey.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gjujkumpp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gaywumigm.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gswvptzyt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gzwbhcklo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gfortwnsn.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gdzuezmno.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gyalowfjq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gvyddvvbt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gxwlmumko.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gqzpjkujp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/geyhzemzw.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gbzyrwmkn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtmuxcccp.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpshayezy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gfobnntey.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gxtjezmkd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gwknpysbl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/ghaucvlbc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmjhyxrbu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gatcianrs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gaeziodge.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjcgcneld.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gukldcxbd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gamiojjdf.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjhxjtwxr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/ghkstyytm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gumnulfnq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gclkxqbnw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gakxkuqbk.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gzkdnhszk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gczhekxdi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gzrhzudjs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkabnxrup.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gsxkobuuv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/ghkyoxxrm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gwgwkcasm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gctdtpjue.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gjuyloxjc.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gvmkbhnab.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gjdcbddkg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gwrhwcchf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gejhmbabm.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gsvsejiej.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gehjehaxs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/grrvvfgzv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/glvaitrfd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/ginjyczod.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwauggfyx.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gznsdddzn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gayezjiax.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/ggufgfwte.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gwrwxvjhb.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gfgdgeizs.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gdjlkqnzb.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gypneujnj.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gsgrgupmt.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gaabnbzbn.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gofgyazjm.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gbzttpsvh.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gpnqtoohc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gjyryoqlk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gqtxcuzjs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/ggurwescr.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gzwbdjutr.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gxvbsnypn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gtykmmadz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gyvphtjyp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gjnqpqmwp.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gjirtewfd.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gpxifdrru.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gxuatgmpo.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gpwksdflx.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gjrtmrhiz.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gmlzuezue.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gznbrfijv.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gjlvazyzx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ghanzqpeg.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gsucvycdy.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/guovmqocm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gsuapslft.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gcnwlwtsc.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gliairyrf.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gvootkniv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gyotofpcc.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/ghavwzxsq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gwlguoncv.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gbespznmj.sHtML


<!-- 参考信息 -->