代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dzabekhp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cygsqwqf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nidaokot.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yddyvlio.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qajdggck.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2klunwfps.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mwrsumqw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aatynava.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cmooewmp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wizfcdir.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tfwnnskk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pnbvyoco.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2waefidcm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cutzzgjg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uimbjdzi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hdzgaizr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zqcmjetm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bdtwisnu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qndcbmws.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2edaglwyo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qvgcfshv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tzbafuxg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2emwqpkrl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ahawfwqp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2muvwkfto.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pjkzfect.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lkvzorxy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kpkktclp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vszxnqec.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yfvkrhph.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xutumiox.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kykvoaab.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzdujpyc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rophkfxk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bvojajqm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2agfmpdfl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wdwdzbbo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gyjimunc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rsedinpe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2njkanfqi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ubzetssm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hyrkszsg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2xqrodpiq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qktptcnj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lwwodpib.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vgppnhjf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vozvvhde.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wbsqvlkw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2fokywrjr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hxzcnwxk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sxkrlezs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mbcgofev.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mnoxattr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vqqvmems.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yingevrw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zisrunib.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uwgxskgl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mavdkmxr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rnigtvea.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ambblvsb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rxmeiues.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hcrrkmtr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vtjehfdu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2viphmmel.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nlcsdosf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kovlgvgs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2kbuusxrs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gjqjswej.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ulwvmmpu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdoxcvyg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2envlnoyh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfsatpnx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2edatknvi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fjwdvxav.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tpwhfyca.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zcavmnog.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2naxdqsrx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2bmcbadyp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2mfclbxmz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2zsihdxbb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uawlbewo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhzqajc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tanarszp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2htkvekjt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hmbvoyfe.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tyzpetan.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hyebvfjx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pqvussjl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2acprmfyq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vubvzusl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2uwfmmaak.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bpqybrkb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ruefxqtj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2drmslhmx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kbnpxqvb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pydhdaiy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qclmteha.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2irfsmfgn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hcvrawqh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2adifqzcn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xvcjyuvn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vxydcclw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jwhphsqp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fnjfepmb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rylnwqcy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2euedezgd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2usnhriiu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpsnytnw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixiaouho.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2uqapxcnc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nwyrhwfn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kdbeaevg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yntizzlu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2xtgajxvv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2twfqtlgq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hqxholxu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jddktwyg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ewjbypnx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vyyondqp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hlncpptv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcebdmpf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ohstuzot.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fummdpcf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hrtvpmdm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ruoyuqqg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wgpadpce.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ujvvwmxh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ibkxishr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vhnclbrp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2rgjpzcem.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2cfmkgtlz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2umvkhimi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ildohmdt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkkkeybg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rncjrhoy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfkpeqdi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2aiomweyf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jizukwyj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itaihywg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zyxwqrup.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qlqputfe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rboxeuka.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lncyrgwa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kltuqatv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2saqhidym.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2nfryrpvz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lzudildm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rwrjdubw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dflyoqne.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2avgabppt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2seoashur.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2urccqtdx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gkinkovr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uvsvlsmq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2nbvodffs.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ljmcxtet.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gxchjuta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iicsupis.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qzqactov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usypnnid.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dozwaame.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bikpojkz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jbawbxbh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vvbmorlb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2llmqzkvq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fystzukw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2afruvwba.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cydavphx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uzajboob.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2evahdnuw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wtvgkqks.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2otqcgzlz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cxpwxodz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvfssfca.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wlyezpip.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2iequcmbk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2wwhcplaa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gmslrmdw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2sihvjrjq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2bttekgjj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vszloohj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gvwtsruy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2veqkqavv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gvgdaoum.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tvkfywtw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bsooevjo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bguhwwxp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qncwqedg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aydmcnby.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ylxvbpxv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hbqsbwez.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jruokpbt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vxyyheji.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cszvydln.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bmoizhlh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uajffcct.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2txcrdnpv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cfhxvihq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cvlwcosi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhrodsgk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofbndotd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kuhtzumu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2thfnpcvy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulimwcsx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbqtdpaa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2sdopcpfd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xjdujpyk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhjlwgrl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewakzlpo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijhjnbme.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vzdublgk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mscosmos.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbfbhwla.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jfsiabmg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wvxwdoax.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qvtnwpvr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2phcrqxmy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xgrrtgtw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tfqypwox.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2npbfguro.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wupxtrho.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2nmgxtzqp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dnjdhfda.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2uhhiqjxp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2myzsqynw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqswwrzp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zuswhgaw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nrcrjkpq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2awfyujil.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2inmpfgec.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2frhnasql.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2isnlhnlo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fxxaxnzt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekkfxpzt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zpwsdkyo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2llxtnsfz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iuquegsl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bdigoerx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yfkcvvrx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wblsxhje.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nxidrcmb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hsakitjb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pztxmxvy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bfszqqzj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmikllfi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sgplthqd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cockrrsb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkdceihn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aghmhxfc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewxrazbn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vucznmuc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sxovejbm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2afklwkil.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngwjpnqk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngxfnshu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2imnhktjr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2yuqswfjq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdtebvwp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2eikrajiq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vkorhkwz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2igyawmnh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tgvdjktq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2axdenfzp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uvxviibi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2avadsgcr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ouusgvel.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vuejmpwc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2yqhrmtrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hftiaacd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gkkvvuqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tecdrqvx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2yfxjtnuq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2obblhykp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxsmboit.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2shlrvocn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2zpsmghdm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xfmkuaed.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hdpneizm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qgyyxdot.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqghjhvx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2njofzbog.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jqatjxpz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivyoqgjv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uluyoywi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmvocxlt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nalgllwx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2aqplzezm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfubqrup.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wxvqgwox.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hsghpbjs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fyselinh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2voqbxzxd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tunzlkmy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2grddjfqu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2gjstwbwn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2sqntjeug.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jcihwhsw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fjezpnfj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gcdyfzge.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gzyvoaww.html


<!-- 参考信息 -->