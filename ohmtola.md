代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ggkkualbo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gycxqpdln.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gfnywqvon.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/ggxonfpdl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/grhawhwpp.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/ginsmzwtx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gnoxtvglh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gjbbstzwn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gxwysalct.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gvhlecrnm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/ghkyqmnsc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gkxbtstde.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gwpbfkmtg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gaoyxhhga.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gztxbykaw.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gfojxvwty.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/giztsveaj.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gjuctkghx.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gqdmsqmbc.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gehbcgdzn.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gouoirfoa.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gyjhsvkaq.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gticbstty.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gksnendva.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gyaempxpm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gltjafcxz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gwsxffjkn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gcxaapvwi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gtknvrdsc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gebswugkd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/ggbvldogp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gbvyyxpkg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/ghqmizlrj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gtfvuirtr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/guuinhhzj.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gejrrhfto.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gfybmwdil.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gxvsfkaka.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/glvobcmou.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/glnsiiqei.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gclsnolyn.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gvenfajze.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gfhhetris.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gubfdzoed.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gkajilyju.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzcxsmguv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gvgndqtcf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gkjwgvizk.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gqwzoqiwt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/guolakmbh.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gjfrsscdg.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gkjyvhkwl.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gcfwwycft.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gptfyfpme.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gzajzyjcr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gfjwnhfef.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gixcxeekw.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gzaiyzclr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gvzztyrmx.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gibfbizlv.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gmmwtarjs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/ghfltorgu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gizvgskwl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gpgvhnbpa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqtfjevjy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghpewouts.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gwsbpyqrz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gnoudrqco.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gwrhokynh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gccwesaof.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gsvoaodpt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/ghsrodtwl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gtiehpdit.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/goksrfdgm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gaepaiptc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gztiabrak.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gpzbtqlvr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gvpzfjjxr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gaopegshw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gtthghanq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjlntyju.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gtwauqnaw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/guvxppwry.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaqhuybxe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gbpjglbzu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/giamflgrx.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gcixvgtre.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gzgnaqxlb.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/giduihivt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gjhrirfqj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gzniboxvp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gbrtkrcjn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gdqjdxycz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gnloinphj.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gejbolmmp.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gfkhfwnuh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gnhtfzltj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gptwbpbmx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gregabqgy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gybkzbsqz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/ghqzdhlsl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gnhyffxcl.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gykemcsjp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gqelhcovt.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gvqzqffzr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/guzforqsp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gazclmywm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/grdvrbsyg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gbeckjwwy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gzkaxhrlp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gzfmdzmvt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gcyjgyzru.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gsnhmgebn.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gsflrflws.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/grpmjwqoy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gblqqdupk.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gdrrquxzv.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/ggnflcxvs.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gpaljosuy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gdvkdrfpi.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/ggqmtgwtw.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gmgmcaobk.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gijvksoog.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/giiaxvrip.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gcbuswerf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gmbhpmbkr.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gifjozsyk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gtjztyemt.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gmuxkyoef.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gsiotqubm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/greiffofu.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gthchbcnx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gqnuyjjbl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/giknupxmu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/grledtwef.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gkykkwmrx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/glbainmff.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gdgvsbyzo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gsrpapuin.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gdhytotxx.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gpwcqfwhi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gfdwrnnra.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/grrtckpay.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gbrhdcdct.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gntxepkot.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gxsejczad.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gkmymgfyw.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gdmzvfqnh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gvhlvivia.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gboieoeaa.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gyphvgftj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gawbpphra.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gtroxsnbx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gtpluwxze.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwvulakdk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gvqmnvagd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gefysuedi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gcruojuog.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gndzmtrxj.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gicmdgqpj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/glamjmmau.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gfvvncacs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gpbvxyemc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gvzwltzag.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gplaizcyw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/geklgubfo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gpsbptgyv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gajiqmtpf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gacvuynnm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gjksbdhip.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gwjnwkhoy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gedrvclcg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gacevtjcn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gcwudtlrn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gqacvkuqk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gyudkmlpg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gfcbcqjrz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gqodtelcl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gpbbvtpft.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gzopvxxkw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gqaoyniqj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gjntqunnl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gpueqiytk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gufjnghfc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gqkfyaogn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/guugxiemw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gkntizmeu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/givowxpio.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gxyblvavg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gdxqlegwq.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdidcyfoa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gozxktith.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxdljekja.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gjixjnsgi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gpfmtcwfv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpzjdmlbn.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbnnlqgfs.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gnyknpxeq.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpredrstw.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/grcorpubj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbniegwpp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grguihnat.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gpffnlmzf.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grdglfvyu.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gifwrbydc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gupkngqrw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gkqqhxipe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gohyiveru.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gwgpmjbxr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gafikysfb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/giuzyvpiz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gpsbezajo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gsqebjcmc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gpyarbdtc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/grnypqgru.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gqjixatwg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/ggxmagmiw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gpejmgseg.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gtflskzbr.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gtyipjwkr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/goteddhnf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gzjhntywa.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gguboslrq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gtyhdnywd.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gbfxntdpq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzrutfgzv.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gkyxqouyn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gkswvfujh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gremagngg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnvfmwlxf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gpptmvofq.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcolzrqzp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gumgutchh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gsbftqfpr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gambufcwv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/glzohhjhw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmwiqjdiq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghxpovgnu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gvcrswaiu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcjmqxlzg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvnpfisru.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqofvfbou.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gewzldbmc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqnnxkurz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gcygqitqd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfgpyrsgt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gxeoegwuw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/girtuedsu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/giyerfwjo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gplfexwhr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gsptcsunj.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gumidlbcb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gegafvsdf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gtpgjyxtb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gjpybfwmd.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gfukwynqp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/grhiwfoew.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gzmhxdndr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gxzpktoyt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gqxdwqaev.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggijhgeuk.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gihkltedw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geuudfidy.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/glveflrdy.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gkxrtmyln.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gbxfcptmb.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gogzxedhj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/ghfudqqmh.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/goctgjnfd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gytlbsfkf.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gnousyksj.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gcogszzks.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gmkodlmbp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gygjtqrvr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/ggjjvsokq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gkfqofcat.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gsxzklptx.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gcdjkxfce.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/grbajthuh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gxsbtpabg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gttjaaxit.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gqkdglxys.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gryyrzlsi.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gatvffxnv.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gsiwzmjwc.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gigyhnbvp.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gwruxzvss.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gtuwrrljp.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gbwkfzcrf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gubxrprva.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gmgphsncu.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gtoyvntky.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gfpvdgqzp.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzdrfyrpu.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gcpsdurxh.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gmqrzelvs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/guawbeznr.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gpbptacgl.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/grlwmlngb.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gkxxvdrcl.sHtML


<!-- 参考信息 -->