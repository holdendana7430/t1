代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oqgsvvwi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ocorfdtn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zbeyoxfw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3avgassur.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3lrqpugxu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3imjddxsw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3xfhfmovq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pcgcpzdd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ggftzmxc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ffpeswke.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3emwizlhh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ueulqrfv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gwlhpysi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3oyrosnin.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vjjulljo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3seecnohd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wuevkext.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xvyiuygw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rlxzbfoq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fhywjqhl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wdmlwbya.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mvafmvro.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gybeomdt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3hxfwkrzu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3plwxqcea.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zujmoiob.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ejelbzem.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gdhossjt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dmhosqdj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3shxmkvca.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ecbquqri.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vptzpoha.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3uelyrbmo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xrlogsjj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3khjxkdla.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ezjrbkzx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ukyddopa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3bcyaboej.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ptqwgula.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qmrbbetn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3liczstfm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3icyzjcai.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lwkizloo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eaklbvcl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ufrexkod.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3netchxav.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kfsjqrek.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xspngmoj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zpfhnlxr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fqbtmgxr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3codbjsyj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3onslxbms.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bltkujkl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oheorzne.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3auqvoxpo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3acjqakle.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rarfifmn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qjdbprtr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bnsnztkb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wdreykci.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bcxbkyfp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vzfctqlo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mwhfiovt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tubttaud.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wabnmtig.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yswudbuv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3lyxnwbmv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rffzmtbp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ginlqvaq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rnhaavxe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zzintxlj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3odiesafa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oiatgeeh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xluvhedh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3gdbgxaid.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3buxqtzrs.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3uqsjuvih.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cdvycraf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3geazprji.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3loqwubum.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hjrknhoo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ctexkngv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vushtcyd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zgibwimb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3siwdnnrc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3zutcnjtc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aceljsab.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jzpiibfv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ibuwhbrd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pvxkwzwm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lxmmbbqn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3sahfiqib.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3crrjyyui.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fluizetf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jwemelqf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nbgpseek.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3uvupdefp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ezmlzkjy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rjybizcq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hjbgavai.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ypgwcfcd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3kovyqwya.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3uthbzcqs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lztenfvt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bgywgrzl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3enbbzwng.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bfvvwxou.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnlfzcpq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zynkaqem.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3enctybse.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cyklwsjm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vnwxfqlt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gnponpre.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3mhzaydkx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3aaciwygt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lfarxogq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3thiewucf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vaybxucv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lqppgcbr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3nqysmpff.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kxyblvlo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wmwpleph.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3atdgigok.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3igobgzbl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ouqbohjc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fbiltqne.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3occzknjf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mlfsfqhw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qvjiogif.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3etpfuyhu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3pjkuoutg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ktskyqfe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wzltcdbv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfwhiynp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3snkyjqoi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apgyqhaf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3udohlfqt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3yplnaovn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yunizcvb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3pswgngzx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3narffkus.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ubsapdzs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ajqjcahy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3meuvbiww.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dbdgqndc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bajglwsr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ajtrwdte.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qmyztuki.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hzphlasx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctsqpcpv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hxcbznvr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vnqecvni.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rtboubnz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yyxyviqa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3iwqjrsth.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3usvsazfu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tkidhykj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snslukhx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3jmxtbnqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqfebdll.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljjiyycd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3opgbdfai.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tgngxsif.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tydazvry.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kmddwoqr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rzxeuhlh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wblwqopk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vessldwu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qpsvvqgy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dlhaxjez.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3rloxtuld.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3iszkvghs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzirlfyb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3habdmjob.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3budhbyvc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mqphrlin.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3emdamocx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxxpwaam.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3riesnlhq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rqfcmssm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3sooozdxa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jdfdxzhl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gbtfadpx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dmglwvxr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ibjydvks.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3iiejaqkh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mxjfgawy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptmmgbjk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3apldalwm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3djearzqa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rfipiira.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hevvvlwv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3pqooonsg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3znrcrymg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mubpmluu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jrdcojhv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hcbjxmof.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3aeimfcdw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3irvwddxx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xruyqzdt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlnrrsei.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cfcotrub.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3toyrjfnu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmiuixqo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftyifzdy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xxxqddlu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fosqmjov.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dyxefvmz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rftrrrvx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbuujqvh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ahnsrnzr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxkdetwc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clfertww.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rppkrqmu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gjqqlbwu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3eguftmgr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ovoymkjd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kmsvljig.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gprbmlti.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3eyehsjkx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3wblawymt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lplfsyal.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3oolcplwa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nqazygvc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvrxcdq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vpooyhfk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lpzlmpow.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hctqqafm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uyihtkdc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gqxffppe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tatzttxb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pfvqasqk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ipeaxtik.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qoelcafu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jmsspivc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3arvixvsk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cbgraerh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ggzgdhna.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kwcmeiqd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpsdeets.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3afpikcdq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zfyddtde.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnwtemva.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pexxgrkw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etbrorqw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfwfxbvi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3agiodexz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jgavpdcv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvenoggy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rckvcuut.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3uwgmpfsp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yvhwkcvc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kqvppspy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdudqhyi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3arezbubx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vjxseiqf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ttlysczv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3muxoctuv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3oxvncwwr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3crcmmjyk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3cwnvafdg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tidiezas.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ysacwnyo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3etqsynoo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zseiwqwl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vgamwyvi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wqvzskze.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rxmmpesf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwdcsimv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3sbfizcpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3natglzmq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rtvmmvux.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lnltttnx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3drjmuajl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xqzqgyhd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kmkhwqmx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3loqlqgfp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wwgetnbu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xdwekbqk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ameqrsrj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3caskfhaz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wecfkdbu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhhniqgv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kufbvwcu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kxkayvtx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnfinpif.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cecwecdv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ixeqvnwy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvkplfup.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ceykboon.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wuwklhxy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zwmqclcm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3neefgcas.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ppoxrsvi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3bblfgcyt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3iwyghbcy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lcnsosym.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3orvfqwmq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3flrxarey.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yyyjjghb.html


<!-- 参考信息 -->