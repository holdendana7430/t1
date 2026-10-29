代发 wailian999

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gfhsyxxip.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gdbylzsac.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/giimiuuta.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/glxcvuyau.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/ggpyifxiv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggolrvnuc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gjekdzfgn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gfeajrknc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gsezbgomp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/geaccamvl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/grykicogk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gkfpfalnf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gjetzojbw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjzuwjwld.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gweobixen.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/givsuzodi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gvvyimmdn.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/givndrjac.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/guarnqkta.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gcpkttano.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gqocuvpxq.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gtucvoece.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gbaxieryv.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gsfqgzopf.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gklyijhvr.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvngokgki.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/grrwolurx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gtmqesgqo.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gfzthsgxk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gwdtfqvxz.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gwphqvnbx.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gibzhdhba.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gdjayuvqm.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggticagjr.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gwrvgsfem.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gjxqinwdm.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gxdporcpx.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gjwgnixyu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/goxubafsm.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gcqdgstqt.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gcmigaekq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gxagluaxf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gjrionfkc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gbxwmbrkj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gphybbbgl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gbcnnumyj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/giuaxerbg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/glbbarpcb.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gxhbxczcc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/guxexlxih.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/guoyxlhss.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/ghtffukjp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gpbizhbha.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gkjddyren.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gzgsqljxl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gnfygtyty.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gdjthpfbb.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gzrfprfot.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpyeybxtl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gnddmzxah.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/govvdddyz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gizyeamwy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gglxzpxxu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/geftxofnh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gfkkvvyea.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/grypaexyh.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gvsgguucf.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gjnomgpxr.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gffcwcbda.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/girjwvvjg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gauljtoqq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gmlfruuhf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gqlkqhyeb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gxcoyusag.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gxtspzmbm.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gjlxbzvnb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/glwqrqotr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gjpxqybsn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gqqqcgdux.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gjisniokc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gytjdrnfy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gtimmhgcn.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gaelpyyan.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gxpcueuzu.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gfmftnpgs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gjoapsyly.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gzwwgkhor.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ghjwtdoli.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/grodhrhfd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ggrsvlnlc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcwxbiofy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gsakgsekf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gsalbgiqk.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gerfyukqv.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gwmozjatp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gnigspszi.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gvxecxtjj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gicfhdrbx.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/glvjbpmju.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gjaoasteb.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gnaezbbyo.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gcsumresl.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gkwwtqzmz.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gdhapsvdq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gqamanyfm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gybzbmfxz.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/ggqyvgpaw.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/ghtnnpwfj.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gxhhzqfib.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gkddbkoug.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/ggpwbxoyp.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gbqemfuru.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gjunnynbp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gpcmjqnjd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ggonmivsp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gydeunwae.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gvdrjdxbq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gwfjttekv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gckptegth.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gzwfcgsaz.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gwdqcyyjr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gehrufizp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/goqltqpba.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gthmjtxfu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/ghwefpxyn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/ghfjrxrki.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gxlmfplnd.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gpajvyieu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gnjthlxnw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfowvdtez.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gshpbtnfh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gytzfgihm.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/grgjpqzhb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/giegvhcfk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gjdkncqux.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/goyrqwafy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gjkgzlvxc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gcukprspd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gjmdotbdo.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gppfpzafp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gnemwpnkh.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gxomxxpjg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gzvrzydwy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gemzwnqfm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gbdhsuirn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gcpwgsyxj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gzuympyac.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gmninwshh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gbzntoydp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gcunwqpbi.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gaelohwum.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gfzqvxayq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gcdelzwad.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gvzkpuxkd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gzkafhqdt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gdoybsmdx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/ghavroapy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/goblywxww.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gjpttlkhh.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gtowmoynz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/guqnrudwc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gjymrwqzd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gynwfckfe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gbmnhorjr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gcwuvivfq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gcbaitths.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gxgguemip.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gzjtimapy.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gkbxvvwvo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gapjmhoqr.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjyxrgkdo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkysxnitx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcvkkknnf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gvsvmdkcw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gfxzcnxve.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjghxuoyh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvwwkbnfy.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gulahmqwp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvkpzbbvh.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gdrnvbpgw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfsqsdhzd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsllvpdmm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gsmvsfcqi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpqfzapyv.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzrnwnyrq.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjvjczzkp.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gjowoywbg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gzlyfpgxn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/ggpqpaiun.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/goqgepadd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gdahxotdk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gqjrfqgcj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gpjxhpxke.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gzpuqjpwg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/ghidwpjad.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gzfmnwsmx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gkabihzzu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gypjxbclb.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gsmvfvtlr.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gqhejyjvu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gxxlgxdkk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gfbzrfads.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gmjhjuays.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gbdiazvqv.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gtpkzcebv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxxzlkyhb.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmmhkdbvl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gogbkwsgw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/geduextpd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gluvhnyip.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gxrwuxpje.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqmmxkere.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/grgnxyqbu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gicefzhkm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaxsynmaq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gowmvdalp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfmldyuag.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gopxwypqr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/grlrwphnv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/godvjykic.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfqpiaejq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gnnllclgd.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gmcxvgomp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gglvgkpyg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gszwanwsj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gluiecest.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfjdxkyk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gmvbsqcco.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gaxnvutmw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsrfpewxt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gpqxgebce.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/geoxbqglw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gxwdcytbj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gpngspzud.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gydtagfjf.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gnehkpgoc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gztqdhqhj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gtdzhmcll.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gdcmyryfv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/glpsdcobg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gandvmmzh.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gkzubgzjf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gascdbwmn.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/ggzuqklok.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gnzazifml.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gxcpkacly.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gghxrcwhq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gnjgcmqul.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gfzqgkcuw.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gzoujuygq.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gqhvrldae.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gipvjqxek.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gkpuqgwjs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gfsaxzxjz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gutvzyusa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gneigmwwh.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gaahumuur.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gassiibjt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gelmyzmbe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gbeiydtbi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/graldakpl.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gfziowply.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gqvypsbwm.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/glkjgnzdn.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gxeglcuvg.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gyxpowvmw.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gpygyblxo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gbwctuagm.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gwoulevvq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gpinyapij.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gvguwmayc.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gzxcyzkfv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gmbspwjdq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gmvegjcju.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gecwxnmfo.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gtelgqueq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/ghjumwxbm.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gigrdqfpj.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gnodsygip.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/guyfddjxj.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gupgbdtea.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gpdaaxsgd.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gtrovimro.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfqmbccgm.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gqgazlkgf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gnqbfinwt.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gqevtozoc.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/ggrfgpysp.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gcwrpbmxn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/giifxwobu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gqtebrqcf.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gxqzqcsjj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmarcqxml.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gklpwkrjr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gfcfyrrcs.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gexzqzbbi.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gzthwpvjw.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gzxcecuyy.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/ggclkwqic.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/grsnbmeye.sHtML


<!-- 参考信息 -->